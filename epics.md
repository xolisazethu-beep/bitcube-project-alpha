 #Epic Breakdown — Conference Room Booking System



# Epic: Conference Room Booking System

## Epic 1: Core Booking Experience

> Covers the fundamental ability for employees to find and reserve rooms, the foundation on which all other functionality depends.

- Story #1: Basic Room Booking
- Story #2: Recurring Meetings Setup
- Story #3: Room Capacity Filtering
- Story #4: Booking Cancellation
- Story #5: Room Equipment Requirements


## Epic 2: Administration & Oversight

> Covers the tools that admins need to monitor the system, maintain data integrity, and enforce business rules across all bookings.

- Story #6: Admin Dashboard Viewing
- Story #9: Booking Conflict Resolution
- Story #10: Usage Reports Generation


## Epic 3: Facilities & Space Management

> Covers the operational needs of the Facilities Manager role, specifically the ability to take rooms out of service for maintenance without disrupting the broader booking flow.

- Story #7: Room Maintenance Scheduling


## Epic 4: Visitor & Guest Services

> Covers the front-desk workflow that allows Receptionists to act as booking proxies for external guests who cannot access the internal system.

- Story #8: Visitor Booking Assistance


## Epic Dependency Map

```
Epic 1: Core Booking Experience
  └── Epic 2: Administration & Oversight  (requires booking data to exist)
        └── Epic 3: Facilities & Space Management  (requires admin dashboard)
  └── Epic 4: Visitor & Guest Services  (extends core booking + cancellation)

