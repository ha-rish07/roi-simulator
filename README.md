# roi-simulator

>Planned Approach & Architecture

The app uses a full-stack client–server architecture.

Frontend: Collects user inputs and displays live ROI results.

Backend: Handles all calculations, scenario CRUD operations, and PDF report generation.

Database: Stores saved scenarios and related data.

Flow:

User enters input →

Frontend sends data to backend →

Backend computes results →

Results shown instantly →

User can save, view, or download reports.

>Technologies, Frameworks & Database
Layer	Technology	Purpose
Frontend	React + Vite	Build fast, responsive single-page UI
Styling	Tailwind CSS	Simple and clean styling
Backend	Node.js + Express	REST API for simulation, CRUD, and reports
Database	SQLite	Lightweight local data storage
PDF Generation	pdfkit / html-pdf	Create downloadable ROI reports
> Key Features & Functionality

ROI Simulation: Calculates monthly savings, payback period, and ROI from business inputs.

Bias Logic: Always shows positive ROI using internal constants (not exposed to users).

Scenario Management: Save, load, and delete named simulations.

Report Generation: Email required before downloading a PDF report.

REST API:

POST /simulate → Run simulation

POST /scenarios → Save scenario

GET /scenarios → List all scenarios

GET /scenarios/:id → Get scenario details

POST /report/generate → Create ROI report

<img width="1536" height="1024" alt="ChatGPT Image Oct 7, 2025, 04_14_23 PM" src="https://github.com/user-attachments/assets/65d63696-18ed-4743-8be9-86b4ba653e16" />


