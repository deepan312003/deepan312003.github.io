# occupancy chart based on availability for CSE
### To generate an occupancy chart for all rooms for CSE, we will need to have the following information:

List of rooms and their capacities
Time table/schedule of events and classes in each room
List of room reservations made by users

Using this information, we can create an occupancy chart that shows the availability of each room at different times. This can be done by creating a table with rows representing each room and columns representing each time slot, and filling in the table with information about which events/classes are scheduled in each room at each time slot. Any room that is not scheduled for an event/class at a particular time slot is considered to be available.

To search for room availability on a particular day/time and reserve the same, users can interact with the occupancy chart through a web application or mobile app. They can select a particular day/time and view which rooms are available for reservation. They can then select the room they want to reserve and make a reservation by providing their personal details and the purpose of the reservation.

User stories for this project can be divided into epics and sub-stories. The epics for this project could be:

Room Management: This epic will include all the stories related to managing the rooms, such as adding new rooms, updating room details, and deleting rooms.
Event Management: This epic will include all the stories related to managing the events and classes scheduled in each room, such as creating new events, updating event details, and deleting events.
Reservation Management: This epic will include all the stories related to managing the room reservations made by users, such as creating new reservations, updating reservation details, and cancelling reservations.
Some example user stories for each epic could be:

#### Room Management:

As a system administrator, I want to be able to add new rooms to the system, so that they can be used for scheduling events and classes.
As a system administrator, I want to be able to update the details of existing rooms, such as their capacity and location, so that they are up-to-date.
As a system administrator, I want to be able to delete rooms that are no longer needed, so that they do not clutter the system.
#### Event Management:

As a teacher, I want to be able to schedule a new class in a particular room at a particular time, so that my students know where and when to attend.
As an event organizer, I want to be able to create a new event in the system and assign it to a particular room at a particular time, so that attendees know where and when to go.
As a system administrator, I want to be able to delete events that have been cancelled or are no longer needed, so that they do not clutter the system.
Reservation Management:

As a user, I want to be able to search for available rooms on a particular day and time, so that I can reserve a room for my event.
As a user, I want to be able to reserve a room for a particular day and time, and provide details about the purpose of the reservation, so that I can use the room for my event.
As a user, I want to be able to cancel my reservation if I no longer need the room, so that it becomes available for others to use.
For a sprint 0 chart, we could have the following tasks and user types:

#### Tasks:

Set up the database and data models for rooms, events, and reservations
Create a basic occupancy chart UI for viewing room availability
Implement room management functionality, including adding, updating, and deleting rooms
Implement event management functionality, including creating, updating, and deleting events
Implement reservation management functionality, including searching for available rooms and making reservations





| Epic | User Story | Sub-Story | Task | Plan to Work | User Types |
| --- | --- | --- | --- | --- | --- |
| Time Table Management | Manage Time Table | Define Time Table Format | Define fields and data types for time table\nIdentify stakeholders and gather requirements for time table format | Team Lead, Faculty, Admin |
|  |  | Create Time Table | Develop code to create time table based on stakeholder requirements\nValidate time table data for accuracy and completeness | Team Lead, Admin |
|  |  | Update Time Table | Define user interface for updating time table\nDevelop code to update time table based on user input\nValidate user input for date, time, and room availability | Faculty, Admin |
| Room Management | Manage Rooms | Define Room Types | Define different types of rooms (e.g. classroom, lab, conference room)\nIdentify requirements for each room type (e.g. size, equipment)\nDocument room type specifications | Team Lead, Admin |
|  |  | Create Rooms | Develop code to create rooms based on room type specifications\nValidate room data for accuracy and completeness | Team Lead, Admin |
|  |  | Update Rooms | Define user interface for updating room information\nDevelop code to update room information based on user input\nValidate user input for room type, size, and equipment | Admin |
| Occupancy Chart Generation | Generate Occupancy Chart | Retrieve Time Table | Define time table format\nIdentify data source for time table (e.g. database, API, manual input)\nDevelop code to retrieve time table data from data source | Team Lead, Admin |
|  |  | Calculate Room Occupancy Status | Define room occupancy statuses (e.g. "Available", "In Use", "Unavailable")\nDevelop algorithm to calculate room occupancy status based on time table data\nTest algorithm with sample time table data | Team Lead, Admin |
|  |  | Display Occupancy Chart | Define user interface for displaying occupancy chart\nDevelop code to display occupancy chart\nIntegrate occupancy chart data with user interface | Faculty, Admin |
| Room Availability Check | Check Room Availability | Search for Room Availability | Define search criteria (e.g. date, time, room capacity)\nDevelop code to search for room availability based on search criteria\nTest search functionality with sample data | Faculty, Student |
|  |  | Display Room Availability | Define user interface for displaying room availability\nDevelop code to display available rooms based on search results\nIntegrate room availability data with user interface | Faculty, Student |
| Room Reservation | Reserve a Room | Reserve a Room | Define user interface for reserving a room\nDevelop code to reserve a room based on user input\nValidate user input for date, time, and room availability\nIntegrate reservation data with occupancy chart | Faculty |
|  |  | Cancel Room Reservation | Define user interface for canceling a room reservation\nDevelop code to cancel a room reservation based on user input\nIntegrate cancellation data with occupancy chart | Faculty |
|  |  | Edit Room Reservation | Define user interface for editing a room reservation\nDevelop code to edit a room reservation based on user input\nValidate user input for date, time, and room availability\nIntegrate edit data with occupancy chart | Faculty |
|  | Manage Room Reservations | View Room Reservations | Define user interface for viewing room reservations\nDevelop code to retrieve and display room reservation data\nIntegrate reservation data with occupancy chart | Admin |
|  |  | Manage Room Reservation Requests | Define user interface for managing room reservation requests\nDevelop code to approve or deny room reservation requests based on room availability and other criteria\nIntegrate reservation request data with
