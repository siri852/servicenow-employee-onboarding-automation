# ServiceNow Employee Onboarding Automation

Multi-department employee onboarding built on ServiceNow. One HR form submission creates parallel tasks for HR, IT, Finance and Admin, assigns each to the right group, tracks them against an SLA and reports progress on a dashboard, with no manual coordination.


# The Problem

Onboarding a new hire usually means chasing several departments by email. Tasks get missed, ownership is unclear and nobody can see what is overdue. This app turns a single request into tracked, assigned and time-bound work.

# How It Works
HR submits the Employee Onboarding catalog item.
Flow Designer creates 4 SC Tasks in parallel: HR, IT, Finance and Admin.
A Business Rule (GlideRecord) assigns each task to the correct assignment group.
A 5-day resolution SLA starts on each task, with an email notification on breach.
A dashboard shows task volume, ownership, state and priority.
# Features
Area	What was built
Service Catalog	Custom catalog item with 6 variables: Employee Name, Start Date, Department, Manager, Location, Designation
Flow Designer	Flow that creates 4 parallel SC Tasks on submission
Business Rule	Server-side script using GlideRecord to auto-assign tasks to the correct group
SLA	5-day resolution SLA with breach email notification
Dashboard	4 KPI widgets: Total Tasks, Tasks by Assignment Group, Tasks by State, High Priority Tasks

# Demo

Watch the 2-minute walkthrough: [add your video link here]

# Tech Stack
ServiceNow Flow Designer
Service Catalog and Catalog Builder
JavaScript (Business Rules, GlideRecord)
SLA Definitions and Notifications
Platform Analytics Dashboard
# Installation
Download sys_remote_update_set_3475cc7ec3b403102913f73ed401319e.xml from this repository.
In your instance, go to System Update Sets > Retrieved Update Sets.
Click Import Update Set from XML and upload the file.
Open the imported update set, click Preview Update Set, then Commit Update Set.
# Possible Next Steps
Add manager approval before tasks are created
Sync new-hire data with an external HR system through a REST integration
Add ACLs and roles to restrict who can submit the request
# Author

Sirigireddy Siri, ServiceNow CAD and CSA certified LinkedIn | GitHub
