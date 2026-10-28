# Student Life Rescue Web Plan

## Approach
Build a responsive React dashboard in the initialized web-db-user project. The browser preview uses clearly labeled demo data in localStorage so the student can immediately run and demonstrate the interface without Oracle. The existing Python + Oracle project remains the academic database implementation; this web preview does not claim Oracle-backed persistence. Data helpers will keep the feature model aligned with the six Oracle tables and will support add, complete/submit, search/filter, delete, calendar views, and reports.

## Design
Three possible directions: **Quiet Command Center** — low-contrast academic operations UI (0.07); **Midnight Study Club** — dark editorial student planner (0.06); **Precision Sprint** — energetic KPI-first productivity dashboard (0.08). Chosen: Quiet Command Center.

- **Design movement:** modern SaaS dashboard with editorial typography and calm utility.
- **Core principles:** hierarchy before decoration; fast scanning; strong state feedback; responsive density.
- **Color philosophy:** navy sidebar creates focus, violet marks action, teal signals progress, amber/red are reserved for deadline risk.
- **Layout paradigm:** fixed navigation rail + spacious asymmetric workspace with metric strip and task timeline.
- **Signature elements:** lavender score ring, soft white cards with thin borders, deadline-risk pills.
- **Interaction philosophy:** every click produces a visible state change; destructive actions confirm; demo data is labeled.
- **Typography:** Inter/system sans for UI, strong 30–36px page titles, compact uppercase metadata.
- **Brand essence:** a calm academic command center for students who want fewer deadline surprises; focused, supportive, practical.
- **Brand voice:** “Make the next deadline visible.” / “Small wins compound into breathing room.”
- **Signature brand color:** #7667F8 violet.

## Structure
- `client/src/pages/Home.tsx`: complete interactive dashboard shell and module views.
- `client/src/index.css`: responsive visual system and dashboard styling.
- `public/manus-routes.json`: route manifest for the preview.
- `drizzle/` and `server/`: retained starter infrastructure for later durable persistence.
