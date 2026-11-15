# Exercise 3: Class Distribution — Serly's Component

| Class | Primary component | Reason for assignment |
|---|---|---|
| LocationUpdate | CO4 — Tracking and Notification | Represents a trip's location sample and validates its latitude, longitude, and timestamp. |
| DelayReport | CO4 — Tracking and Notification | Represents the reported delay and validates its duration and revised expected arrival. |
| Notification (abstract) | CO4 — Tracking and Notification | Contains shared notification information and the send() and renderMessage() operations. |
| DelayNotification | CO4 — Tracking and Notification | Specializes Notification to produce a delay message. |
| TripChangeNotification | CO4 — Tracking and Notification | Specializes Notification to describe a changed departure time, route, or stop. |

These five classes are assigned once, to CO4. ScheduledTrip, Reservation, Student, and Driver remain owned by the other relevant components; references to them do not transfer their ownership. This is Serly's portion of the team distribution table.
