# Sprint 1 Planning Session

Date[13 May 2026]
Sprint Goal : Enable verified users to search for available conference rooms and make a booking.


## Attendees
- Product Owner: Skye
- Scrum Master: X-Man
- Development Team: Khauhelo (Backend) , Tebello (Frontend) , Alika (Full-stack) and Sandiso (QA)


## Velocity Target
- 21 Story Points

## Selected User Stories 
Story #1: Basic Room Booking |I want to book a conference room for a specific date and time |  

Story #2: Recurring Meetings Setup| I want to set up recurring bookings | 

Story #3: Room Capacity Filtering | I want to filter available rooms by capacity (number of attendees) |

Story #4: Booking Cancellation | I want to cancel my room booking with a single click |

Story #5: Room Equipment Requirements | I want to specify required equipment when booking | 

Story #6: Admin Dashboard Viewing | I want to view a dashboard showing all current and upcoming bookings across all rooms |


## Dependencies   

Story #2 to Story #6 Depends on Story #1 to be excecuted(authentication must be in place before room browsing)


## Risks

## Blocks of code


| Risk                                                                 | Probability | Impact | Mitigation                                                                                                  |
| -------------------------------------------------------------------- | :---------: | :----: | ----------------------------------------------------------------------------------------------------------- |
| Double-booking conflicts caused by simultaneous booking requests     |     High    |  High  | Implement real-time availability checks and database locking mechanisms to prevent overlapping reservations |
| Integration issues with Outlook/Google Calendar APIs                 |    Medium   |  High  | Use tested API libraries, create fallback sync retries, and perform integration testing early               |
| Timezone and daylight saving time inconsistencies affecting bookings |    Medium   |  High  | Store all booking data in UTC and convert to local timezone on display using reliable timezone libraries    |

## Standup Cadence
Time: 09:15 daily (15 minutes maximum)
Format: Yesterday / Today / Blockers
