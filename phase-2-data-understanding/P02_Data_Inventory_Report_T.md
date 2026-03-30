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

## Definitions, Acronyms, and Abbreviations {#definitions-acronyms-and-abbreviations}

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
| 1. | *\[[P01_Project_Plan_G](./P01_Project_Plan_G.md)\]* | *\[Defines business objectives and analytical scope for churn prediction.\]* |
| 2. | *\[Enterprise Data Catalog\]* | *\[Source metadata repository for CRM tables.\]* |
| 3. |  |  |
| 4. |  |  |
| 5. |  |  |
| 6 |  |  |
| 7. |  |  |

