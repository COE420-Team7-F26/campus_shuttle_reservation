# Exercise 3: Component Description — Serly's Contribution
Serly Torrosian — G00098361

| Field | Description |
|---|---|
| Component ID | CO4 |
| Component name | Tracking and Notification |
| Responsibilities | Validate and manage location updates, validate driver delay reports, and prepare and send notifications about delays and trip changes. |
| Supported functionality | Live shuttle tracking and location sharing (UC07, UC19, UC20); shuttle delay reporting and notification (UC16); notification of changes to trip time, route, or stop location (UC17, UC18). |
| Included classes | LocationUpdate, DelayReport, Notification, DelayNotification, TripChangeNotification |

LocationUpdate stores latitude, longitude, and the recording time for a trip. Updates originate automatically from the assigned driver's device while sharing is active. DelayReport stores the delay duration and revised expected arrival time. Notification is the abstract parent class for common delivery behavior. DelayNotification and TripChangeNotification specialize the message content.

This component obtains trip and driver-assignment information from Shuttle and Route, active reservations from Reservation and No-Show, and authorization from User and Access. It only notifies students with active reservations on the affected trip. Tracking stops when location sharing ends or the trip is completed.
