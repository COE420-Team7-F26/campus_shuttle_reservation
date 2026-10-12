| **UC ID** | **Use Case Name** | **Primary Actor** | **Short Description** | **Contributor** |
|---|---|---|---|---|
| UC-01 | Mark driver as no-show | Student | If the shuttle trip time has arrived and the driver did not show up or report that there would be a delay, the student can mark them as no-show | Meera |
| UC-02 | Mark student as no-show | Shuttle Driver | If the shuttle trip time has arrived and the student with active booking did not appear at the pickup point, the driver can mark them as no-show | Meera |
| UC-03 | Cancel seat reservation | Student | A student can cancel their seat reservation on a shuttle if there are more than 10 minutes left before the shuttle’s scheduled departure. Within 5 seconds the seat becomes available to other students. | Meera |
| UC-04 | Late Cancellation | Student | An error message appears when a student tries to cancel their shuttle booking if there are 10 minutes or less left until the shuttle departs | Meera |
| UC-05 | Review no-show reports | Transport Admin | The transport admin reviews no-show reports and can either suspend the account of the the person reported or dismiss the no-show report | Meera |
| UC-06 | Update Shuttle information | Transport Admin | The transport admin sets or updates basic shuttle information such as schedules, routes and shuttle shuttle details before the trip | Rana |
| UC-07 | Track booked shuttle | Student | A student tracks the location of their booked shuttle in real time while waiting for the shuttle | Rana |
| UC-08 | View shuttle schedule | Student | A student views the available shuttle routes and scheduled departure times before choosing a shuttle | Rana |
| UC-09 | View booking details | Student | Student views the shuttle, route, departure time and seat associated with their reservation | Rana |
| UC-10 | Log in | Student/ Driver/ Transport Admin | A user enters their credentials to access the system, and the system grants access to the interface and functions associated with their assigned role | Rana |
| UC-11 | View system error logs | IT administrator | IT staff access internal secured database to investigate application errors, crashes, failed login attempts for maintenance purposes. | Yusr |
| UC-12 | Viewing vehicle details | Student | A student with a reservation logs into the application to view specific details about a vehicle including the license plate or the color | Yusr |
| UC-13 | Auto-terminate session | Transport admin/Student | The application closes the session and forces a user to sign back in after 30 minutes of inactivity | Yusr |
| UC-14 | Lock user account | Student | The system will temporarily lock the user out for 10 minutes after 5 unsuccessful login attempts. | Yusr |
| UC-15 | Secure driver logout | Driver | The driver initiates a secure logout that instantly terminates all background processes storing session data and tracking location | Yusr |
| UC-16 | report shuttle delay | shuttle driver | The driver selects the assigned trip and reports a delay with a revised expected arrival time. The system records the update and alerts students who reserved that trip. | serly |
| UC-17 | change trip departure | transport admin | The administrator selects a scheduled trip and changes its departure time. The system saves the new time and alerts students with reservations on that trip. | serly |
| UC-18 | change trip route or stop | transport admin | The administrator selects a scheduled trip and changes its departure time. The system saves the new time and alerts students with reservations on that trip. | serly |
| UC-19 | start location sharing for assigned trip | shuttle driver | The driver opens the assigned trip and starts it. During the active trip, the system receives the driver device location for students tracking their reserved shuttle. | serly |
| UC-20 | complete assigned trip | shuttle driver | The driver marks the assigned trip complete after arriving. The system closes the trip and stops collecting and sharing that trip’s driver location. | serly |
