# Sprint 1 Review

## Sprint Goal Outcome

Partially met. The core sprint goal — enabling authenticated users to search for available conference rooms and make a basic booking — was achieved. US-01 through US-05 were completed and demonstrated in the staging environment. US-06 (Booking Confirmation Email) was deferred due to SendGrid credentials not being provisioned until Day 9, leaving insufficient time for integration testing and acceptance sign-off.

## Completed Work

| Story # | Acceptance Criteria Met |
|---------|------------------------|
| US-01 — User Login & Authentication | Yes — JWT login/logout/refresh working; protected routes return 401 without a valid token |
| US-02 — View List of Available Rooms | Yes — authenticated users see a paginated room list showing name, capacity, and amenities |
| US-03 — Filter Rooms by Capacity and Amenities | Yes — filters applied via URL params; state persists on page refresh |
| US-04 — View Room Details Page | Yes — detail view shows full room info and routes correctly from the list |
| US-05 — Make a Room Booking | Yes — users can select date and time slot and confirm a booking; conflict check prevents double-booking |

## Incomplete Work

| Story # | Reason | Next Action |
|---------|--------|-------------|
| US-06 — Receive Booking Confirmation Email | SendGrid credentials provisioned too late (Day 9) to complete integration testing within the sprint | Carry over to Sprint 2; mock implementation already in place, reducing remaining estimate to ~2 pts |

## Sprint Metrics

Planned points: 21
Completed points: 13
Actual velocity: 21