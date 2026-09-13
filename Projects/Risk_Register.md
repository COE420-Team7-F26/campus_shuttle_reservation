# Project Risk Register

## Project

Campus Shuttle Reservation System

The following risk register identifies potential risks that may affect the development and successful completion of the Campus Shuttle Reservation System.

| Risk ID | Risk Description | Possible Cause | Probability | Impact | Mitigation/Response Strategy |
|---|---|---|---|---|---|
| R1 | The project requirements may change or remain unclear during development. | Team members or intended users may have different expectations about reservation rules, routes, schedules, and cancellation procedures. | Medium | High | The team will document and review the requirements before implementation. New requirements will be evaluated before being added to prevent uncontrolled changes to the project scope. |
| R2 | The team may experience difficulty implementing some technical features. | The system may require unfamiliar technologies for authentication, reservation management, databases, or the user interface. | Medium | High | The team will research the required technologies early, divide tasks according to member skills, create small prototypes, and request guidance when necessary. |
| R3 | A team member may be unavailable or unable to complete an assigned task on time. | Illness, examinations, conflicting deadlines, or personal commitments may affect team-member availability. | Medium | High | Tasks will be assigned early and tracked through GitHub. Members will provide progress updates, document their work, and reassign delayed tasks when necessary. |
| R4 | Integration problems may occur when combining work completed by different team members. | Members may modify the same files, use inconsistent formats, or develop components that do not interact correctly. | Medium | High | The team will use separate branches when appropriate, follow consistent naming conventions, commit frequently, review changes before merging, and test components after integration. |
| R5 | The project may fall behind schedule. | The team may underestimate task complexity or encounter technical problems and delayed contributions. | Medium | High | The project will be divided into smaller tasks with internal deadlines. The team will monitor progress weekly, prioritize essential features, and reserve time for testing and corrections. |
| R6 | User information or reservation data may be accessed or modified without authorization. | Weak authentication, insufficient validation, insecure data storage, or programming errors may create security and privacy problems. | Low | High | The system will require authentication, validate user input, restrict access according to user roles, avoid storing unnecessary personal information, and test important security controls. |
| R7 | Shuttle schedule or seat-availability information may become inaccurate. | Delayed database updates, simultaneous reservations, cancellations, or incorrect data entry may produce incorrect availability information. | Medium | High | The system will validate reservations before confirmation, immediately update availability after booking or cancellation, prevent bookings beyond shuttle capacity, and test simultaneous reservation scenarios. |

## Risk Monitoring

The team will review this risk register regularly throughout the project. The probability and impact of each risk will be updated when project conditions change. High-impact risks will receive priority, and mitigation strategies will be adjusted when necessary.
