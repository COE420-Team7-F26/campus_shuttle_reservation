1. Model selection
The selected software process model for the Campus Shuttle Reservation System is the incremental model.
The system will be developed through a series of functional increments. Each increment will add new features to the existing system and will undergo testing before being integrated into the overall product.

2. Justification
	The Incremental model is appropriate for the Campus Shuttle Reservation system because the requirements are relatively clear and stable. The system has several distinct features that can be developed separately and gradually combined into the complete system.
The main features include:
- viewing shuttle occupancy
- booking a shuttle seat
- cancelling a reservation
- allowing staff to update shuttle information
- sending notifications about delays, timing changes, and location changes
- Booking admin functions such as reviewing no-show reports, suspending accounts with repeated no-shows, and resolving disputes between students and drivers
These features can be divided into different increments. For example, our team can first develop the basic shuttle information and occupancy features, followed by booking and cancellation, and then staff management, notifications and finally the booking admin functions.
This approach allows us to have a working system ready and add more functionality with each increment. Each increment will also be tested before the next features are added, which makes it easier to identify and fix problems.

3. Model overheads
	the main overheads associated with this model are:
- repeated planning: each increment requires planning and organisation
- Integration overhead: new functionality must be integrated with previously developed components
- Re-testing: existing functionality must be retested after new features are introduced
- Documentation overhead: technical and user documentation must be maintained as the system evolves

4. Strategy for managing overheads:
	Our team will manage these overheads through these strategies:
- We will be using a standard planning template for each increment, including requirements, tasks, responsibilities, deadlines, and testing activities. This will make planning much faster and consistent across increments.
- Each team member will follow the agreed system structure and database design when developing their part. Completed components will be integrated regularly rather than combining everything at the end
- The team will identify which existing functions are affected by each new increment and focus re-testing on those areas. A small set of tests for critical functions, such as seat booking, cancellation, and occupancy, will be maintained and reused after relevant changes.
- Documentation will be maintained throughout development. We will be using a shared document and update only the sections affected by each increment to avoid unnecessary duplication

5. Model drawbacks
Although the incremental model is suitable for the project, it has several drawbacks such as
- Integration problems: a new increment might not work properly with an earlier increment
- Dependencies: some features cannot be developed until other features are completed
- Uneven workload: some increments may require much more work than others

6. Strategies for addressing drawbacks:
- Manage integration: The team will agree on the main database structure and system interfaces before development begins. Each completed increment will also be integrated and checked before moving on to the next one.
- Manage dependencies: Dependencies will be identified before assigning increments. The team will develop features in logical order, completing important foundational features before features that depend on them.
- Balance workload: Each increment will be divided into smaller tasks and distributed among team members based on the difficulty and amount of work involved. Progress will be checked regularly so tasks can be reassigned if one member becomes overloaded.
