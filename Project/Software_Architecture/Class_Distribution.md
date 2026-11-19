| Class | Primary component | Reason for Assignment |
| :--- | :--- | :--- |
| UserAccount | CO1: User and Access | Stores credentials and role, tracks failed login attempts, locks the account after 5 failed tries, and supports account suspension. |
| UserSession | CO1: User and Access | Manages active sessions, ends them after 30 minutes of inactivity, and handles secure logout. |
| SystemErrorLog | CO1: User and Access | Records system errors and failed login attempts for IT review. |
| Student | CO1: User and Access | It is the subclass of UserAccount and represents the student role. It inherits login and access control. |
| Driver | CO1: User and Access | It is the subclass of UserAccount and represents the driver role. Also inherits the login and access control. |
| TransportAdmin | CO1: User and Access | It is the subclass of UserAccount representing the transport admin role. Also inherits the login and access control. |
| ITAdministrator | CO1: User and Access | It is the subclass of UserAccount representing the IT staff role that views the system error logs. |
| Shuttle | CO2: Shuttle and Route | Stores and manages shuttle information, including shuttle ID, license plate, capacity and status. |
| Route | CO2: Shuttle and Route | Manages route information, including route ID, origin, destination and description. |
| ScheduledTrip | CO2: Shuttle and Route | Represents a scheduled shuttle trip and manages its associated shuttle, route, driver assignment, departure time, arrival time and trip status. |
| Reservation | CO3: Reservation & No-Show Management | Manages booking, seat allocation and status rules. |
| NoShowReport | CO3: Reservation & No-Show Management | Abstract class that stores information about a no-show report and allows the transport admin to suspend the reported user or dismiss the report. |
| DriverNoShowReport | CO3: Reservation & No-Show Management | No-show report submitted by a student when the driver does not turn up. |
| StudentNoShowReport | CO3: Reservation & No-Show Management | No-show report submitted by a driver when the student does not turn up. |
| LocationUpdate | CO4: Tracking and Notification | Represents a trip's location sample and validates its latitude, longitude, and timestamp. |
| DelayReport | CO4: Tracking and Notification | Represents the reported delay and validates its duration and revised expected arrival. |
| Notification (abstract) | CO4: Tracking and Notification | Contains shared notification information and the send() and renderMessage() operations. |
| DelayNotification | CO4: Tracking and Notification | Specializes Notification to produce a delay message. |
| TripChangeNotification | CO4: Tracking and Notification | Specializes Notification to describe a changed departure time, route, or stop. |