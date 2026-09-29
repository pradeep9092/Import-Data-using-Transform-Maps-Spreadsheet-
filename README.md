# Import Data using Transform Maps & Spreadsheet

## Project Overview
This repository documents the process of importing employee data into ServiceNow using spreadsheets, Import Set staging tables, and Transform Maps, along with data validation and coalesce mechanisms to prevent duplicates.

---

## Folder Structure
```text
.
├── Milestone1/
│   ├── Creation Of Spreadsheet-1.png
│   ├── Creation Of Spreadsheet-2.png
│   └── Creation of Tables.png
├── Milestone2/
│   ├── Create Importset Table.png
│   └── Create Transform Map.png
├── Milestone3/
│   ├── Enable Coalesce to Avoid Duplicate Records-1.jpeg
│   ├── Enable Coalesce to Avoid Duplicate Records-2.png
│   ├── Enable Coalesce to Avoid Duplicate Records-3.png
│   ├── Inserting New Data In Excel Format-1.jpeg
│   ├── Inserting New Data In Excel Format-2.jpeg
│   ├── Inserting New Data In Excel Format-3.jpeg
│   ├── Inserting New Data In Excel Format-4.jpeg
│   ├── Transform Data & Validate-1.png
│   └── Transform Data & Validate-2.png
└── README.md
```

---

## Project Milestones

### Milestone 1: Creation Of Spreadsheet And Table
**Description:**  
Prepares the employee spreadsheet (containing Employee ID, Name, Email, Department, and Location) and uploads it into ServiceNow. Data is stored temporarily in an Import Set Table and mapped to the target Employee table using Employee ID as the unique key to insert new records or update existing ones.

### Milestone 2: Creation Of Import Set Table And Transform Map
**Description:**  
* **Import Set Table:** A staging table that temporarily stores uploaded raw employee data before validation and transformation into target records.
* **Transform Map:** Configures field mapping between the Import Set Table and the target Employee table, setting Employee ID as the coalesce field to identify matching records.

### Milestone 3: Transform Data, Validate, & Enable Coalesce
**Description:**  
* **Transform Data:** Transfers and converts data from the Import Set Table to the target Employee table based on the Transform Map rules.
* **Validate Data:** Checks imported records to ensure mandatory fields (Employee ID, Name, Email) are complete and accurately formatted.
* **Enable Coalesce:** Uses Employee ID as a unique identifier—updating existing employee records when matches are found and inserting new ones to eliminate duplicate records.
