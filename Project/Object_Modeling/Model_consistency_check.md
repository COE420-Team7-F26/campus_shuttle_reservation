# Class Model Consistency Check

Every use case (UC-01 to UC-21) maps to at least one class and method.  


 DFD data stores:
  - D1 User Accounts--> UserAccount, UserSession
  - D2 Shuttle Information --> Shuttle, Route, ScheduledTrip, LocationUpdate, DelayReport
  - D3 Reservations/ No-shows--> Reservation, NoShowReport and its subclasses


Regarding relationships, every association was checked for a name and multiplicities.  