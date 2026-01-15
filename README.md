Project: Legal Prescription Tracker Pro
Version: 10.0 (Ultimate Edition)
Date: 2026-01-15
Status: Stable, Unblocked

--- ARCHITECTURE ---
Frontend: Single Page Application (SPA)

Tech: HTML5, Tailwind CSS via CDN, Vanilla JS

Features: 3-Column Layout (Sidebar, Main, Chat), Responsive, PWA-ready

Deployment: Google Apps Script Web App (iframeable)

Backend: Google Apps Script (Serverless)

Runtime: V8 Engine

API: doGoogleLogin(), saveMatter(), processScannedDocument(), etc.

Integration: Gemini 2.0 Flash (AI), Gmail (Drafts), Drive (PDFs), Sheets (DB)

Database: Google Sheets

Structure: Relational-style tabs

Tabs:

Tracker (Matters) - Matches 'Tracker (3).csv'

Users (Auth) - Matches 'Users (2).csv'

Clients (CRM) - Matches 'Clients.csv'

Logs (Audit) - Matches 'Logs (1).csv'

Templates (Docs) - Matches 'Templates.csv'

Keys (License) - Matches 'Auth Key (1).csv' (Logic present, UI hidden in v10)

--- KEY FEATURES IMPLEMENTED ---

Authentication: Username/Password login (unblocked).

Dashboard: Real-time stats (Total, Critical <30d, Upcoming <90d).

Matter Management: CRUD operations with auto-calculated prescription dates.

AI Associate:

Chat: Context-aware Q&A side panel.

Vision: "Scan to Capture" using phone camera & Gemini Vision.

Docs: PDF Generation from Google Doc templates via Drive API.

Utilities:

Drive Mode (Voice dictation UI).

CSV Import/Export.

Email Reporting (HTML summary).

User Management (Add/Delete users in Settings).

--- FILE INVENTORY ---

Code.js (Backend Logic)

index.html (Frontend UI)

pwa_wrapper.html (GitHub Pages Container)

manifest.json (PWA Config)

sw.js (Service Worker)

404.html (SPA Router)

--- KNOWN STATE ---

Login is currently unblocked (no license check enforced on UI).

Data initialization uses hardcoded 'Graham/1001' credentials.

AI features require valid 'GEMINI_API_KEY' in Script Properties.
