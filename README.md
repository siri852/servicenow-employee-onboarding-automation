# ServiceNow Employee Onboarding Automation

## Project Overview
Automates multi-department employee onboarding on ServiceNow.
One HR form submission triggers parallel tasks across HR, IT, Finance 
and Admin departments simultaneously — no manual coordination needed.

## Features Built
- **Service Catalog Item** — Custom form with 6 variables (Employee Name, 
  Start Date, Department, Manager, Location, Designation)
- **Flow Designer** — 4 parallel SC Tasks created automatically on submission
- **Business Rule** — Auto-assignment to correct group via GlideRecord (JavaScript)
- **SLA Management** — 5 day resolution SLA with breach email notification
- **Performance Analytics Dashboard** — 4 KPI widgets (Total Tasks, Tasks by 
  Assignment Group, Tasks by State, High Priority Tasks)

## Technologies Used
- ServiceNow Flow Designer
- JavaScript (GlideRecord, Business Rules)
- Service Catalog & Catalog Builder
- SLA Definitions & Notifications
- Platform Analytics Dashboard

## Certifications
- ServiceNow Certified System Administrator (CSA)
- ServiceNow Certified Application Developer (CAD)

## How to Install
1. Download the XML file from this repository
2. Go to ServiceNow → System Update Sets → Retrieved Update Sets
3. Click Import Update Set from XML
4. Upload the XML file
5. Preview Update Set → Commit Update Set
