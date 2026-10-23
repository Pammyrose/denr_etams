<p align="center">
  <img src="public/denr_logo.png" alt="DENR logo" width="110">
</p>

<h1 align="center">DENR EcoTrack Asset Management System</h1>

<p align="center">
  A web application for managing employee records, tracking asset inventory and assignments, generating QR asset tags, and monitoring inventory through dashboards and reports.
</p>

## About the Project

DENR EcoTrack supports the Department of Environment and Natural Resources in maintaining a centralized record of employees, equipment, and asset accountability.

The system provides administrators with tools to manage personnel, user accounts, inventory records, and employee asset assignments. Regular users can view their employee profile and assigned assets through their account.

## Features

- Employee record management with organizational units, positions, salary grades, and assignment places.
- Employee data import from Excel spreadsheets.
- Asset inventory management, including purchase details, quantities, locations, conditions, and statuses.
- Asset assignment to employees with assignment dates.
- QR code generation and printable asset tags for identifying inventory items.
- Dashboard summaries for employees, users, assets, and assigned assets.
- Inventory charts showing purchase quantities over time and asset distribution by location.
- Report views with month and year filters.
- Archiving and restoration of employee, user, and inventory records.
- User account management with administrator and regular-user access.
- Employee profiles displaying personnel information and assigned assets.
- Account profile and password settings.

## Technology Stack

| Layer | Technologies |
| --- | --- |
| Backend | PHP 8.2+, Laravel 12, Eloquent ORM |
| Frontend | Vue 3, TypeScript, Inertia.js 2, Tailwind CSS 4 |
| UI components | Reka UI, Lucide icons |
| Asset build | Vite 7, npm |
| Database | Laravel database connections; existing reporting queries use MySQL-specific SQL |
| Spreadsheet processing | PhpSpreadsheet 5 |
| QR code generation | Endroid QR Code 4 |
| Charts | Chart.js 4, vue-chartjs 5 |
| Automated testing | Pest 3, Laravel test utilities |

## System Workflow

1. **Sign in:** A user signs in with their email address and password. Administrators access management tools, while regular users access their profile.
2. **Maintain employee records:** Administrators create or import employee records and maintain personnel reference information.
3. **Record assets:** Administrators enter inventory details, including quantities, purchase information, location, condition, and status.
4. **Assign equipment:** Administrators link assets to employees and record assignment dates. Users can view their assigned equipment in their profile.
5. **Generate asset tags:** Administrators generate QR asset tags and print tags for inventory identification.
6. **Monitor inventory:** Administrators use the dashboard and report filters to review asset quantities, purchase trends, and distribution by location.
7. **Maintain historical records:** Administrators archive records that are no longer active and restore them when needed.

## Security & Access

The application uses email and password authentication and administrator middleware to restrict management workflows. Regular users access their own profile and linked asset information. QR asset-tag pages are accessible without signing in, so information displayed on those pages should be reviewed before deployment.

Operational access is intended for authorized DENR personnel. Account creation, administrator privileges, and employee assignments should be managed by designated administrators according to each user's responsibilities.

Credentials, environment configuration, employee information, operational datasets, and database backups should be shared only through approved internal channels. Production operation requires appropriate hosting controls, HTTPS, and maintained backups.

## Source Code Availability

Source code access should be managed by the project owner or designated DENR system administrator. Requests for access should be directed to the responsible project maintainers for review.

This README provides an overview of the project, its features, and its intended access policy. Repository visibility and collaborator permissions must be configured on the repository hosting platform to enforce that policy; this document does not change repository access.
