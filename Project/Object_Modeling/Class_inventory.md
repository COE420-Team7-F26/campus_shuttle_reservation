

| Class name | attributions | methods | changes |
| :---- | :---- | :---- | :---- |
| **UserAccount** | **\-userId: String, \-username: String, \-passwordHash: String, \-role: String, \-failedLoginAttempts: int, \-isLocked: boolean, \-lockoutEndTime: DateTime** | **\+login(): boolean, \+logout(): void, \+lockAccount(): void, \-incrementFailedAttempts(): void** | **\> fixed spelling  \> made class into a superclass for all actors \> added userID and logout() method** |
| **UserSession** | **\-sessionId: String, \-lastActivityTime: DateTime, \-sessionStatus: String** | **\+autoTerminateSession(): boolean, \+updateActivityTime(): void, \+secureLogout(): void** | **\> fixed spelling** |
| **Student** | **\-studentId: String, \-name: String, \-email: String, \-phone: String** | **\+bookSeat(trip: ScheduledTrip, seatNumber: String): boolean, \+cancelSeat(reservationId: String): boolean, \+viewBookingDetails(): List\~Reservation\~, \+trackBookedTrip(trip: ScheduledTrip): LocationUpdate** | **\> merged class from Rana’s and Serly’s diagrams \> added bookSeat() and cancelSeat() methods \> updated parameter in trackBookedTrip.**  |
| **Driver**  | **\-driverId: String, \-name: String, \-phone: String** | **\+startTrip(trip: ScheduledTrip): void, \+completeTrip(trip: ScheduledTrip): void** | **\> now it inherits from UserAccount superclass** |
| **TransportAdmin**  | **\-adminId: String, \-name: String, \-email: String** | **\+updateShuttleInfo(shuttle: Shuttle): void, \+updateRoute(route: Route): void, \+updateSchedule(schedule: ScheduledTrip): void** | **\> now it inherits from UserAccount superclass \> removed phone attribute \> updated aupdateSchedule method paramater** |
| **ITAdministrator**  | **\-adminId: String** | **\+viewSystemErrorLogs(): List\~SystemErrorLog\~** | **\> renamed the class \> now it inherits from UserAccount superclass** |
| **Shuttle**  | **\-shuttleId: String, \-licensePlate: String, \-capacity: int, \-status: String** | **\+updateDetails(): void, \+setStatus(status: String): void, \+getCurrentLocation(): String** | **\> shuttleId is now a string** |
| **Route**  | **\-routeId: String, \-origin: String, \-destination: String, \-description: String** | **\+updateRoute(): void, \+getRouteDetails(): String** | **\> routeID is now a string** |
| **ScheduledTrip**  | **\-tripId: String, \-departureTime: DateTime, \-arrivalTime: DateTime, \-date: Date, \-status: String, \-sharingActive: boolean** | **\+start(): boolean, \+complete(): boolean, \+stopSharing(): void, \+updateSchedule(): void, \+getScheduleDetails(): String** | **\> merged classes from Rana’s and Serly’s diagrams and combined methods \> removed the driver parameter from start() and complete() methods, now its mapped via association line** |
| **Reservation**  | **\-reservationId: String, \-seatNumber: String, \-bookingTime: DateTime, \-status: String, \-notes: String** | **\+cancel(): boolean, \-canCancel(currentTime: DateTime): boolean, \+isActive(): boolean, \+getBookingDetails(): String, \+updateStatus(status: String): void** | **\> combined from Meera’s and Rana’s diagrams and combined core methods \> removed bookingDate method from Rana’s diagram as its abundant** |
| **LocationUpdate**  | **\-updateId: String, \-latitude: Double, \-longitude: Double, \-recordedAt: DateTime** | **\+isValid(): Boolean** | **\> no changes** |
| **NoShowReport**  | **\-reportId: String, \-reportTime: DateTime, \-decision: String** | **\+suspendReportedUser(admin: TransportAdmin): void, \+dismiss(admin: TransportAdmin): void, \+getDecision(): String, \#isWithinReportWindow(currentTime: DateTime): boolean** | **\> reportID is now a string** |
| **DriverNoShowReport**  |  | **\+isValidDriverReport(currentTime: DateTime): boolean** |  |
| **StudentNoShowReport**  |  | **\+isValidStudentReport(): boolean** |  |
| **DelayReport**  | **\-reportId: String, \-delayMinutes: int, \-expectedArrival: DateTime, \-reportedAt: DateTime** | **\+isValid(): Boolean** |  |
| **SystemErrorLog**  | **\-logId: String, \-timestamp: DateTime, \-errorType: String, \-description: String** | **\+recordLog(): void, \+getLogDetails(): String** |  |
| **Notification**  | **\-notificationId: String, \-createdAt: DateTime, \-deliveryStatus: String** | **\+send(): boolean, \+renderMessage(): String\*** |  |
| **DelayNotification**  | **\-reason: String** | **\+renderMessage(): String** |  |
| **TripChangeNotification**  | **\-changeType: String, \-oldValue: String, \-newValue: String** | **\+renderMessage(): String** |  |

