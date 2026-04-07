# P02-DATA-DICTIONARY-REPORT-T  
Document Name: **Data Dictionary Report**

---

## Document Information

| Field | Value |
|------|------|
| Project Name | *[Customer Churn Prediction]* |
| Project Code | *[CCP-2025-01]* |
| CRISP-DM Phase | **P02 – Data Understanding** |
| Artifact Level | **T – Technical Artifact** |
| Document Owner (Role) | *[Data Lead \| DS Lead]* |
| Version | *[0.0.1]* |
| Last Updated | *[DD Month YYYY]* |
| Document Status | *[Draft \| Final]* |

---

Working version: [Google Doc template](https://cutt.ly/dtPhXLKy)

---
# 1 Introduction

*\[This section introduces the Data Dictionary Report and explains its role within CRISP-DM Task 2.2 Describe Data. The purpose is to document the structural and surface-level characteristics of the acquired datasets. This document must describe data format, volume, structure, field identities, and initial observations, and evaluate whether the acquired data satisfies the project’s business requirements. This section should remain high-level and non-technical.\]*

*\[**Example**: This document describes the structure and content of the datasets acquired for the Customer Churn Prediction project. It includes table-level and field-level metadata, data formats, record counts, and initial surface observations. The objective is to assess whether the available data sufficiently supports churn modeling objectives.\]*

## 1.1 Purpose

*\[Provide a concise statement explaining why this document exists. The purpose should clearly state that this report documents structural and descriptive metadata of acquired datasets and evaluates their suitability for subsequent data preparation and modeling tasks. Avoid operational or transformation details.\]*

*\[**Example**: The purpose of this document is to provide a structured description of all datasets acquired for churn modeling, including their format, size, structure, and key attributes. It also evaluates whether the data meets the analytical requirements defined in the Business Understanding phase.\]*

## 1.2 Audience

*\[Identify the intended readers of this document. This typically includes Data Scientists, Data Engineers, Data Analysts, Data Stewards, and relevant technical stakeholders. Avoid listing individual names; refer to roles.\]*

*\[**Example:** This document is intended for Data Scientists, Data Engineers, and Analytics stakeholders involved in the churn modeling initiative, as well as Data Governance roles responsible for metadata validation.\]*

## 1.3 Definitions, Acronyms, and Abbreviations

*\[Provide definitions for all project-specific terms, dataset abbreviations, system names, and technical identifiers required to correctly interpret the document.*

*Where applicable, reference the central Project Glossary instead of duplicating definitions.*

*Only include terms that are necessary to interpret this specific document.\]*

| \# | Term | Explanation |
| ----- | :---- | :---- |
| 1\. | *\[CRM\]* | *\[Customer Relationship Management system storing contract and demographic data.\]* |
| 2\. | *\[Churn\]* | *\[Customer termination of service within the defined observation window.\]* |
| 3\. |  |  |
| 4\. |  |  |
| 5\. |  |  |
| 6 |  |  |
| 7\. |  |  |

## 1.4 Document Overview

*\[Explain how the document is structured and how the sections relate to CRISP-DM Task 2.2 Describe Data. Provide a short description of each major section to guide readers.\]*

*\[**Example**: Section 3 provides a structured description of each dataset, including table-level metadata and detailed field-level definitions. The final section evaluates whether the acquired data sufficiently supports churn prediction objectives.\]*

# 2 References

*\[List all documents referenced within this report. These typically include the Project Plan, Business Requirements, Data Inventory Report (Task 2.1), and any governance or glossary documents. Provide document identifiers and version references where applicable.*  
*Avoid listing unrelated materials.\]*

| \# | Document | Explanation |
| ----- | :---- | :---- |
| 1\. | *\[[P01_Project_Plan_G](../phase-1-business-understanding/P01_Project_Plan_G.md)\]* | *\[Defines business objectives and analytical scope for churn prediction.\]* |
| 2\. | *\[[P02\_Data\_Inventory\_Report\_T](./P02_Data_Inventory_Report_T.md)\]* | *\[.\]* |
| 3\. |  |  |
| 4\. |  |  |
| 5\. |  |  |
| 6 |  |  |
| 7\. |  |  |

# 3 Data Description Baseline

*\[This section establishes the structural and descriptive baseline of all datasets acquired during CRISP-DM Task 2.1 and examined under Task 2.2 Describe Data.*

*The purpose of this section is to document the objective structural characteristics of the data, including dataset composition, table-level schema structure, field-level metadata, and observable surface properties.*

*This section must remain descriptive in nature. It must not include data cleansing actions, transformation logic, feature engineering decisions, or modeling considerations.*

*All quantitative metrics (record counts, field counts, missing value percentages, distinct value counts) should reflect the dataset state at the documented snapshot date.*

*The objective is to provide transparency, reproducibility, and a shared structural understanding of the data before entering the Data Preparation phase.\]*

*\[**Example**: For the Customer Churn Prediction project, this section documents the structural characteristics of the datasets acquired, including CRM customer master data, transaction history, mobile application activity logs, and historical churn labels.*

*The section provides dataset-level summaries, table-level schema descriptions, and field-level metadata, including data types, nullability, key definitions, and initial surface observations such as missing values and distribution irregularities.*

*The objective is to confirm that the available datasets contain sufficient customer identifiers, historical behavior metrics, and churn labels required to support subsequent data preparation and modeling activities.\]*

## 3.1 Dataset Structural Overview {#dataset-structural-overview}

*\[This subsection provides a high-level structural summary of each dataset acquired and examined under CRISP-DM Task 2.2 Describe Data.*

*The objective is to document quantitative and structural characteristics of each dataset, including size, format, and structural complexity, without duplicating source ownership or access information already documented in the Data Inventory Report (Task 2.1).*

*All metrics must reflect the dataset state at the defined snapshot date.*

*This section must remain descriptive and structural. It must not include data transformation details, feature engineering logic, or modeling assumptions.\]*

*\[**Example**: In the Customer Churn Prediction project, five datasets were examined: CRM Customer Master Data, Transaction History, Mobile App Activity Logs, Customer Support Logs, and Historical Churn Labels.*

*For each dataset, the total number of records, total number of fields, data format, and snapshot date were documented to establish a structural baseline before proceeding to detailed field-level description and surface-level observations.\]*

*\[Dataset Structural Overview Table*

* ***Dataset Name** \- The official name of the dataset as defined in the Data Inventory Report. This should correspond to the dataset identifier used in Task 2.1.*  
* ***Inventory Reference ID** \- The Data Source ID assigned in the Data Inventory Report (e.g., DS-01). This ensures traceability between Task 2.1 and Task 2.2.*  
* ***Record Count** \- Total number of records (rows) present in the dataset at the snapshot date. Must be a numeric value reflecting actual measurement.*  
* ***Field Count** \- Total number of fields (columns) contained in the dataset.*  
* ***Data Format** \- The physical storage format of the dataset (e.g., SQL Table, CSV, JSON, Parquet).*  
* ***Storage Type** \- Logical storage classification (e.g., Relational Database, Flat File, Log-Based File, API Extract).*  
* ***Snapshot Date** \- The date when the dataset structure and metrics were measured. This ensures reproducibility.*  
* ***Contains PII (Y/N)** \- Indicates whether the dataset includes any fields classified as containing Personally Identifiable Information. This is a structural characteristic and must align with the PII assessment in the Field-Level Data Dictionary.\]*

| Dataset Name | *\[Customer Master Data\]* | *\[Transaction History\]* | *\[Mobile App Activity Logs\]* | *\[Customer Support Logs\]* | *\[Historical Churn Labels\]* |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **Inventory Ref ID** | *\[DS-01\]* | *\[DS-02\]* | *\[DS-03\]* | *\[DS-04\]* | *\[DS-05\]* |
| **Record Count** | *\[250,000\]* | *\[12,500,000\]* | *\[8,200,000\]* | *\[320,000\]* | *\[250,000\]* |
| **Field Count** | *\[18\]* | *\[12\]* | *\[9\]* | *\[14\]* | *\[2\]* |
| **Data Format** | *\[SQL Table\]* | *\[SQL Table\]* | *\[JSON\]* | *\[CSV\]* | *\[Excel\]* |
| **Storage Type** | *\[Relational Database\]* | *\[Relational Database\]* | *\[Log-Based File\]* | *\[Flat File\]* | *\[Flat File\]* |
| **Snapshot Date** | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* |
| **Contains PII** | *\[Y\]* | *\[Y\]* | *\[N\]* | *\[Y\]* | *\[N\]* |

## 3.2 Table-Level Structure {#table-level-structure}

*\[This subsection documents the structural schema characteristics of tables or files contained within each dataset identified in [Section 3.1 Dataset Structural Overview](#dataset-structural-overview)*

*The purpose of this section is to describe how data is organized at the table or file level, including row counts, column counts, and structural key relationships where explicitly defined in the schema.*

*This section must capture only objective structural properties that exist in the dataset at the snapshot date. It must not introduce derived relationships, inferred keys, or business logic not formally defined in the data structure.*

*Primary and foreign keys should only be recorded if they are explicitly defined in the database schema or clearly identifiable from structural documentation.*

*This subsection must remain descriptive and structural. It must not include transformation logic, data cleansing decisions, referential integrity enforcement steps, or modeling considerations.\]*

*\[**Example:** In the Customer Churn Prediction project, several datasets contained multiple tables requiring structural documentation.*

*The Transaction History dataset included a primary transactions table with a defined primary key (Transaction\_ID) and a foreign key (Customer\_ID) referencing the Customer Master table.*

*The Mobile App Activity dataset consisted of log-based records without enforced foreign key constraints but included a consistent Customer\_ID field used for structural alignment.*

*This section documents only formally defined keys and structural properties observed in the schema at the snapshot date.\]*

*\[*

* ***Dataset Name** \- The name of the dataset as defined in Section 3.1. Must match exactly to ensure traceability.*  
* ***Table / File Name** \- The exact technical name of the table or file as stored in the database or file system. Use physical names, not business aliases.*  
* ***Row Count** \- Total number of rows contained in the table or file at the snapshot date. Must reflect actual measured quantity.*  
* ***Column Count** \- Total number of columns (fields) present in the table or file.*  
* ***Primary Key Defined (Y/N)** \- Indicates whether a primary key is explicitly defined in the schema.*  
* ***Primary Key Field(s)** \- List the field name(s) that form the primary key. If composite, list all participating fields separated by commas. If none defined, mark as “Not Defined.”*  
* ***Foreign Key(s) Defined (Y/N)** \- Indicates whether foreign key constraints are explicitly defined in the schema.*  
* ***Foreign Key Field(s)** \- List field name(s) that act as foreign keys, if defined. If not defined, mark it as “Not Defined.”*  
* ***Referenced Table(s)** \- The name(s) of table(s) referenced by the foreign key(s). Leave blank or mark “Not Applicable” if no foreign keys exist.*  
* ***File Encoding / Storage Format (if applicable)** \- For non-database sources (CSV, JSON, etc.), specify encoding (e.g., UTF-8) or structural format (e.g., Nested JSON, Flat CSV). For relational tables, may be marked “Not Applicable.”*  
* ***Snapshot Date** \- Date when structure and metrics were measured.\]*

| Dataset Name | *\[Customer Master Data\]* | *\[Transaction History\]* | *\[Mobile App Activity Logs\]* | *\[Customer Support Logs\]* | *\[Historical Churn Labels\]* |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **Table / File Name** | *\[Customers\]* | *\[Transactions\]* | *\[Mobile\_Activity\_Log\]* | *\[Support\_Tickets\]* | *\[Churn\_Labels\]* |
| **Row Count** | *\[250,000\]* | *\[12,500,000\]* | *\[8,200,000\]* | *\[320,000\]* | *\[250,000\]* |
| **Column Count** | *\[18\]* | *\[12\]* | *\[9\]* | *\[14\]* | *\[2\]* |
| **Primary Key Defined** | *\[Y\]* | *\[Y\]* | *\[N\]* | *\[Y\]* | *\[Y\]* |
| **Primary Key Field(s)** | *\[Customer\_ID\]* | *\[Transaction\_ID\]* | *\[Not Defined\]* | *\[Ticket\_ID\]* | *\[Customer\_ID\]* |
| **Foreign Key(s) Defined** | *\[N\]* | *\[Y\]* | *\[N\]* | *\[Y\]* | *\[N\]* |
| **Foreign Key Field(s)** | *\[Not Defined\]* | *\[Customer\_ID\]* | *\[Not Defined\]* | *\[Customer\_ID\]* | *\[Not Defined\]* |
| **Referenced Table(s)** | *\[Not Applicable\]* | *\[Customers\]* | *\[Not Applicable\]* | *\[Customers\]* | *\[Not Applicable\]* |
| **Encoding / Format** | *\[Not Applicable\]* | *\[Not Applicable\]* | *\[JSON (Nested, UTF-8)\]* | *\[CSV (UTF-8)\]* | *\[Excel (XLSX)\]* |
| **Snapshot Date** | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* | *\[2025-02-01\]* |

## 3.3 Field-Level Data Dictionary {#field-level-data-dictionary}

*\[This subsection provides a detailed description of individual data fields contained within the tables or files identified in Section 3.2.*

*The purpose of this section is to document field-level metadata necessary to understand the structure and meaning of the data prior to data preparation and modeling activities.*

*Each field should be described using objective metadata such as field name, data type, description, nullability, and example values. Where available, documented business definitions or data steward descriptions should be used to ensure semantic clarity.*

*Observed surface properties of the field (such as percentage of missing values or typical value ranges) may be recorded to support an initial understanding of the data. These observations must remain descriptive and must not include cleansing decisions, transformation logic, feature engineering strategies, or modeling assumptions.*

*The goal of this section is to establish a shared structural and semantic understanding of the dataset attributes that will later support the Data Preparation and Modeling phases of the CRISP-DM lifecycle.\]*

*\[**Example**:For the Customer Churn Prediction project, this section documents the field-level metadata for attributes contained in the Customer Master dataset, Transaction History dataset, Mobile Application Activity logs, and Churn Label dataset.*

*Examples include customer identifiers, demographic attributes, transaction metrics, activity timestamps, and the churn status indicator. Each field is described with its technical data type, semantic meaning, and example values observed in the dataset snapshot.*

*This documentation allows the project team to clearly understand available customer behavior indicators and ensures that subsequent feature engineering and modeling activities are based on well-defined and traceable data attributes.\]*

*\[Field Definitions:*

* ***Dataset Name** \- The dataset to which the field belongs. Must correspond to the dataset listed in Section 3.1 Data Source Register.*  
* ***Table / File Name** \-  The table or file containing the field, as defined in Section 3.2 Table-Level Structure.*  
* ***Field Name** \- The exact technical name of the field as defined in the database schema or source file structure.*  
* ***Data Type \-** The technical data type of the field (e.g., Integer, Float, String, Boolean, Date, DateTime, JSON, etc.).*  
* ***Business Description** \- A clear description of the meaning and business interpretation of the field. Prefer definitions provided by data owners or data stewards when available.*  
* ***Allow Nulls (Y/N) \-** Indicates whether the field allows missing or null values according to the schema or observed dataset structure.*  
* ***Example Values** \- A few representative values observed in the dataset snapshot to illustrate typical content.*  
* ***Units / Format (if applicable) \-** Units of measurement or formatting rules when relevant (e.g., USD, percentage, ISO date format, timestamp format).*  
* ***Sensitivity Level \-** Indicates whether the field contains sensitive information. Typical categories may include: Public / Internal / Confidential / PII.*  
* ***Notes \-** Optional clarifications such as special interpretation rules, known semantic nuances, or links to business definitions.\]*

| Table / File Name | Field Name | Data Type | Business Description | Nulls | Example Values | Units / Format | Sensitivity | Notes |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| **Dataset Name:** *\[Customer Master Data\]* |  |  |  |  |  |  |  |  |
| *\[Customers\]* | *\[Customer\_ID\]* | *\[String\]* | *\[Unique identifier for each customer\]* | *\[N\]* | *\[CUST10245\]* | *\[Alphanumeric\]* | *\[Internal\]* | *\[Primary identifier\]* |
| *\[Customers\]* | *\[Age\]* | *\[Integer\]* | *\[Age of the customer in years\]* | *\[Y\]* | *\[34, 52, 41\]* | *\[Years\]* | *\[Internal\]* | *\[Missing values possible\]* |
| *\[Customers\]* | *\[Gender\]* | *\[String\]* | *\[Customer gender recorded in CRM\]* | *\[N\]* | *\[M, F\]* | *\[Categorical\]* | *\[PII\]* | *\[Requires standardization\]* |
| **Dataset Name:** *\[Transaction History\]* |  |  |  |  |  |  |  |  |
| *\[Transactions\]* | *\[Transaction\_ID\]* | *\[String\]* | *\[Unique ID of a financial transaction\]* | *\[N\]* | *\[TXN783912\]* | *\[Alphanumeric\]* | *\[Internal\]* | *\[Primary transaction key\]* |
| *\[Transactions\]* | *\[Average\_Balance\]* | *\[Float\]* | *\[Avg account balance over window\]* | *\[Y\]* | *\[5200.5, 1200.0\]* | *\[Currency (USD)\]* | *\[Confidential\]* | *\[Calculated in source\]* |
| **Dataset Name:** *\[Mobile App Logs\]* |  |  |  |  |  |  |  |  |
| *\[Mobile\_Activity\]* | *\[Last\_Login\]* | *\[DateTime\]* | *\[Timestamp of recent mobile login\]* | *\[Y\]* | *\[2025-01-15\]* | *\[ISO 8601\]* | *\[Internal\]* | *\[Engagement analysis\]* |
| **Dataset Name:** *\[Support Logs\]* |  |  |  |  |  |  |  |  |
| *\[Support\_Tickets\]* | *\[Complaint\_Count\]* | *\[Integer\]* | *\[Number of complaints in last year\]* | *\[N\]* | *\[0, 1, 3\]* | *\[Count\]* | *\[Internal\]* | *\[Derived from tickets\]* |
| **Dataset Name:** *\[Churn Labels\]* |  |  |  |  |  |  |  |  |
| *\[Churn\_Labels\]* | *\[Churn\_Status\]* | *\[Boolean\]* | *\[Whether the customer churned\]* | *\[N\]* | *\[0, 1\]* | *\[Binary\]* | *\[Confidential\]* | *\[Target variable\]* |

## 3.4 Initial Data Observations {#initial-data-observations}

*\[Document notable observations identified during the initial inspection of the acquired datasets.*

*Observations recorded in this section should be:*

* *based on preliminary data exploration*  
* *descriptive rather than analytical*  
* *limited to high-level patterns, anomalies, or structural characteristics visible in the data*

*Typical observations may include:*

* *presence of missing values*  
* *unusual or skewed distributions*  
* *inconsistent or unexpected values*  
* *potential data leakage risks*  
* *early hypotheses related to the modeling objective*

*The purpose of this section is to capture early signals that may influence later phases of data preparation and modeling.*

*Observations documented here are preliminary and may be further investigated or validated during subsequent phases.*

*This section does not replace formal data quality assessment.*

*Detailed validation and quantitative checks are performed later in the Data Quality Report (Task 2.4 – Verify Data Quality).\]*

*\[**Example**: Observation Register*

| Observation ID | Field Name | Observation Type | Description | Potential Impact | Next Action |
| :---- | :---- | :---- | :---- | :---- | :---- |
| ***\[OBS-01\]*** | *\[Age\]* | *\[Missing Values\]* | *\[\~1% missing values observed in customer age field\]* | *\[May require imputation or exclusion\]* | *\[Evaluate during Data Prep\]* |
| ***\[OBS-02\]*** | *\[Average\_Balance\]* | *\[Distribution\]* | *\[Strong right-skew distribution detected\]* | *\[May require log scaling\]* | *\[Assess during Feature Eng\]* |
| ***\[OBS-03\]*** | *\[Last\_Login\]* | *\[Temporal Pattern\]* | *\[Records contain very old timestamps (\>5 years)\]* | *\[Inactive accounts or data artifacts\]* | *\[Validate with Biz Owner\]* |
| ***\[OBS-04\]*** | *\[Complaint\_Count\]* | *\[Outliers\]* | *\[Extremely high values detected (\>100 complaints)\]* | *\[Data entry issue or aggregation artifact\]* | *\[Verify aggregation logic\]* |
| ***\[OBS-05\]*** | *\[Churn\_Status\]* | *\[Target Balance\]* | *\[Target variable moderately imbalanced (\~20%)\]* | *\[May require class balancing techniques\]* | *\[Assess during Modeling\]* |

## 3.5 Data Requirement Alignment Assessment {#data-requirement-alignment-assessment}

*\[Assess whether the datasets and fields described in this document are sufficient to support the business and analytical objectives defined during the Business Understanding and Data Understanding phases.*

*This section provides a high-level evaluation of how well the available data aligns with the project’s analytical requirements.*

*The assessment should focus on:*

* *whether the required entities and attributes are present in the available datasets*  
* *whether the target variable (if applicable) is available and sufficiently defined*  
* *whether the historical coverage of the data is adequate for the intended modeling task*  
* *whether any critical data gaps or missing attributes have been identified*  
* *whether additional data sources may be required in later phases*

*The purpose of this section is **not to perform detailed validation**, but to provide an **early assessment of dataset adequacy** for the analytical objective.*

*If major gaps are identified, they should be recorded and may result in:*

* *additional data acquisition*  
* *feature engineering from alternative sources*  
* *refinement of project scope or modeling approach*

*This section serves as a bridge between **Data Understanding** and **Data Preparation**, ensuring that the available data supports the project’s analytical goals.\]*

*\[**Example:** For the Customer Churn Prediction project, the objective is to identify customers who are likely to stop using the bank's services.*

*The available datasets provide information about:*

* *customer demographics*  
* *financial activity*  
* *digital behavior*  
* *historical churn labels*

*Initial assessment indicates that the available data supports the primary analytical objective. Key behavioral and financial indicators that may influence churn risk are present in the datasets.*

*However, several potential gaps were identified:*

* *limited information about customer satisfaction or sentiment*  
* *absence of external competitive behavior data*  
* *incomplete history of customer interactions across all channels*

*These gaps may affect the ability to capture certain churn drivers. During later phases, the project team may consider incorporating additional sources such as:*

* *customer survey data*  
* *customer support transcripts*  
* *marketing interaction history*

*Overall, the current dataset is considered **sufficient for initial modeling**, with opportunities for improvement through additional data enrichment.\]*
