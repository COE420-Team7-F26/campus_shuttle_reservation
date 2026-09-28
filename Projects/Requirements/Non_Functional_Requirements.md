| **NFR ID** | **Category** | **Non-Functional Requirement** | **Contributor** |
|---|---|---|---|
| NFR-01 | Performance | The system shall display the current shuttle occupancy within 3 seconds of a student’s request | Rana |
| NFR-02 | Usability | The system shall display each shuttle's schedule and availability information on a single screen, including the shuttle route, departure time, and number of available seats. | Rana |
| NFR-03 | Reliability | The system shall update shuttle seat availability within 5 seconds when a reservation is made or cancelled | Rana |
| NFR-04 | Portability | The system shall be accessible on Android 11 or later and iOS 15 or later on smartphones and tablets. | Rana |
| NFR-05 | Security | The system shall require authentication and shall display only the functions and interface options permitted to their assigned role, such as student, driver, or transport admin | Rana |
| NFR-06 | Ease of Use | After 15 minutes of training, a student shall be able to book a seat on a trip within 2 minutes starting from opening the app to getting the confirmation message | Meera |
| NFR-07 | Robustness | If the app crashes the system shall allow the user to reopen it and use it within 30 seconds after the crash | Meera |
| NFR-08 | Reliability | The app shall successfully show a confirmation message for the booked seat for at least 99% of booking attempts | Meera |
| NFR-09 | Reliability | The app shall be available for the students to access for at least 97% of the shuttle’s daily operating hours | Meera |
| NFR-10 | Ease of Use | After 30 minutes of training the transport administrator shall be able to review at least 10 no-show reports in an hour | Meera |
| NFR-11 | Performance | The app shall send notifications about reported delays, timetable changes, and route or stop location changes to affected students within 5 seconds after the update is recorded. | Serly |
| NFR-12 | Location Accuracy | During an active trip, the app shall refresh the shuttle’s device based location at least once every 10 seconds and display a location accurate to within 25 metres under normal GPS conditions. | Serly |
| NFR-13 | Security | The app shall require users to log in before accessing reservation, account, or live shuttle-location information. After five unsuccessful login attempts, access shall be temporarily blocked for 10 minutes. | Serly |
| NFR-14 | Scalability | The system shall support at least 500 users accessing shuttle schedules, occupancy information, and reservations simultaneously while maintaining a response time of no more than 3 seconds for at least 95% of requests. | Serly |
| NFR-15 | Privacy | The app shall stop collecting and sharing the driver’s device location within 30 seconds after the assigned shuttle trip is marked as completed. | Serly |
| NFR-16 | Portability | The application shall install and execute without graphical errors on both iOS (version 15 and above) and Android (version 11 and above) operating systems | Yusr |
| NFR-17 | reliability | In the event of a network disconnection, the driver application shall locally cache "no-show" reports and automatically synchronize them with the server once the connection is restored | Yusr |
| NFR-18 | security | The system shall automatically terminate user sessions and require re-authentication after 30 minutes of inactivity, excluding drivers who are actively operating a scheduled trip. | Yusr |
| NFR-19 | usability | 100% of the messages would be clear, context-specific error messages in plain text (e.g., "This shuttle is currently at maximum capacity") . I will not be displaying raw technical error codes to students and drivers | Yusr |
| NFR-20 | availability | The system architecture shall allow the IT department to apply minor software updates and patches with a maximum of 60 minutes of scheduled downtime per month, minimizing disruption to end users | Yusr |
