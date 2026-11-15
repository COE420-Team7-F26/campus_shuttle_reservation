# Exercise 4: Interfaces — Tracking and Notification

The editable diagram and PDF show CO4's provided interfaces as lollipops and required interfaces as sockets. The interface classifiers list typed operations. This is an individual component fragment to merge into the team's complete four-component diagram.

## Provided interfaces
### ITrackingNotification
- validateLocation(update: LocationUpdate): Boolean
- validateDelay(report: DelayReport): Boolean
- sendNotification(notification: Notification): Boolean
- renderNotification(notification: Notification): String

These operations delegate respectively to LocationUpdate.isValid(), DelayReport.isValid(), Notification.send(), and Notification.renderMessage(). The last operation dispatches to the appropriate DelayNotification or TripChangeNotification implementation. Thus the interface exposes existing class behavior through parameterized component-level operations.

## Required interfaces
### IAccessControl — provided by User and Access
- authorize(sessionId: String, action: String, tripId: String): Boolean

### ITripContext — provided by Shuttle and Route
- getTrip(tripId: String): ScheduledTrip
- isAssignedDriver(tripId: String, driverId: String): Boolean

### IReservationLookup — provided by Reservation and No-Show
- getActiveReservations(tripId: String): List<Reservation>

The three required contracts are architectural proposals for the owning teammates to incorporate into their interfaces; their names and signatures are not claimed to be verbatim Lab 5 methods. List<Reservation> denotes a collection of Reservation objects. Retrieval failures must be handled by the implementing component before notifications are sent.

## Collaboration for UC16
1. Check the driver's session and authorization through IAccessControl.
2. Obtain the trip and verify that the driver is assigned through ITripContext.
3. Validate the DelayReport; reject invalid input before sending notifications.
4. Obtain active reservations for the affected trip through IReservationLookup.
5. Create a DelayNotification for each recipient and call sendNotification(). Check its Boolean delivery result; do not mark a failed send as successful.

The caller/orchestrating workflow supplies the trip and report context. Notification subclasses determine message content. These contracts support the Lab 6 delay-reporting interaction without moving ScheduledTrip or Reservation into CO4.
