## Story #2: Recurring Meetings Setup

 
As an Employee
I want to set up a recurring room booking (daily, weekly, or custom cadence)
So that I do not have to manually re-book the same room for regular team meetings


### Acceptance Criteria:
- Given I am creating a booking, When I enable the recurrence option and select a frequency (daily / weekly / monthly), Then the system creates individual bookings for all occurrences within the defined date range

- Given a recurring series is active, When one occurrence conflicts with an existing booking, Then the system flags that date and asks me whether to skip or cancel the series

- Given I have a recurring booking, When I cancel a single occurrence, Then only that occurrence is removed and the rest of the series remains intact

### Story Points:
8
 
### Priority:
Medium
 
### Dependencies:
 Story #2: Recurring Meetings Setup

### Technical Notes:
- Recurring bookings should be stored as a series with a shared parent ID so edits can cascade
- Maximum recurrence horizon should be configurable (e.g., 12 months)
- Conflict detection must run across all proposed dates before the series is saved

### Design Notes:
- Recurrence options should appear as an expandable section to keep the base booking form clean
- Show a calendar preview of all upcoming occurrences before confirmation
- Include an "end date" or "number of occurrences" toggle


## Story #6: Admin Dashboard Viewing
 
As an Admin

I want to view a centralised dashboard showing all current, upcoming, and past bookings across all rooms
So that I can monitor room utilisation and manage the booking system effectively

### Acceptance Criteria:
- Given I am logged in as Admin, When I navigate to the dashboard, Then I see a live overview of all rooms with their current status (available, booked, under maintenance)

- Given the dashboard is displayed, When I apply filters by date range, room, or user, Then the booking list updates to show only matching records

- Given a booking entry is shown, When I click on it, Then I can view the full booking details including the organiser, attendees, and purpose

### Story Points:
5
 
### Priority:
High
 
### Dependencies:
- Story #6: Admin Dashboard Viewing

### Technical Notes:
- Dashboard data should auto-refresh at a configurable interval (default: every 60 seconds)
- Admin role must be enforced server-side; the dashboard route should return 403 for non-admin users
### Design Notes:
- Use a colour-coded room grid (e.g., green = available, red = booked, grey = maintenance) for at-a-glance status
- Filters should persist across page refreshes using query parameters