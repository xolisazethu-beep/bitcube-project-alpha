# Prioritisation Matrix — Conference Room Booking System



## Priority Matrix

| Story # | Title | Business Value | Technical Complexity | Priority | Sprint |
|--------:|-------|----------------|----------------------|----------|--------|
| 1 | Basic Room Booking | High | Medium | High | 1 |
| 3 | Room Capacity Filtering | High | Low | High | 1 |
| 4 | Booking Cancellation | High | Low | High | 1 |
| 6 | Admin Dashboard Viewing | High | Medium | High | 2 |
| 9 | Booking Conflict Resolution | High | High | High | 2 |
| 5 | Room Equipment Requirements | Medium | Low | Medium | 2 |
| 2 | Recurring Meetings Setup | Medium | High | Medium | 3 |
| 7 | Room Maintenance Scheduling | Medium | Medium | Medium | 3 |
| 8 | Visitor Booking Assistance | Medium | Medium | Medium | 3 |
| 10 | Usage Reports Generation | Medium | High | Medium | 4 |


## Prioritisation Rationale

Sprint 1 — Foundation (Stories #1, #3, #4)
These three stories represent the minimum viable product. Without the ability to book, filterand cancel rooms, the system has no value. They are high business value and relatively low-to-medium complexity, making them ideal sprint-opener stories that can be shipped quickly to validate the core workflow.

Sprint 2 — Operational Integrity (Stories #6, #9, #5)**  
Once bookings exist, the admin needs visibility (Story #6) and the system must protect itself against conflicts (Story #9). Equipment filtering (Story #5) is included here as it extends the already-built search flow with minimal additional complexity and increases daily usability.

Sprint 3 — Extended Workflows (Stories #2, #7, #8)**  
Recurring meetings, maintenance scheduling, and visitor bookings are important but not blockers to the core experience. Each extends an existing workflow rather than creating a new one, so they are best tackled after the foundation is stable.

Sprint 4 — Analytics (Story #10)**  
Usage reports require clean, accumulated booking data to be meaningful. They deliver business intelligence rather than operational capability, so they are best delivered once the system has been running for at least a sprint cycle.

---

## Extra Credit — Velocity & Sprint Estimation

### Total Story Points

| Story # | Points |
|--------:|--------|
| 1 | 5 |
| 2 | 8 |
| 3 | 3 |
| 4 | 3 |
| 5 | 3 |
| 6 | 5 |
| 7 | 5 |
| 8 | 5 |
| 9 | 8 |
| 10 | 8 |
|Total| 53 |



### Proposed Team Velocity

Assumed team composition: 2 developers, 1 QA engineer, 1 part-time tech lead  
Sprint length: 2 weeks  
Proposed velocity: 13–15 story points per sprint

Reasoning:

A team of this size is realistic for an internal office tooling project. A velocity of 13–15 points per sprint accounts for:

- ~20% overhead per sprint for ceremonies (planning, review, retro, standups)
- ~10% allocation for bug fixes and technical debt as the system matures
- Ramp-up effect: Sprint 1 velocity may be closer to 11 points as the team establishes conventions and dev environment; later sprints should reach 15 points once patterns are established

At a mid-range velocity of **13 points per sprint**:

| Sprint | Stories | Points |
|--------|---------|--------|
| 1 | #1, #3, #4 | 11 |
| 2 | #6, #5, #9 (partial) | 12 |
| 3 | #9 (remainder), #2 (partial), #7 | 13 |
| 4 | #2 (remainder), #8, #10 (partial) | 13 |
| 5 | #10 (remainder) + buffer/polish | 8 + buffer |

Estimated delivery: 4–5 sprints (8–10 weeks)

The slight imbalance in sprint 1 (11 points) is intentional — it allows the team breathing room to set up infrastructure, CI/CD pipelines and database schemas without underdelivering on feature stories. Sprint 5 absorbs any overflow, final integration testing, and UX polish ahead of release.
