## Day 1 — Tuesday, 13-05-2026

### Khauhelo (Backend)

Yesterday: Sprint planning, reviewed architecture with team, set up local PostgreSQL instance
Today: Draft database ERD for bookings, rooms, and users tables; begin API contract design
Blockers: None

### Tebello (Frontend)

Yesterday: Sprint planning, cloned design system repo, audited existing Figma components
Today: Map out booking form wireframes; identify 3 missing components needed (date-time picker, room card, capacity badge)
Blockers: None

### Alika (Full-stack)

Yesterday: Sprint planning, researched Azure AD OAuth2 flow for corporate SSO
Today: Spike Azure AD integration; build minimal auth prototype
Blockers: None

### Sandiso (QA)

Yesterday: Sprint planning, reviewed acceptance criteria for all 5 committed stories
Today: Set up Cypress test project; write API contract test stubs for Story #1 endpoints
Blockers: QA environment not ready yet (ticket #INF-042 pending); working locally for now

### X-Man (Scrun Master)

Notes: Team energy is high. Reminded everyone to update Asana board before standup. Sandiso’s blocker flagged for follow-up.
Action: Escalate QA environment ticket with DevOps after standup.

## Day 2 — Wednesday, 2026-05-07

### Khauhelo (Backend)

Yesterday: Completed ERD v0.1 (bookings, rooms, users, recurring_patterns tables); shared on Confluence
Today: Implement database migrations; build REST API skeleton for Story #1 (POST /bookings, GET /rooms/available)
Blockers: None

### Tebello (Frontend)

Yesterday: Completed wireframes for booking flow; identified missing components
Today: Build reusable RoomCard component with capacity badge; begin DateTimePicker component
Blockers: None

### Alika (Full-stack)

Yesterday: Azure AD spike successful — OAuth2 authorization code flow works with corporate tenant
Today: Integrate auth middleware into API; protect booking endpoints; begin user context injection
Blockers: None

### Sandiso (QA)

Yesterday: Cypress project scaffolded; 5 API contract tests drafted for Story #1
Today: Write unit test cases for booking validation logic; begin edge-case list (double-booking, timezone)
Blockers: QA environment still pending — working against Khauhelo’s local API for now

### X-Man (Scrum Master)

Notes: Good momentum. ERD approved by team with minor feedback. Alika’s auth success unblocks Story #1 integration.
Action: Confirmed with DevOps — QA environment ETA moved to Day 4.

## Day 3 — Thursday, 2026-05-08
### Khauhelo (Backend)

Yesterday: Database migrations deployed to local dev; API skeleton for Story #1 80% complete
Today: Complete booking creation endpoint with conflict detection; write unit tests for availability query
Blockers: None

### Tebello (Frontend)

Yesterday: RoomCard component built and reviewed; DateTimePicker 60% complete
Today: Finish DateTimePicker with timezone handling; begin booking form page layout
Blockers: None

### Alika (Full-stack)

Yesterday: Auth middleware integrated; protected endpoints active
Today: Connect frontend login flow to Azure AD; begin booking form state management (React Context)
Blockers: None

### Sandiso (QA)

Yesterday: 12 unit test cases drafted; edge-case list reviewed with Khauhelo
Today: Run first integration test against local API; document 2 bugs found in validation logic
Blockers: QA environment delayed to Day 4; local testing sufficient for now

### X-Man (Scrum Master) 

Notes: Story #1 progressing well across all layers. Minor concern: Tebello’s DateTimePicker more complex than estimated due to timezone logic.
Action: Suggested Tebello and Alika pair on timezone handling after lunch.

## Day 4 — Friday, 2026-05-09
### Khauhelo (Backend)

Yesterday: Booking creation endpoint complete with conflict detection; availability query optimized with index
Today: Begin Story #2 (Recurring Meetings) — design recurrence schema using RRULE pattern; spike iCalendar format
Blockers: None

### Tebello (Frontend)

Yesterday: DateTimePicker complete with timezone support; booking form layout 70% done
Today: Complete booking form with validation; integrate with Khauhelo’s API for end-to-end booking creation
Blockers: None

### Alika (Full-stack)

Yesterday: Frontend login flow connected to Azure AD; React Context for auth state working
Today: Pair with Tebello on booking form API integration; begin Story #4 (Cancellation) — design DELETE /bookings/{id} endpoint
Blockers: None

### Sandiso (QA)

Yesterday: First integration tests passing; 2 validation bugs filed and fixed by Khauhelo same day
Today: QA environment finally provisioned! Deploy tests to QA; begin Story #1 acceptance test suite
Blockers: QA environment ready — no blockers today 🎉

### X-Man (Scrum Master)

Notes: QA environment resolved. Team velocity feels on track. Story #1 likely to hit In Review by Day 5.
Action: Updated Asana — moved Story #1 to In Progress, Story #2 to In Progress.

## Day 5 — Monday, 2026-05-12
### Khauhelo (Backend)

Yesterday: Story #2 recurrence schema drafted; RRULE spike successful
Today: Implement recurring booking generation service; build parent/child instance model
Blockers: None

### Tebello (Frontend)

Yesterday: Booking form complete; API integration working locally — can create bookings end-to-end!
Today: Polish booking form UX (loading states, error messages); prepare Story #1 for code review
Blockers: None

### Alika (Full-stack)

Yesterday: Paired with Tebello on API integration; drafted cancellation endpoint spec
Today: Implement Story #4 cancellation endpoint with soft-delete and audit trail; build frontend cancel button
Blockers: None

### Sandiso (QA)

Yesterday: QA environment active; Story #1 acceptance tests 80% complete
Today: Complete Story #1 acceptance tests; begin Story #4 test cases
Blockers: None

### X-Man (Scrum Master)

Notes: Story #1 end-to-end flow working locally — major milestone. Tebello and Khauhelo demoed booking creation to the Product Owner during lunch and received positive feedback on the UX direction.
Action: Moved Story #1 to In Review. Scheduled Story #1 demo for Day 6.