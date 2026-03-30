# P02_Data_Inventory_Report_T  
Document Name: **Data Inventory Report**

---

## Document Information

| Field | Value |
|------|------|
| Project Name | *\[e.g. Customer Churn Prediction\]* |
| Project Code | *\[e.g. CCP-2025-01\]* |
| CRISP-DM Phase | P02 - Data Understanding |
| Artifact Level | T - Technical Artifact |
| Document Owner (Role) | *\[Data Lead \| DS Lead\]* |
| Version | *\[0.0.1\]* |
| Last Updated | *\[DD Month YYYY\]* |
| Document Status | *\[Draft \| Final\]* |

---

Working version: [Google Doc template](https://cutt.ly/BtPhLJXz)

---

# Introduction

*\[This document provides a structured and controlled format for identifying, describing, and registering all datasets collected during CRISP-DM Phase P02 - Data Understanding.  
It ensures traceability between business objectives and available data sources, documents ownership and access constraints, and establishes the initial data baseline before profiling and transformation activities begin.  
This document supports technical transparency, reproducibility, and alignment with project scope defined in the Project Plan.\]*

*\[**Example**: In the Customer Churn Prediction project, this document registers internal CRM tables, billing history datasets, customer support interaction logs, and external demographic enrichment sources collected for churn modeling.\]*

## Purpose

*\[Describe the objective of this document clearly and concisely.*

*The purpose is to formally document what data has been collected, from which sources, under what ownership and access conditions, and how it relates to the analytical objective.*

*The section should allow the reader to quickly determine whether this document contains the required dataset inventory information.\]*

*\[**Example**: The purpose of this document is to register all raw datasets collected to support churn prediction modeling, including customer contract history, service usage metrics, and historical churn labels.\]*

## Audience

*\[Identify the primary and secondary audiences who rely on this document for execution, validation, or oversight.*

*Typical recipients include Data Scientists, Data Engineers, Analytics teams, Delivery Leads, and Data Governance stakeholders.*

*Specify roles rather than individual names.\]*

*\[**Example:** This document is intended for the Data Science team performing exploratory analysis, the Data Engineering team preparing data pipelines, and the Delivery Lead overseeing scope alignment.\]*

## Definitions, Acronyms, and Abbreviations

*\[Provide definitions for all project-specific terms, dataset abbreviations, system names, and technical identifiers required to correctly interpret the document.*

*Where applicable, reference the central Project Glossary instead of duplicating definitions.*

*Only include terms that are necessary to interpret this specific document.\]*

| # | Term | Explanation |
|-----|:----|:----|
| 1. | *\[CRM\]* | *\[Customer Relationship Management system storing contract and demographic data.\]* |
| 2. | *\[Churn\]* | *\[Customer termination of service within the defined observation window.\]* |
| 3. | *\[ARPU\]* | *\[Average Revenue Per User, calculated from monthly billing records.\]* |
| 4. |  |  |
| 5. |  |  |
| 6 |  |  |
| 7. |  |  |

## Document Overview

*\[Briefly explain how this document is structured and how information is organized.*

*Keep this section concise (2-4 sentences).*

*Describe the logical grouping of data source identification, structural metadata, ownership, access restrictions, and preliminary relevance notes.\]*

*\[**Example**: This document is structured into sections covering data source identification, dataset ownership, structural characteristics (format, volume, update frequency), access constraints, and relevance to churn modeling objectives.\]*

---

# References

*\[Provide links or formal references to documents, systems, repositories, or governance artifacts referenced within this document.*

*Include only documents that are explicitly cited or required for contextual interpretation.*

*Avoid listing unrelated materials.\]*

| # | Document | Explanation |
|-----|:----|:----|
| 1. | *\[[P01_Project_Plan_G](../phase-1-business-understanding/P01_Project_Plan_G.md)\]* | *\[Defines business objectives and analytical scope for churn prediction.\]* |
| 2. | *\[Enterprise Data Catalog\]* | *\[Source metadata repository for CRM tables.\]* |
| 3. |  |  |
| 4. |  |  |
| 5. |  |  |
| 6 |  |  |
| 7. |  |  |

---

# Data Collection Baseline

*\[This section formally registers all datasets collected during CRISP-DM Phase P02 \- Data Understanding as part of Task 2.1 Collect Initial Data.*

*It establishes the initial data baseline by documenting data sources, structural characteristics, ownership, storage locations, and access conditions.*

*Only raw, acquired datasets must be recorded here. No profiling, quality assessment, transformation planning, or analytical interpretation should be included in this section.*

*The purpose of this section is to provide a transparent and traceable inventory of data assets available for subsequent analysis in Task 2.2 Describe Data.\]*

*\[**Example**: In the Customer Churn Prediction project, this section documents the collection of CRM customer records, transaction history tables from the Data Warehouse, customer support interaction logs, mobile app activity logs, and historical churn labels extracted from BI systems. Each dataset is registered with its owner, storage location, format, update frequency, and snapshot date to establish the initial analytical data baseline.\]*

## Data Source Register

*\[This section provides a formal register of all raw datasets acquired during Task 2.1 Collect Initial Data.*

*Each row represents a distinct dataset that has been physically accessed, extracted, or formally confirmed as available for analytical use.*

*The purpose of this register is to establish a clear and reproducible data acquisition baseline by documenting:*

*  *where the data originates from,*  
*  *where it is stored after acquisition,*  
*  *how it was collected, and*  
*  *under whose ownership and access control it operates.*

*This section operates strictly at the data source level.*

*It must not include attribute-level descriptions, data profiling metrics, quality statistics, transformation plans, or analytical interpretation.*

*Only datasets actually acquired or granted access to must be recorded.\]*

*\[**Example**: In the Customer Churn Prediction project, this register includes CRM customer master data, transaction history tables from the Enterprise Data Warehouse, mobile application activity logs stored in AWS, customer support ticket records, and historical churn labels extracted from BI systems. Each dataset is recorded with its owner, storage location, format, update frequency, snapshot date, and method of acquisition to ensure traceability and reproducibility.\]*

*\[Field description.*  
***Core** fields are mandatory for CRISP-DM compliance.*

***Advanced** fields may be completed depending on organizational maturity and governance requirements.*

* ***Data Source ID (Core**)  \- Assign a unique identifier for each dataset (e.g., DS-01, DS-02). Maintain consistent numbering across the document.*  
* ***Data Source Name (Core)**\- Provide a clear and human-readable name of the dataset or table group.*  
* ***Internal / External (Advanced)** \- Specify whether the data originates from internal enterprise systems or external providers.*  
* ***Source System (Core)** \- Indicate the originating system, application, or provider from which the data was collected.*  
* ***Description (Advanced)**\- Briefly describe the type of information contained in the dataset. Avoid analytical interpretation.*  
* ***Data Owner \- Role (Advanced)** \- Specify the accountable role responsible for the dataset (not individual names unless required by governance policy).*  
* ***Storage Location (Core)** \- Indicate where the dataset is physically stored after collection (e.g., Data Warehouse, AWS S3, local secure storage).*  
* ***Format (Core)** \- Specify the data format (e.g., SQL table, CSV, JSON, API endpoint).*  
* ***Update Frequency (Advanced)** \- Indicate how often the dataset is updated (e.g., Daily, Monthly, Real-Time, One-time Snapshot).*  
* ***Snapshot Date (Core)** \- Record the date when the dataset was extracted or confirmed for analytical use. This establishes the baseline reference.*  
* ***Collection Method (Core)** \- Specify how the dataset was acquired (e.g., ETL pipeline, API extraction, manual export, direct database access).*  
* ***Estimated Volume (Advanced)** \- Provide an approximate size of the dataset (e.g., number of records, file size). Do not include statistical profiling.*  
* ***Sensitivity Level (Advanced)** \- Indicate the data sensitivity classification according to the organization’s data governance or information security policy.*   
  *Typical classifications may include: Public, Internal, Confidential, Restricted, or PII-containing datasets.*   
  *If no formal classification exists, provide a clear descriptive label reflecting the sensitivity of the data (e.g., “Contains Personal Identifiable Information (PII)” or “Financial Transaction Data”).*  
  *This field supports secure handling, controlled access, and compliance alignment but does not replace formal governance documentation.\]*

| Data Source ID (Core) | *\[DS-01\]* | *\[DS-02\]* | *\[DS-03\]* | *\[DS-04\]* |
| :---- | :---- | :---- | :---- | :---- |
| **Data Source Name (Core)** | *\[Customer Master Data\]* | *\[Transaction History\]* | *\[Mobile App Activity\]* | *\[Churn Labels\]* |
| **Internal / External (Advanced)** | *\[Internal\]* | *\[Internal\]* | *\[Internal\]* | *\[Internal\]* |
| **Source System (Core)** | *\[CRM System\]* | *\[Core Banking System\]* | *\[Mobile Backend\]* | *\[BI Reporting Layer\]* |
| **Description (Advanced)** | *\[Core customer demographic\]* | *\[Historical transactions\]* | *\[Login & activity logs\]* | *\[Historical churn status\]* |
| **Data Owner \- Role (Advanced)** | *\[Customer Data Manager\]* | *\[Banking Data Team\]* | *\[IT Operations Lead\]* | *\[Marketing Analytics Lead\]* |
| **Storage Location (Core)** | *\[Enterprise DW (SQL)\]* | *\[Data Warehouse (SQL)\]* | *\[AWS S3 Bucket\]* | *\[Analytics Sandbox\]* |
| **Format (Core)** | *\[SQL Table\]* | *\[SQL Table\]* | *\[JSON Files\]* | *\[CSV Export\]* |
| **Update Frequency (Advanced)** | *\[Daily\]* | *\[Daily\]* | *\[Real-Time\]* | *\[Quarterly\]* |
| **Snapshot Date (Core)** | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* |
| **Collection Method (Core)** | *\[ETL Extraction\]* | *\[Direct DB Access\]* | *\[API Extraction\]* | *\[Manual Export\]* |
| **Estimated Volume (Advanced)** | *\[\~1.2M records\]* | *\[\~45M records\]* | *\[\~120M log events\]* | *\[\~250K records\]* |
| **Sensitivity Level (Advanced)** | *\[Confidential \- PII\]* | *\[Confidential \- Financial\]* | *\[Internal \- Behavioral Data\]* | *\[Internal \- Analytical Label\]* |

## Data Acquisition Issues & Resolutions

*\[This section documents any issues encountered during Task 2.1 Collect Initial Data and the actions taken to resolve them.*

*Each issue related to data access, extraction, format incompatibility, permission restrictions, incomplete delivery, corrupted files, or technical integration barriers must be recorded.*

*The purpose of this section is to support transparency, traceability, and reproducibility of the data acquisition process. Recording issues and their resolutions ensures that future replication of this project — or similar projects — can anticipate and mitigate recurring challenges.*

*Only acquisition-related issues should be documented here. Data quality observations, profiling findings, or analytical insights must be documented in the Data Dictionary Report (Task 2.2).\]*

*\[**Example:** During the Customer Churn Prediction project, several acquisition challenges were encountered, including restricted access to CRM tables due to role-based permissions, incomplete transaction exports caused by query timeouts, and inconsistencies in timestamp formats across mobile application logs. Each issue was documented along with the corrective action taken, such as obtaining extended database permissions, optimizing extraction queries, and standardizing timestamp formats during ingestion.\]*

*\[Data Acquisition Issues & Resolutions \- Field-Level Operational Instructions:*

* ***Issue ID** \- Assign a unique identifier for each recorded issue (e.g., ISS-01, ISS-02). Maintain consistent numbering within this document.*  
* ***Related Data Source ID** \- Reference the corresponding Data Source ID from Section 3.1. If the issue affects multiple datasets, list all applicable IDs separated by commas.*  
* ***Issue Description** \- Provide a clear and concise description of the acquisition-related problem encountered. Focus strictly on access, extraction, format, permission, or ingestion barriers. Do not include analytical findings.*  
* ***Impact on Data Acquisition** \- Describe how the issue affected data availability, completeness, timing, or integrity during the acquisition stage. Quantify impact where possible (e.g., delay duration, partial extraction).*  
* ***Resolution Implemented** \- Document the corrective action taken to resolve the issue. The description should be specific enough to allow replication in future projects.*  
* ***Resolution Date** \- Record the date when the issue was fully resolved and data acquisition was successfully completed or restored.*  
* ***Responsible Role** \- Indicate the role accountable for resolving the issue (e.g., Data Engineer, IT Security Lead). Use roles rather than individual names unless governance policy requires otherwise.*  
* ***Status** \- Indicate the current state of the issue using standardized labels such as: Open, In Progress, Resolved, or Escalated. At the conclusion of Task 2.1, all issues should ideally be marked as Resolved or formally documented as Accepted Risk.\]*

| Issue ID | *\[ISS-01\]* | *\[ISS-02\]* | *\[ISS-03\]* |
| :---- | :---- | :---- | :---- |
| **Related Data Source ID** | *\[DS-01\]* | *\[DS-02\]* | *\[DS-03\]* |
| **Issue Description** | *\[Access to CRM tables restricted by IT\]* | *\[Transaction export failed (timeout)\]* | *\[Inconsistent timestamp formats in logs\]* |
| **Impact on Data Acquisition** | *\[Delayed data extraction by 3 days\]* | *\[Incomplete dataset extraction\]* | *\[Potential ingestion errors\]* |
| **Resolution Implemented** | *\[Access rights granted by IT Security\]* | *\[Query optimized & extraction segmented\]* | *\[Standardized format during ingestion\]* |
| **Resolution Date** | *\[2025-02-03\]* | *\[2025-02-02\]* | *\[2025-02-04\]* |
| **Responsible Role** | *\[IT Security Lead\]* | *\[Data Engineer\]* | *\[Data Engineer\]* |
| **Status** | *\[Resolved\]* | *\[Resolved\]* | *\[Resolved\]* |

## Data Integration Notes

*\[This section documents any initial data integration activities performed during Task 2.1 Collect Initial Data.*

*If multiple datasets were combined, joined, harmonized, or structurally aligned at the acquisition stage, the integration logic must be recorded here at a high level.*

*This section is not intended to describe full data preparation, feature engineering, or transformation logic. Only initial structural integration steps required to enable subsequent data understanding activities should be documented.*

*If no integration was performed at this stage, this section may be marked as “Not Applicable.”*

*The purpose of this section is to ensure transparency and reproducibility of any structural alignment or consolidation actions taken before Task 2.2 Describe Data.\]*

*\[**Example** \- In the Customer Churn Prediction project, initial integration was required to align CRM customer records with transaction history tables using Customer\_ID as the primary key. Additionally, mobile app activity logs were mapped to customer profiles using hashed account identifiers. These integration steps were performed to create a consolidated analytical dataset for subsequent description and profiling activities. No feature-level transformations were applied at this stage.\]*

*\[Data Integration Notes \- Field-Level Operational Instructions:*

* ***Integration ID** \-  Assign a unique identifier for each integration activity (e.g., INT-01, INT-02). Maintain consistent numbering within this document to ensure traceability.*  
* ***Data Sources Involved** \- List all relevant Data Source IDs from Section 3.1 that participate in the integration. Use the predefined identifiers (e.g., DS-01, DS-02) rather than dataset names to preserve referential consistency.*  
* ***Integration Type** \- Specify the structural integration method used (e.g., Inner Join, Left Join, Union, Aggregation, Key Mapping, Data Consolidation). This field should describe the structural mechanism, not business logic.*  
* ***Join / Alignment Key** \- Indicate the primary field(s) used to align datasets (e.g., Customer\_ID, Account\_Number, Hashed\_User\_ID). If composite keys are used, list all relevant fields.*  
* ***Integration Location** \- Specify where the integration was technically executed (e.g., Enterprise DW, Analytics Sandbox, Python Notebook, ETL Pipeline). This supports reproducibility and auditability.*  
* ***Description** \- Provide a concise high-level explanation of what was integrated and for what structural purpose. Do not document transformation logic or feature engineering details here.*  
* ***Performed By (Role)** \- Indicate the responsible role that executed the integration (e.g., Data Engineer, Data Scientist). Use roles rather than personal names unless governance policy requires otherwise.*  
* ***Date** \- Record the date when the integration activity was completed and the integrated dataset became available for Task 2.2 Describe Data.\]*

| Integration ID | *\[INT-01\]* | *\[INT-02\]* | *\[...\]* |
| :---- | :---- | :---- | :---- |
| **Data Sources Involved** | *\[DS-01, DS-02\]* | *\[\]* |  |
| **Integration Type** | *\[Inner Join\]* | *\[\]* |  |
| **Join / Alignment Key** | *\[Customer\_ID\]* | *\[\]* |  |
| **Integration Location** | *\[Analytics Sandbox\]* | *\[\]* |  |
| **Description** | *\[Merged customer demographics with transaction history\]* | *\[\]* |  |
| **Performed By (Role)** | *\[Data Engineer\]* | *\[\]* |  |
| **Date** | *\[2025-02-02\]* | *\[\]* |  |

## Data Lineage Summary

*\[Provide a concise narrative summary (1–2 paragraphs) describing the overall data acquisition flow.*

*Summarize how datasets were sourced, accessed, any major issues encountered, and how they were structurally integrated prior to Task 2.2 Describe Data.*

*Do not include feature engineering, transformations, or modeling-related preparation steps.*

*The objective of this section is to provide contextual clarity and support reproducibility at a high level.\]*

*\[**Example** \- For the Customer Churn Prediction project, four primary internal data sources were acquired: CRM customer master data, transaction history, mobile application activity logs, and historical churn labels. Data access was established through a combination of ETL extraction and direct database access. One access delay occurred due to permission restrictions in the CRM system, which was resolved through coordination with IT Security.*

*Initial integration was performed in the analytics sandbox environment, where customer demographic records were joined with transaction history using Customer\_ID. Mobile activity logs were aligned via hashed account identifiers. The resulting consolidated dataset served as the baseline input for Task 2.2 Describe Data.\]*
