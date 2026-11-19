DG01: Modularity

Related classes stay together in one component. Interface contracts reduce the effect of internal changes on other components. A change to notification message formatting, for example, does not require changes to seat-booking rules. This supports incremental development and maintainability.




DG02: Security

User and Access centrally handles credentials, role checks, account lockout after five unsuccessful login attempts, and session expiration after 30 minutes of inactivity. Other components require authorization before protected actions, such as submitting a delay for an assigned trip or viewing a booked shuttle's location.

