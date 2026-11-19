| Class | Primary component | Reason for Assignment |
| :--- | :--- | :--- |
| Student | CO1: User and Access | It is the subclass of UserAccount and represents the student role. It inherits login and access control. |
| Driver | CO1: User and Access | It is the subclass of UserAccount and represents the driver role. Also inherits the login and access control. |
| TransportAdmin | CO1: User and Access | It is the subclass of UserAccount representing the transport admin role. Also inherits the login and access control. |
| ITAdminstrator | CO1: User and Access | It is the subclass of UserAccount representing the IT staff role that views the system error logs. |
| Shuttle | CO2: Shuttle and Route | Stores and manages shuttle information, including shuttle ID, license plate, capacity and status |
| Route | CO2: Shuttle and Route | Manages route information, including route ID, origin, destination and associated stops |
| Schedule | CO2: Shuttle and Route | Represents a scheduled shuttle trip and manages its associated shuttle, route, driver assignment, departure time, arrival time and trip status |
| Reservation | CO3: Reservation & No-Show Management | Manages booking, seat allocation and status rules. |
| NoShowReport | CO3: Reservation & No-Show Management | Abstract class that stores information about reports and allows the transport admin to put bookings on hold or cancel. |
| DriverNoShowReport | CO3: Reservation & No-Show Management | No show report specific to checking if drivers have not turned up. |
| StudentNoShowReport | CO3: Reservation & No-Show Management | No show report specific to checking if students have not turned up. |
| LocationUpdate | CO4: Tracking and Notification | Represents a trip's location sample and validates its latitude, longitude, and timestamp. |
| DelayReport | CO4: Tracking and Notification | Represents the reported delay and validates its duration and revised expected arrival. |
| Notification (abstract) | CO4: Tracking and Notification | Contains shared notification information and the send() and renderMessage() operations. |
| DelayNotification | CO4: Tracking and Notification | Specializes Notification to produce a delay message. |
