# User Stories — Conference Room Booking System


## Story #1: Basic Room Booking

As an Employee
I want to search for and book an available conference room for a specific number of people , date and time
So that I can secure a meeting space in advance and avoid conflicts with other bookings

## Story Points:
5
## Priority:
High
## Dependencies:
1

## Technical Notes:

Room availability must be queried in real time against the bookings database
Booking confirmation should trigger an email and/or in-app notification
Assume single-room booking per form submission; no bulk booking in this story

Design Notes:

Date/time picker should default to the next available business-hour slot
Available rooms should display room name, floor, and capacity at a glance
Confirmation screen should show a summary before final submission


## Story #3: Room Capacity Filtering

As an Employee
I want to filter available rooms by minimum seating capacity
So that I can find a room that comfortably accommodates all my meeting attendees and to meet certain specification. 

### Acceptance Criteria:
- Given filtered results are shown, When I hover or tap a room  card, Then I can see the exact stated capacity of that room
- Given I am logged in, When I select a date, start time and end time, Then I see a list of available rooms for that slot
- Given I have selected a room, When I confirm the booking, Then the room is reserved under my name and I receive a confirmation notification
- Given a room is already booked for the selected time, When I view availability, Then that room does not appear in the results

### Story Points:
3

### Priority:
High

### Dependencies:
3 

### Technical Notes:
- Room availability must be queried in real time against the bookings database
- Booking confirmation should trigger an email and/or in-app notification
- Assume single-room booking per form submission; no bulk booking in this story

### Design Notes:
- Capacity filter can be a simple number input or a slider (≤ 20 people)
- Rooms near the capacity limit
- Date/time picker should default to the next available business-hour slot
- Available rooms should display room name, floor, and capacity at a glance
- Confirmation screen should show a summary before final submission

### Story #4: Booking Cancellation
As a Employee
I want to cancel a room booking I have made
So that the room becomes available to other colleagues when I no longer need it
Acceptance Criteria:

- Given I have an upcoming booking, When I navigate to "My Bookings" and select cancel, Then the booking is removed and the room slot becomes immediately 
available

- Given a cancellation is confirmed, When the action is processed, Then all attendees who were invited receive a cancellation notification

- Given the booking starts within 30 minutes, When I attempt to cancel, Then the system displays a late-cancellation warning before proceeding.

### Story Points:
3
### Priority:
High
### Dependencies:

Story #4: Booking Cancellation

### Technical Notes:

Cancellations should be soft-deleted (retained in the database) for audit and reporting purposes
Business rules around late cancellations (e.g., locking cancellation within 15 minutes) should be configurable by admin

### Design Notes:

Cancellation option should be clearly visible on the "My Bookings" view but require a confirmation step to prevent accidental cancellations
Show reason-for-cancellation field (optional) to help facilities managers understand patterns