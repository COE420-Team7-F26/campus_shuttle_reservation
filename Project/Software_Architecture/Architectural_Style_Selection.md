# Exercise 2: Architectural Style Selection
Serly Torrosian — G00098361

## Selected architectural style
A layered architecture with functionally separated business components is selected for the Campus Shuttle Reservation system. It has a presentation layer, an application/business layer, and a data-access layer. The four business components are User and Access, Shuttle and Route, Reservation and No-Show, and Tracking and Notification, matching the decomposition stated in DG01.

## Main characteristics
- The presentation layer displays role-specific screens and forwards user requests.
- The application/business layer applies the rules for authentication, trips, reservations, no-show reports, tracking, and notifications.
- The data-access layer handles persistent account, trip, reservation, report, and notification records.
- Business components communicate through explicit provided and required interfaces. Presentation code does not access persistent data directly.
- Authentication and authorization are handled by User and Access and checked before protected business operations. Hiding buttons alone is not an authorization check.

The four components are functional divisions of the business layer; they are not four layers and do not require four independently deployed services. Presentation and data-access concerns can be represented as layers/packages within the team's four-component design.

## Why it suits the project
The system has distinct responsibilities but also shared workflows. For example, reporting a shuttle delay requires checking the assigned driver and trip, validating the delay, obtaining active reservations, and notifying the booked students. Layering separates screens, business rules, and storage, while explicit component interfaces coordinate this workflow without exposing each component's internal classes.

## Support for the design goals
| Goal | Architectural support |
|---|---|
| DG01: Modularity | Related classes stay together in one component. Interface contracts reduce the effect of internal changes on other components. A change to notification message formatting, for example, does not require changes to seat-booking rules. This supports incremental development and maintainability. |
| DG02: Security | User and Access centrally handles credentials, role checks, account lockout after five unsuccessful login attempts, and session expiration after 30 minutes of inactivity. Other components require authorization before protected actions, such as submitting a delay for an assigned trip or viewing a booked shuttle's location. |

## Advantages
- Clear responsibilities make the system easier to understand, maintain, and divide among team members.
- Layers and interfaces support separate testing of screens, business rules, and data access.
- Central access checks give components a consistent way to enforce role and session restrictions.
- Storage or user-interface changes can be contained behind stable interfaces.

## Potential limitations
- Requests may pass through several layers, adding some processing overhead.
- Shared database or application failures can affect several components.
- In a single deployment, patching one component may still require restarting the application. Modularity alone does not guarantee the NFR-20 downtime target; deployment and recovery procedures must also support it.
- Layer boundaries and interfaces must be maintained to prevent tightly coupled code and circular dependencies.
