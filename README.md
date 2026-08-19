# EZ Tech Repair Manager

A full-featured device repair ticket management web app built for **EZ Tech Mobile** — a real repair business operating under Amazon Home Services. Designed to track every device from customer drop-off to pickup without losing a single detail.

**Live App:** https://ojwhite11.github.io/EZ_Ticket_Tracker/

---

## What It Does

EZ Tech Repair Manager gives a repair shop a single place to manage every open job. Instead of sticky notes, spreadsheets, or memory, every ticket moves through a defined lifecycle with full history attached.

Ticket stages: **Received → Diagnosing → Awaiting Parts → In Repair → Testing → Ready for Pickup → Delivered**

---

## Features

**Dashboard**
- KPI tiles showing open ticket count, devices ready for pickup, and overdue jobs
- 7-column Kanban board — one column per repair stage
- Toggle between Kanban view and a sortable list/table view
- Priority and technician filters
- Team workload panel showing tickets per tech
- Recent activity feed

**Ticket Management**
- Create new tickets with: customer name, device, issue description, priority (Low / Normal / Urgent), assigned technician, and estimated completion date
- Full ticket detail modal with repair checklist, activity timeline, and workflow action buttons
- Move tickets forward or backward through any stage from the detail view
- Overdue tickets flagged with a red border and alert icon
- Unique ticket IDs (EZ-XXXX format)

**Activity Log**
- Dedicated Activity view showing a chronological feed of every action across all tickets
- Sourced from individual ticket history, merged and sorted by timestamp

**UX Details**
- Dark theme with amber accent color matching the EZ Tech brand
- Responsive layout — works on desktop, tablet, and mobile
- Search by customer name or device
- Toast notifications on ticket updates
- Keyboard shortcut: Escape closes any open modal
- View preference (Kanban vs List) saved to localStorage

---

## How to Use

1. Open the app at the live link above
2. **Dashboard** is the default view — shows your full repair queue in Kanban form
3. Click any ticket card to open the detail panel
4. Use the **Move to →** buttons inside the detail panel to advance a ticket through stages
5. Check off tasks in the repair checklist as work is completed
6. Click **+ New Ticket** in the top bar to intake a new device
7. Use the **Activity** nav item to see a full timeline of everything that's happened across all jobs
8. Filter the board by priority or technician using the dropdowns above the Kanban columns

---

## Tech Stack

- **Vanilla HTML / CSS / JavaScript** — zero dependencies, zero build process
- Single `index.html` file — deployable anywhere static files are served
- Hash-based client-side routing (`#dashboard`, `#tickets`, `#activity`)
- CSS custom properties for the full design token system
- Google Fonts (Inter + IBM Plex Mono) via CDN
- localStorage for view preference persistence

---

## AI Tools Used

This project was built using multiple AI tools across different phases:

| Phase | Tool | Role |
|---|---|---|
| Initial build | ChatGPT (GPT-4o) | Scaffolded the React + TypeScript + Next.js source app |
| Research & Design | Claude (Cowork) | Competitive research on Orderry, Fixitize, RepairDesk; hybrid design spec |
| Bug diagnosis | Claude (Cowork) | Browser automation audit of the live React app; identified routing failures |
| Source code fix | Claude (Cowork) | Patched `page.tsx` — added `hashchange` listener + conditional view rendering |
| GitHub Pages version | Claude (Cowork) | Rebuilt as standalone HTML with vanilla JS for zero-dependency deployment |

---

## Project Context

Built as the final project for an AI Applications course at University of Advancing Technology (UAT). The assignment required selecting a real-world use case, using multiple AI tools to build it, and deploying to GitHub Pages.

EZ Tech Mobile is an active device repair business with an Amazon Home Services contract and a 100% customer satisfaction record. This app was designed around its actual workflow.

---

## Author

**Oshay White**  
EZ Tech Mobile | UAT — AS in 3D Maker & Fabrication  
GitHub: [@ojwhite11](https://github.com/ojwhite11)
