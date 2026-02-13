diff --git a/README.md b/README.md
new file mode 100644
index 0000000000000000000000000000000000000000..c1d57bd6754aa3aab25aa06294c4af254338e171
--- /dev/null
+++ b/README.md
@@ -0,0 +1,104 @@
+# Finance Dashboard
+
+A React-based admin and analytics dashboard for exploring finance-oriented metrics with interactive tables, forms, calendars, and charts.
+
+## Overview
+
+This project is a single-page application built with React, Material UI, React Router, and Nivo charts. It includes prebuilt pages for team management, contacts, invoices, FAQs, calendar scheduling, and multiple chart views.
+
+The dashboard ships with mock data so you can run it locally without any backend setup.
+
+## Features
+
+- Responsive sidebar navigation with grouped sections for data, pages, and charts.
+- Dashboard homepage with KPI cards, revenue chart, transactions list, campaign summary, and geographic traffic.
+- Data tables powered by MUI Data Grid (team, contacts, invoices).
+- Form page using Formik and Yup validation.
+- FullCalendar integration for schedule and event visualization.
+- Dedicated bar, line, pie, and geography chart pages (Nivo-based visualizations).
+- Light/dark theme support via Material UI theming.
+
+## Tech Stack
+
+- **Framework:** React (Create React App)
+- **Routing:** React Router
+- **UI:** Material UI + Emotion + React Pro Sidebar
+- **Charts:** Nivo (bar, line, pie, geo)
+- **Forms:** Formik + Yup
+- **Calendar:** FullCalendar
+- **Testing:** React Testing Library + Jest DOM
+
+## Getting Started
+
+### Prerequisites
+
+- Node.js 18+ (recommended)
+- npm 9+
+
+### Installation
+
+```bash
+npm install
+```
+
+### Run in development
+
+```bash
+npm start
+```
+
+The app runs at `http://localhost:3000` by default.
+
+### Build for production
+
+```bash
+npm run build
+```
+
+### Run tests
+
+```bash
+npm test -- --watchAll=false
+```
+
+## Available Routes
+
+- `/` → Dashboard
+- `/team` → Manage Team
+- `/contacts` → Contacts Information
+- `/invoices` → Invoices Balances
+- `/form` → Profile Form
+- `/calendar` → Calendar
+- `/faq` → FAQ Page
+- `/bar` → Bar Chart
+- `/pie` → Pie Chart
+- `/line` → Line Chart
+- `/geography` → Geography Chart
+
+## Project Structure
+
+```text
+finance-dashboard/
+├── public/
+├── src/
+│   ├── components/      # Reusable UI widgets and chart wrappers
+│   ├── data/            # Mock table/chart/geography data
+│   ├── scenes/          # Route-level pages
+│   │   └── global/      # Shared layout (Topbar, Sidebar)
+│   ├── theme.js         # Color tokens + light/dark theme logic
+│   └── App.js           # Main layout and route definitions
+├── package.json
+└── README.md
+```
+
+## Scripts
+
+- `npm start` — start local development server
+- `npm run build` — create optimized production bundle
+- `npm test` — run test suite
+- `npm run eject` — eject CRA configuration (irreversible)
+
+## Notes
+
+- This project currently uses mock/local data and is ideal as a starter template for finance/admin analytics products.
+- You can integrate real APIs by replacing the mock data modules in `src/data/` and wiring network requests in scene/components.
