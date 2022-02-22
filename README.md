# simple-inventory
Simple Inventory Management System

## Features
1. Enter details of assets (Name, Location, Serial No, Insurance expiry date, Registration details)
2. Notification (email) when insurance expires
3. Attach documents against assets (scanned copies of warranty, registration docs etc.)
4. Enter the locations
5. Reports
6. Export/Import data (Scheduled)
7. Audit trail of updates to assets

## Details
### Asset Details (All fields are not Mandatory)
1. Name
2. Description
3. Asset Category
4. Asset Status
5. Serial Number
6. Sponser Name
7. Registration Number
8. Model Name
9. Purchased Date
10. Sold Date
11. Sold to
12. Warranty Period
13. Warranty End Date
14. Asset Owners
15. Price of the Asset
16. Currency
17. Purpose of the Asset
18. Registration Details
19. Is Insured?
20. Insurance Start Date
21. Insurance End Date
22. Additional Field 1
23. Additional Field 2
24. Tags
25. List of Documents

### Document Details (Scanned/soft copies of documents, images etc.)
1. Document Name
2. Document Description
3. Document

## API Endpoints
### Asset Management
Name | Method | URL
--- | --- | ---
**Get all Assets** | `GET` | */assets*
**Get a Specific Asset** | `GET` | */assets/\<asset id\>*
**Get Assets by Category** | `GET` | */assets?category=\<category code\>*
**Get Assets by Location** | `GET` | */assets?location=\<location code\>*
**Get Assets by Status** | `GET` | */assets?status=\<status code\>*
**Get a Specific Asset** | `GET` | */assets/\<asset id\>*
**Create an Asset** | `POST` | */assets*
**Update an Asset** | `PUT` | */assets/\<asset id\>*
**Update the status of an Asset** | `PUT` | */assets/\<asset id\>/status*
**Activate an Asset** | `PUT` | */assets/\<asset id\>/activate*
**Deactivate an Asset** | `PUT` | */assets/\<asset id\>/activate*

### Asset Owner Management
Name | Method | URL
--- | --- | ---
**Get all Asset Owners** | `GET` | */asset-owners*
**Get a Specific Asset Owner** | `GET` | */asset-owners/\<asset owner id\>*
**Create a Asset Owner** | `POST` | */asset-owners*
**Update a Asset Owner** | `PUT` | */asset-owners/\<asset owner id\>*
**Delete a Asset Owner** | `DELETE` | */asset-owners/\<asset owner id\>*

### Location Management
Name | Method | URL
--- | --- | ---
**Get all Locations** | `GET` | */locations*
**Get a Specific Location** | `GET` | */locations/\<location id\>*
**Create a Location** | `POST` | */locations*
**Update a Location** | `PUT` | */locations/\<location id\>*
**Delete a Location** | `DELETE` | */locations/\<location id\>*

### Asset Category Management
Name | Method | URL
--- | --- | ---
**Get all Asset Categories** | `GET` | */asset-categories*
**Get a Specific Asset Category** | `GET` | */asset-categories/\<asset category id\>*
**Create a Asset Category** | `POST` | */asset-categories*
**Update a Asset Category** | `PUT` | */asset-categories/\<asset category id\>*
**Delete a Asset Category** | `DELETE` | */asset-categories/\<asset category id\>*

### Asset Status Management
Name | Method | URL
--- | --- | ---
**Get all Asset Statuses** | `GET` | */asset-statuses*
**Get a Specific Asset Status** | `GET` | */asset-categories/\<asset-status id\>*
**Create a Asset Status** | `POST` | */asset-statuses*
**Update a Asset Status** | `PUT` | */asset-categories/\<asset-status id\>*
**Delete a Asset Status** | `DELETE` | */asset-categories/\<asset status id\>*

### Data Export & Import
Name | Method | URL
--- | --- | ---
**Export Data** | `GET` | */data-management*
**Import Data** | `POST` | */data-management*
**Schedule Automatic Data Export** | `PUT` | */data-management/schedule-auto-export*
**Activate Automatic Data Export** | `PUT` | */data-management/activate-auto-export*
**Deactivate Automatic Data Export** | `PUT` | */data-management/deactivate-auto-export*
