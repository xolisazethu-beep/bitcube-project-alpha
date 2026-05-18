# Conference Room Booking System
 
- A web application for browsing, booking, and managing conference room reservations within an organisation.

## Table of Contents
- [Project Overview](#project-overview) 
- [System Context](#system-context)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)
- [Contribution Workflow](#contribution-workflow)
- [Future Sections](#future-sections)

## Project Overview
The **Conference Room Booking System** is a web application that allows employees to view available conference rooms, make bookings, and manage existing reservations. It is intended for use by all staff members within an organisation, as well as administrators who manage room availability and configurations

**Key capabilities:**
- Browse available rooms with capacity and amenity filters
- Book a room for a specific date and time slot
- View, edit, or cancel your own bookings
- Admin controls for managing rooms and resolving conflicts


## System Context
 
The application is structured as a standard web project. The major components are:
 
| Component | Description |
|-----------|-------------|
| **Frontend** | Browser-based UI for users to interact with the booking system |
| **Backend / API** | Handles business logic, booking rules, and data persistence |
| **Database** | Stores room definitions, bookings, and user data |
| **Auth Layer** | Manages user identity and access control |



## Getting Started
 
### Prerequisites 
Before running this project locally, ensure you have the following installed:
 
- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [Git](https://git-scm.com/)
- A package manager: `npm` or `yarn`

### Installation
 
```bash
# 1. Clone the repository
git clone https://github.com/<your-org>/conference-room-booking-system.git
 
# 2. Navigate into the project folder
cd conference-room-booking-system
 
# 3. Install dependencies
npm install
 
# 4. Copy the environment variable template and fill in your values
cp .env.example .env
 
# 5. Start the development server
npm run dev
```


## Repository Structure

conference-room-booking-system/
├── docs/                   # Sprint artefacts and project documentation
│   ├── user-stories.md         # Agreed user stories from sprint planning
│   ├── definition-of-done.md   # Team's DoD for this project
│   └── retrospective.md        # Sprint retrospective notes
├── src/                    # Application source code
│   ├── components/             # UI components
│   ├── pages/                  # Page-level views
│   └── api/                    # API routes and handlers
├── .github/
│   ├── PULL_REQUEST_TEMPLATE.md    # Standard PR template
│   └── ISSUE_TEMPLATE/             # Bug and feature request templates
├── .env.example            # Environment variable template
├── README.md               # This file
└── documentation-and-collaboration-reflection.md

### Key Markdown Artefacts
 
| File | Purpose |
|------|---------|
| `docs/user-stories.md` | Describes features from the user's perspective; useful for understanding intended behaviour |
| `docs/definition-of-done.md` | The agreed quality bar for any piece of work to be considered complete |
| `docs/retrospective.md` | Team reflections from the sprint; useful context for past decisions |

## Contribution Workflow
 
This project uses **Pull Requests (PRs)** as the primary vehicle for introducing changes. Direct commits to `main` are not permitted.

### Steps to Contribute

1. **Create a branch** from `main` using a descriptive name:
   ```bash
   git checkout -b feature/room-filter-by-capacity
   ```
 
2. **Make your changes** and commit with clear, meaningful messages:
   ```bash
   git commit -m "feat: add capacity filter to room search"
   ```
 
3. **Push your branch** and open a Pull Request on GitHub:
   ```bash
   git push origin feature/room-filter-by-capacity
   ```
 
4. **Fill in the PR template** — explain what changed, why, and what reviewers should focus on.
5. **Request a review** from at least one teammate.
6. **Address review feedback** before merging.

### Reporting Issues
 
Use the issue templates in `.github/ISSUE_TEMPLATE/` to report bugs or propose new features. Choose the appropriate template and fill in all fields — this helps the team understand and triage the issue without back-and-forth.
 
---
 
## Future Sections
 
The following sections are placeholders for documentation to be added as the project matures:
- **API Reference** — Endpoint documentation for the backend API <!-- TODO -->
- **Deployment Guide** — Instructions for deploying to staging and production <!-- TODO -->
- **Environment Variables** — Full reference of all required `.env` values <!-- TODO -->
- **Testing Strategy** — Overview of unit, integration, and end-to-end test approach<!-- TODO -->
- Accessibility Notes — Known accessibility considerations and standards followed <!-- TODO -->

