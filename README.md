# Import Data using Transform Maps & Spreadsheet

> **Repository Description:** Step-by-step documentation and visual guide for importing employee data into ServiceNow using Import Set Tables, Transform Maps, field validation, Coalesce duplicate prevention, and custom reports/dashboards.

---

## 📁 Project Resources & Links

* 📊 **Dataset**: [`Dataset/Sample_Spreadsheet.xlsx`](Dataset/Sample_Spreadsheet.xlsx) — Sample Excel spreadsheet used for importing employee data.
* 📄 **Project Report**: [`Final_Project_Report.pdf`](Final_Project_Report.pdf) — Comprehensive project report.
* 🎥 **Demo Video**: [Watch Demo Video on Google Drive](https://drive.google.com/drive/folders/1l-A8JSE9MAAyO0BhMEwXL-FRcT4iD5xA?usp=sharing) — Video demonstration of the ServiceNow Transform Maps process.

---

## 📂 Folder Structure

```text
.
├── Dataset/
│   └── Sample_Spreadsheet.xlsx
├── Screenshots/
│   ├── Milestone1/
│   │   ├── Creation Of Spreadsheet-1.png
│   │   ├── Creation Of Spreadsheet-2.png
│   │   └── Creation of Tables.png
│   ├── Milestone2/
│   │   ├── Create Importset Table.png
│   │   └── Create Transform Map.png
│   ├── Milestone3/
│   │   ├── Enable Coalesce to Avoid Duplicate Records-1.jpeg
│   │   ├── Enable Coalesce to Avoid Duplicate Records-2.png
│   │   ├── Enable Coalesce to Avoid Duplicate Records-3.png
│   │   ├── Inserting New Data In Excel Format-1.jpeg
│   │   ├── Inserting New Data In Excel Format-2.jpeg
│   │   ├── Inserting New Data In Excel Format-3.jpeg
│   │   ├── Inserting New Data In Excel Format-4.jpeg
│   │   ├── Transform Data & Validate-1.png
│   │   └── Transform Data & Validate-2.png
│   └── Milestone4/
│       ├── Create Reports-1.jpeg
│       ├── Create Reports-2.jpeg
│       ├── Create Reports-3.jpeg
│       ├── Dashboard-1.jpeg
│       └── Dashboard-2.jpeg
├── Demo_Video
├── Final_Project_Report.pdf
└── README.md
```

---

## 🎯 Project Milestones

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

### Milestone 4: Creation Of Reports And Dashboard
**Description:**  
* **Create Reports:** Generates custom reports in ServiceNow to visualize employee data metrics and monitor import results.
* **Dashboard:** Consolidates reports into an interactive dashboard for centralized data visualization and real-time insights.
