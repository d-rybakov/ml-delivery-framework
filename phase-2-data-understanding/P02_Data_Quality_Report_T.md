

# P02_Data_Quality_Report_T 
Document Name: **Data Quality Report**

---

## Document Information

| Field | Value |
|------|------|
| Project Name | *[Customer Churn Prediction]* |
| Project Code | *[CCP-2025-01]* |
| CRISP-DM Phase | **P02 – Data Understanding** |
| Artifact Level | **T – Technical Artifact** |
| Document Owner (Role) | *[DS Lead]* |
| Version | *[0.0.1]* |
| Last Updated | *[DD Month YYYY]* |
| Document Status | *[Draft \| Final]* |
---

Working version: [Google Doc template](https://cutt.ly/HtPh95g5)

---
# 1 Introduction {#introduction}

*\[Provide a brief description of the purpose of this document and its role within the CRISP-DM process.*  
*Explain that the report evaluates the quality of the datasets used in the project by assessing key dimensions such as completeness, consistency, validity, and potential data anomalies.*

*The introduction should clarify that the objective of this report is to identify data quality risks that may impact downstream analytical tasks, particularly Data Preparation (Phase 3\) and Modeling (Phase 4).*

*Also state that detailed dataset structure, field definitions, and metadata are documented separately in the [P02\_Data\_Dictionary\_Report\_T](./P02_Data_Dictionary_Report_T.md) (Task 2.2) and are referenced in this document when needed. The Data Quality Report focuses specifically on assessing whether the available data is suitable for reliable analysis and modeling.\]*

*\[**Example**: This document evaluates the quality of the datasets used in the Customer Churn Prediction project. The objective of the report is to assess whether the available data is sufficiently complete, consistent, and reliable to support exploratory analysis and predictive modeling.*

*The assessment focuses on identifying potential data issues such as missing values, duplicate records, invalid formats, and anomalous values that could affect model performance.*

*The structural description of the datasets, including field definitions and metadata, is documented in the [P02\_Data\_Dictionary\_Report\_T](./P02_Data_Dictionary_Report_T.md) (Task 2.2). This report builds upon that documentation and evaluates the actual quality and usability of the data collected for analysis.\]*

## 1.1 Purpose {#purpose}

*\[Define the primary objective of the Data Quality Report within the CRISP-DM Data Understanding phase. The section clarifies that the document systematically evaluates the reliability and usability of the collected datasets before they are used for analytical modeling.\]*  
*\[Briefly state why data quality assessment is required before proceeding to Data Preparation and Modeling phases. The section should explain that the report identifies potential issues related to completeness, consistency, validity, and integrity of the data.*

*It should also clarify that the goal is not to fix the issues at this stage but to identify and document them, so they can be properly addressed in Phase 3 \- Data Preparation.*

*Keep this section concise (2–3 paragraphs).\]*

*\[**Example**: The purpose of this document is to assess the quality of the datasets used in the Customer Churn Prediction project. The report evaluates key data quality dimensions such as completeness, consistency, validity, and potential anomalies in order to determine whether the data is suitable for exploratory analysis and predictive modeling.*

*The report identifies issues such as missing values, duplicate records, inconsistent formats, and out-of-range values that may affect the reliability of analytical results.*

*The findings documented in this report will guide data cleaning and transformation activities in Phase 3 \- Data Preparation, ensuring that the modeling process is based on reliable and well-understood data.\]*

## 1.2 Audience {#audience}

*\[Identify the primary stakeholders who will use or reference the Data Quality Report. The section clarifies who the document is intended for and how it supports collaboration between technical and business roles during the Data Understanding phase.\]*  
*\[List the main roles that rely on the Data Quality Report and briefly describe how they use the information. The audience typically includes both technical specialists responsible for data preparation and stakeholders overseeing analytical work.*

*This section should remain concise and focus on roles rather than specific individuals.\]*

*\[**Example:** The Data Quality Report is primarily intended for the following roles involved in the Customer Churn Prediction project:*

* *Data Scientists \- to understand data limitations and identify necessary preprocessing steps before feature engineering and modeling.*  
* *Data Engineers \- to identify technical issues in source data pipelines, formats, or extraction logic that may require correction.*  
* *Data Analysts \- to understand the reliability of datasets used for exploratory analysis.*  
* *Project Manager / DS Lead \- to monitor potential risks related to data reliability and ensure appropriate mitigation actions are planned during the Data Preparation phase.\]*

## 1.3 Definitions, Acronyms, and Abbreviations {#definitions,-acronyms,-and-abbreviations}

*\[Provide definitions for technical terms, abbreviations, or dataset-specific concepts that are required to correctly interpret the Data Quality Report.\]*

*\[ List only the terms that are necessary for understanding this document. Avoid duplicating definitions that already exist in the **Project Glossary** or **Data Dictionary Report (Task 2.2)**. When applicable, reference those documents instead of redefining terms.\]*

| \# | Term | Explanation |
| ----- | :---- | :---- |
| 1\. | *\[Missing Value\]* | *\[A data field that contains no recorded value (NULL, blank, or equivalent placeholder). Missing values may occur due to data collection gaps, system errors, or optional input fields.\]* |
| 2\. | *\[Duplicate Record\]* | *\[Two or more records that represent the same real-world entity or event and appear multiple times in the dataset. Duplicates may occur due to data integration or extraction errors.\]* |
| 3\. | *\[Out-of-Range Value\]* | *\[A data value that falls outside the logically valid range for a variable (e.g., negative age or transaction amount). Such values typically indicate data entry or system processing errors.\]* |
| 4\. | *\[Data Completeness\]* | *\[The degree to which required data fields contain valid values across the dataset. Completeness is commonly measured as the percentage of non-missing values per column.\]* |
| 5\. |  |  |
| 6 |  |  |
| 7\. |  |  |

## 1.4 Document Overview {#document-overview}

*\[Explain how the document is structured and how the sections relate to CRISP-DM Task 2.4 Verify data quality. Provide a short description of each major section to guide readers.\]*

*\[**Example**: This document evaluates the quality of the datasets used in the Customer Churn Prediction project.*

*Section 1 introduces the purpose, scope, and audience of the report.*

*Section 3 describes the datasets included in the data quality assessment.*

*Section 4 evaluates key data quality dimensions, including completeness, consistency, duplicates, and value validity.*

*Section 5, 6, 7 summarizes the main data quality findings and identifies potential risks that may affect subsequent data preparation and modeling tasks.\]*

# 2 References {#references}

*\[Provide a list of documents that are referenced in this report and are necessary to correctly interpret the data quality assessment and its context within the CRISP-DM workflow.*  
*List the key project documents referenced in this report. These typically include upstream documents that describe the project objectives and the acquired datasets, as well as documents that provide detailed metadata.*  
*Only include documents that are directly relevant to the interpretation of the Data Quality Report.\]*  
*\[Avoid listing unrelated materials.\]*

| \# | Document | Explanation |
| ----- | :---- | :---- |
| 1\. | *\[[P01_Project_Plan_G](../phase-1-business-understanding/P01_Project_Plan_G.md)\]* | *\[Defines business objectives and analytical scope for churn prediction.\]* |
| 2\. | *\[[P02\_Data\_Inventory\_Report\_T](./P02_Data_Inventory_Report_T.md)\]* | *\[Lists all datasets acquired for the project and provides high-level metadata for each source.\]* |
| 3\. | *\[[P02\_Data\_Dictionary\_Report\_T](./P02_Data_Dictionary_Report_T.md)\]* | *\[Provides detailed field-level metadata (field names, data types, descriptions) for the datasets evaluated in this report.\]* |
| 4\. | *\[[P02\_Exploratory\_Data\_Analysis\_Report\_T](./P02_Exploratory_Data_Analysis_Report_T.md)\]* | *\[Documents exploratory analysis findings that may highlight anomalies or quality issues further investigated in this report.\]* |
| 5\. |  |  |
| 6 |  |  |
| 7\. |  |  |

3. # Data Sources in Scope {#data-sources-in-scope}

*\[Identify the datasets included in the data quality verification process for this project. This section defines the scope of the quality assessment by listing the datasets that were examined as part of CRISP-DM Task 2.4 \- **Verify Data Quality**.\]*

*\[Provide a structured list of all datasets that were evaluated for data quality in this report. For each dataset, include basic identification information such as dataset name, source system, and data format.*

*The structural details of each dataset (tables, fields, and data types) are documented in the Data Dictionary Report (Task 2.2) and should not be duplicated here. This section serves only to confirm which datasets were included in the quality assessment.*

*The list of datasets should correspond to the datasets previously identified in the Data Inventory Report (Task 2.1).\]*

*\[**Example**:\]*

| Dataset Name | Source System | Data Format | Reference |
| :---- | :---- | :---- | :---- |
| ***\[Dataset name\]*** | *\[Origin system or platform\]* | *\[Table / CSV / API / etc.\]* | *\[Data Dictionary Report\]* |
| ***\[Customer\_Demographics\]*** | *\[CRM System\]* | *\[Database Table\]* | *\[P02\_Data\_Dictionary\_Report\_T\]* |
| ***\[Banking\_Transactions\]*** | *\[Core Banking System\]* | *\[Database Table\]* | *\[P02\_Data\_Dictionary\_Report\_T\]* |
| ***\[Call\_Center\_Interactions\]*** | *\[Call Center Platform\]* | *\[CSV File\]* | *\[P02\_Data\_Dictionary\_Report\_T\]* |

*\[These datasets were identified during Task 2.1 Collect Initial Data and structurally documented in the Data Dictionary Report (Task 2.2). The present report evaluates the quality of these datasets to determine their suitability for subsequent analytical tasks.\]*

4. # Data Quality Assessment Framework {#data-quality-assessment-framework}

*\[Define the methodological framework used to evaluate the quality of the datasets included in this report. This section explains the data quality dimensions and validation checks applied during the verification process in CRISP-DM Task 2.4  **Verify Data Quality.**\]*

*\[Describe the data quality dimensions used to assess the datasets. These dimensions represent commonly accepted criteria for evaluating the reliability and usability of data in analytical and machine learning projects.*

*For each dimension, provide a short definition and indicate the types of validation checks or indicators used during the assessment.*

*The purpose of this section is to clarify **how data quality is evaluated**, while the actual results of the evaluation are presented in the subsequent sections of the report.*

*Use a structured table to document the data quality dimensions and their corresponding validation checks.\]*

*\[see Data Quality Dimensions in table below:\]*

| Data Quality Dimension | Description | Typical Validation Checks | Example Indicator |
| :---- | :---- | :---- | :---- |
| **\[Completeness\]** | \[Degree to which required data fields contain values\] | \[Missing value analysis\] | *\[Percentage of null values per field\]* |
| **\[Validity\]** | \[Conformance of data values to expected formats or allowed domains\] | \[Range checks, format validation\] | *\[Age between 18–100\]* |
| **\[Consistency\]** | \[Consistency of values across fields, datasets, or formats\] | \[Cross-field comparisons, format checks\] | *\[Date format mismatch\]* |
| **\[Uniqueness\]** | \[Absence of duplicate records representing the same entity\] | \[Duplicate key detection\] | *\[Duplicate Customer\_ID\]* |
| **\[Accuracy\]** | \[Degree to which data correctly represents real-world entities\] | \[Cross-source validation\] | *\[Address mismatch vs CRM\]* |
| **\[Timeliness\]** | \[Degree to which data is up-to-date and relevant for analysis\] | \[Data freshness checks\] | *\[Last update timestamp\]* |
| **\[Integrity\]** | \[Preservation of relationships and referential integrity between datasets\] | \[Foreign key validation, orphan record detection\] | *\[Transactions without valid Customer\_ID\]* |

*\[In addition to the quality dimensions defined above, the data quality verification process may involve several complementary validation approaches. These methods help identify structural anomalies, data integrity issues, and inconsistencies that may affect analytical reliability.*

*The specific techniques used may vary depending on dataset characteristics and project requirements.*

*Typical validation approaches include:*

* *Data Profiling \- Automated examination of dataset structure, value distributions, and completeness indicators to detect anomalies such as unexpected value ranges, high cardinality fields, or abnormal distributions.*  
* *Cross-Source Validation \- Comparison of equivalent attributes across multiple data sources to identify inconsistencies or discrepancies.*  
* *Rule-Based Validation \- Verification of data against logical or domain-specific rules (e.g., valid value ranges, required attributes, or structural constraints).*  
* *Freshness and Timeliness Checks \- Evaluation of data update frequency and recency to ensure that datasets are sufficiently current for analytical use.*

*Where applicable, project-specific data quality thresholds may be defined to determine acceptable levels of completeness, uniqueness, or validity.\]*

5. # Dataset-Level Quality Overview {#dataset-level-quality-overview}

*\[Provide a high-level summary of the data quality assessment results for each dataset included in the scope of this report. This section offers a consolidated view of key quality indicators at the dataset level, allowing readers to quickly identify potential issues that may require further investigation.\]*

*\[Summarize the overall data quality status for each dataset evaluated in this report. The objective is to provide an initial diagnostic overview before presenting the detailed field-level analysis in the following sections.*

*For each dataset, include basic metrics that indicate the general quality of the data, such as the number of records, the proportion of missing values, and the presence of duplicate records. Where appropriate, provide an overall qualitative assessment (e.g., Green / Yellow / Red) reflecting the dataset’s readiness for analytical use.*

*This section should present aggregated indicators only. Detailed analysis of individual fields and specific data quality issues should be documented in subsequent sections.\]*

*\[**Example**:\]*

| Attribute \\ Dataset | *\[Customer\_Demographics\]* | *\[Banking\_Transactions\]* | *\[Call\_Center\_Interactions\]* |
| :---- | :---- | :---- | :---- |
| **Number of Records** | *\[10,000\]* | *\[1,200,000\]* | *\[80,000\]* |
| **Missing Values (%)** | *\[2%\]* | *\[0.5%\]* | *\[8%\]* |
| **Duplicate Records (%)** | *\[0.3%\]* | *\[0%\]* | *\[0%\]* |
| **Overall Quality Status** | *\[Green\]* | *\[Green\]* | *\[Yellow\]* |
| **Notes** | *\[Minor missing values in optional fields\]* | *\[High data completeness\]* | *\[Missing values in Call\_Outcome field\]* |

*\[This overview indicates that most datasets demonstrate acceptable levels of completeness and uniqueness, although the Call Center dataset contains a higher proportion of missing values that will be analyzed further in the field-level assessment.\]*

6. # Field-Level Data Quality Assessment {#field-level-data-quality-assessment}

*\[Provide a detailed evaluation of data quality at the level of individual fields within the datasets included in the scope of this report. This section identifies specific attributes that may contain missing values, invalid entries, format inconsistencies, or other anomalies affecting analytical reliability.\]*

*\[Assess the quality of individual data fields across the datasets included in the data quality audit. The objective is to detect issues that may impact data usability during subsequent analytical tasks such as feature engineering and modeling.*

*For each field evaluated, document key indicators that describe its structural and statistical characteristics, including the presence of missing values, unexpected value distributions, or potential validity violations. Where applicable, reference the expected data types and value constraints defined in the Data Dictionary Report (Task 2.2).*

*This section should focus on observed quality characteristics, while the formal registration of detected problems and their impact should be documented in Section 7 \- Identified Data Quality Issues.\]*

*\[**Example:** This field-level assessment helps identify attributes that may require further validation or cleaning during Phase 3\. Data Preparation\]*

| Field Name | Data Type | Unique Values | Missing Values (%) | Validity Issues | Notes |
| :---- | :---- | :---- | :---- | :---- | :---- |
| ***Dataset Name : \[Customer\_Demographics\]*** |  |  |  |  |  |
| *\[Age\]* | *\[Integer\]* | *\[55\]* | *\[0%\]* | *\[Out-of-range values (\>100)\]* | *\[Likely data entry errors\]* |
| *\[Gender\]* | *\[Categorical\]* | *\[2\]* | *\[0%\]* | *\[None\]* | *\[Values consistent with dictionary\]* |
| *\[Email\]* | *\[String\]* | *\[9,500\]* | *\[5%\]* | *\[None\]* | *\[Missing values in optional field\]* |
| ***Dataset Name : \[Banking\_Transactions\]*** |  |  |  |  |  |
| *\[Transaction\_Amount\]* | *\[Float\]* | *\[25,000\]* | *\[0%\]* | *\[None\]* | *\[High-value outliers detected\]* |
| ***Dataset Name : \[Call\_Center\_Interactions\]*** |  |  |  |  |  |
| *\[Call\_Outcome\]* | *\[Categorical\]* | *\[4\]* | *\[8%\]* | *\[None\]* | *\[Missing values: incomplete logging\]* |

7. # Identified Data Quality Issues {#identified-data-quality-issues}

*\[Provide a consolidated register of data quality issues identified during the dataset-level and field-level assessments. This section formally documents specific problems detected in the data and evaluates their potential impact on analytical tasks.\]*

*\[List all significant data quality issues identified during the verification process. Each issue should be recorded as a separate entry with a unique identifier to ensure traceability and facilitate follow-up actions in subsequent phases of the project.*

*For each issue, document the dataset and field where the problem occurs, classify the type of issue according to the data quality dimensions defined in Section 4 – Data Quality Assessment Framework, and provide a brief description of the problem and its potential analytical impact.*

*Minor irregularities that do not materially affect analytical reliability may be summarized in the Notes column rather than registered as separate issues.\]*

*\[**Example**:The issues listed in this section represent the primary data quality risks identified during the verification process. Recommended mitigation actions are presented in Section 9  Recommended Data Cleaning Actions.\]* 

| Issue ID | Field Name | Issue Type | Description | Potential Impact |
| :---- | :---- | :---- | :---- | :---- |
| ***Dataset Name : \[Customer\_Demographics\]*** |  |  |  |  |
| *\[DQ-01\]* | *\[Email\]* | *\[Completeness\]* | *\[5% missing values\]* | *\[Limits segmentation by channel\]* |
| *\[DQ-02\]* | *\[Customer\_ID\]* | *\[Uniqueness\]* | *\[100 duplicate records\]* | *\[Risk of data leakage and distorted stats\]* |
| *\[DQ-03\]* | *\[Age\]* | *\[Validity\]* | *\[Values \> 100 detected\]* | *\[Affects demographic feature reliability\]* |
| ***Dataset Name : \[Call\_Center\_Interactions\]*** |  |  |  |  |
| *\[DQ-04\]* | *\[Call\_Outcome\]* | *\[Completeness\]* | *\[8% missing values\]* | *\[Reduces reliability of interaction signals\]* |

8. # Impact Assessment on Analytical Tasks {#impact-assessment-on-analytical-tasks}

*\[Evaluate how the identified data quality issues may affect subsequent analytical activities, including feature engineering, model training, and model evaluation. This section translates technical data quality findings into potential risks for analytical reliability.\]*

*\[Assess the potential analytical implications of the data quality issues documented in Section 7 – Identified Data Quality Issues. The purpose of this section is to determine whether the detected problems could influence the reliability, validity, or interpretability of analytical results.*

*For each relevant issue, describe how it may affect analytical tasks such as:*

* *feature construction and transformation*  
* *statistical analysis and exploratory modeling*  
* *training and evaluation of machine learning models*  
* *data splitting procedures (e.g., train/test leakage)*

*Where applicable, reference the corresponding Issue ID from Section 7 to maintain traceability between the identified problem and its analytical impact.*

*This section focuses on analytical risk assessment, while recommended mitigation actions are provided in Section 9  Recommended Data Cleaning Actions.\]*

*\[**Example**: This assessment helps prioritize data cleaning actions in the next phase of the project and ensures that potential analytical risks are addressed before model development begins.\]*

| Issue ID | Analytical Area Affected | Impact Description | Risk Level |
| :---- | :---- | :---- | :---- |
| ***\[DQ-01\]*** | *\[Feature Engineering\]* | *\[Missing email values reduce the reliability of communication channel features\]* | *\[Low\]* |
| ***\[DQ-02\]*** | *\[Modeling / Evaluation\]* | *\[Duplicate customer records may lead to data leakage between datasets\]* | *\[**High**\]* |
| ***\[DQ-03\]*** | *\[Feature Engineering\]* | *\[Out-of-range age values may distort demographic feature distributions\]* | *\[Medium\]* |
| ***\[DQ-04\]*** | *\[Feature Engineering\]* | *\[Missing call outcome values reduce the reliability of interaction indicators\]* | *\[Medium\]* |

*\[**Example:*** 

***Analytical Risk Interpretation*** 

*The assessment above highlights several important analytical risks associated with the identified data quality issues.*

***Critical Risk** \- Data Leakage (DQ-02)*

*Duplicate customer records represent a high-severity issue because they may violate the assumption of independence between training and test datasets. If duplicates appear in both partitions, model evaluation metrics may become artificially inflated, leading to overly optimistic performance estimates that may not generalize to new data.*

***Feature Reliability Risks** (DQ-03, DQ-04)*

*Issues classified as Medium risk indicate potential degradation of feature reliability. Invalid or missing values in demographic or interaction attributes may introduce noise into feature distributions, which can reduce model stability and predictive performance.*

*These observations help prioritize remediation actions that will be addressed during Phase 3\. Data Preparation.\]*

9. # Recommended Data Cleaning Actions {#recommended-data-cleaning-actions}

*\[Provide recommended actions to address the data quality issues identified in this report. This section outlines potential remediation approaches that can be implemented during CRISP-DM Phase 3\. Data Preparation to ensure that the datasets are suitable for reliable analytical modeling.\]*

*\[Document recommended data cleaning or correction actions corresponding to the issues listed in Section 7\.  Identified Data Quality Issues. Each recommendation should reference the relevant Issue ID to maintain traceability between detected problems and proposed remediation measures.*

*The purpose of this section is to guide data preparation activities by outlining appropriate corrective strategies, such as handling missing values, removing duplicate records, validating value ranges, or standardizing data formats.*

*Recommendations should remain conceptual and method-oriented, rather than describing detailed implementation procedures. The actual implementation of these actions will take place during Phase 3\. Data Preparation.\]*

*\[**Example**: These recommended actions represent potential remediation strategies that will be implemented and validated during Phase 3\. Data Preparation, prior to feature engineering and model training.\]*

| Issue ID | Recommended Action | Proposed Method | Notes |
| :---- | :---- | :---- | :---- |
| ***\[DQ-01\]*** | *\[Handle missing email values\]* | *\[Impute with placeholder or mark as "Unknown"\]* | *\[Email is optional; low impact on core modeling\]* |
| ***\[DQ-02\]*** | *\[Remove duplicate customer records\]* | *\[Deduplicate using Customer\_ID as primary key\]* | *\[Retain the most recent record (last update timestamp)\]* |
| ***\[DQ-03\]*** | *\[Filter invalid age values\]* | *\[Apply range validation (18–100); remove/correct\]* | *\[Likely data entry errors; protects age distribution\]* |
| ***\[DQ-04\]*** | *\[Address missing call outcomes\]* | *\[Impute or introduce "Unknown" category\]* | *\[Essential for consistent categorical encoding\]* |

10. # Data Quality Conclusion {#data-quality-conclusion}

*\[Provide a final summary of the overall data quality assessment and determine whether the datasets evaluated in this report are suitable for further analytical processing. This section consolidates the main findings of the data quality verification performed in CRISP-DM Task 2.4  Verify Data Quality.\]*

*\[Summarize the key conclusions derived from the data quality assessment. The objective is to provide a concise evaluation of whether the identified data quality issues materially affect the feasibility of subsequent analytical tasks.*

*The conclusion should reference the main findings from the previous sections, including the presence of missing values, duplicates, or validity issues, and indicate whether these problems can be addressed during Phase 3\. Data Preparation.*

*Where appropriate, assign an overall qualitative status indicating the readiness of the data for further processing. The conclusion should remain high-level and avoid repeating detailed issue descriptions already documented earlier in the report.\]*

*\[**Example**: Overall, the datasets included in this assessment are considered suitable for analytical use once the identified data quality issues are addressed during Phase 3\. Data Preparation. The recommended remediation actions documented in Section 9 will guide the necessary data cleaning and validation steps prior to model development.\]*

| Indicator | Assessment |
| :---- | :---- |
| **Overall Data Completeness** | *\[Most datasets demonstrate high completeness, with minor missing values in optional fields\]* |
| **Duplicate Records Risk** | *\[Limited number of duplicate customer records detected\]* |
| **Data Validity Issues** | *\[Some out-of-range values identified in demographic attributes\]* |
| **Overall Data Quality Status** | *\[**Yellow**\] \- one of \[Green / Yellow / Red\]\]* |
| **Readiness for Data Prep** | *\[Data is suitable for further preparation after recommended cleaning actions\] \- \[could be \[Suitable / Requires remediation before modeling\]\]* |
