The models were integrated by combining the individual models in a shared draw.io file. 

Duplicate classes resolved
- Reservation (M, R) were merged into one class with shared attributes and methods.
- Schedule (R) and Trip (S) were merged and renamed to ScheduledTrip.
- login()/logout() were in several user classes, so we moved them to UserAccount.

We have changed the class name ITAdminstrator to be singular, and made changes to lab 3 (add UC-21)

The data types were standardized (String IDs, boolean, int)
