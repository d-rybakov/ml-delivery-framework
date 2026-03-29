# P01_Situation_Assessment_Report_G  
Document Name: **Situation Assessment Report**

---
## Document Information

| Field | Value |
|------|------|
| Project Name | *\[e.g. Customer Churn Prediction\]* |
| Project Code | *\[e.g. CCP-2025-01\]* |
| CRISP-DM Phase | P01 - Business Understanding |
| Artifact Level | G - Governance Artifact |
| Document Owner (Role) | *\[Business Analyst \| Product Owner\]* |
| Version | *\[0.0.1\]* |
| Last Updated | *\[DD Month YYYY\]* |
| Document Status | *\[Draft \| In Review \| Approved\]* |

---

Working version: [Google Docs template](https://cutt.ly/otPgdpeK)

---
## Revision History

| Version | Initials | Position | Date | Comments / Description of Changes |
| :---- | :---- | :---- | :---- | :---- |
| *0.1* |  |  |  |  |
| *0.2* |  |  |  |  |
| *0.3* |  |  |  |  |
| *0.4* |  |  |  |  |
| *0.5* |  |  |  |  |

---

## Approval and Sign-Off

| Position | Name | Signature | Date |
| :---- | :---- | :---- | :---- |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |
|  |  |  |  |

---

# Introduction

*\[Provide a high-level introduction to the document, explaining its role within the CRISP-DM process and its purpose in supporting situation assessment before solution design.\]*

*\[Briefly position the document within Phase 1 (Business Understanding), specifically Task 1.2 (Assess Situation).*

*Clarify that the document consolidates key assessment dimensions required to evaluate feasibility and readiness.*

*Avoid duplicating detailed content from core sections.\]*

*\[**Example:** This document presents a structured assessment of the current situation surrounding the identified business problem.*

*It is developed as part of the CRISP-DM Business Understanding phase and supports informed decision-making prior to project planning and modeling activities.\]*

## Purpose

*\[Define the specific purpose of this document as an assessment artifact supporting early-stage decision-making.\]*  
*\[Clearly state what the document is intended to achieve, focusing on its role in:*

* *evaluating feasibility*  
* *identifying constraints and dependencies*  
* *supporting go/no-go and prioritization decisions*

*Do not restate the full CRISP-DM process.\]*  
*\[**Example**: The purpose of this document is to assess the organizational, technical, and data-related conditions relevant to the initiative.*  
*It provides a structured foundation for determining whether the project is feasible and how it should be approached at a high level.\]*

## Audience

*\[Identify the primary stakeholders who will use or rely on this document.\]*

*\[List key audience groups and describe how they use the document.*

*Focus on decision-makers and contributors involved in early project stages.\]*

*\[**Example**: This document is intended for business stakeholders, project sponsors, business analysts, data scientists, and technical leads.*  
*It supports decision-making, alignment, and preparation for subsequent project planning activities.\]*

## Definitions, Acronyms, and Abbreviations

*\[This subsection provides the definitions of all terms, acronyms, and abbreviations required to properly interpret the document. This information may be provided by reference to the project’s Glossary.\]*

| # | Term | Explanation |
|-----|:----|:----|
| 1. | *\[Constraint\]* | *\[A limitation that restricts possible approaches or solutions.\]* |
| 2. | *\[Assumption\]* | *\[A limitation that restricts possible approaches or solutions.\]* |
| 3. | *\[Dependency\]* | *\[An external or internal element required for the initiative to proceed.\]* |
| 4. |  |  |
| 5. |  |  |
| 6 |  |  |
| 7. |  |  |

## Document Overview

*\[Provide a structured overview of the document’s contents to guide the reader.\]*

*\[Summarize the main sections and their purpose in a logical flow.*

*Focus on navigation and comprehension rather than repeating section content.\]*

*\[**Example**: The document is structured as follows:*

*Section [Resource Inventory](#resource-inventory) provides an overview of available resources, including human, data, and technical assets.*

*Section [Requirements, Assumptions, and Constraints](#requirements-assumptions-and-constraints) outlines key requirements, assumptions, and constraints shaping the initiative.*

*Section [Cost-Benefit Overview](#cost-benefit-overview) presents a high-level cost-benefit perspective.*

*Section [Dependencies and External Factors](#dependencies-and-external-factors) identifies dependencies and external factors influencing the project context.\]*

# References

*\[This section contains links to all other places that were referred to in this document. These may include:*

* *Documents on shared document control systems (such as SharePoint)*

* *Web sites*

* *URLs or network locations\]*

| # | Document | Explanation |
|-----|:----|:----|
| 1. | *\[[P01_Stakeholder_Analysis_G](./P01_Stakeholder_Analysis_G.md)\]* | *\[Identifies key stakeholders, their roles, and engagement strategies.\]* |
| 2. | *\[[P01_Risk_Assessment_G](./P01_Risk_Assessment_G.md)\]* | *\[Documents project risks, their impact, and mitigation plans.\]* |
| 3. | *\[[P01_Business_Problem_Statement_G](./P01_Business_Problem_Statement_G.md)\]* | *\[Defines the business context, problem, and intended outcomes.\]* |
| 4. | *\[Enterprise Data Governance Policy\]* | *\[Defines rules and constraints for data usage and access.\]* |
| 5. |  |  |
| 6 |  |  |
| 7. |  |  |


# Resource Inventory

*\[Provide a structured overview of all resources available to support the initiative, ensuring visibility into what can realistically be leveraged at the current stage.\]*

*\[Identify and categorize available resources across people, data, infrastructure, and tools.*

*Focus on availability, accessibility, and ownership.*

*Do NOT include:*

* *detailed capability assessment (covered later in Modeling/Data phases)*  
* *cost estimation (covered in Section 5\)*  
* *project allocation or scheduling (covered in Project Plan)\]*

*\[**Example**: The initiative is supported by cross-functional teams, existing enterprise data sources, and a cloud-based analytics platform already used for reporting and analysis.\]*

## Human Resources

*\[Identify the human roles and expertise available to support the initiative.\]*

*\[List key roles, their functional areas, and level of involvement (e.g., advisory, operational).*

*Focus on availability and relevance.*

*Do NOT include:*

* *detailed responsibility matrices (RACI)*  
* *resource allocation over time\]*

*\[**Example**: The initiative involves business analysts from the Customer Management team, data scientists from the Analytics department, and IT engineers responsible for data access and infrastructure support.\]*

## Data Resources

*\[Identify data sources that may be used to support analysis and solution development.\]*

*\[Describe available data sources, including:*

* *system of origin*  
* *data type and scope*  
* *access method and ownership*

*Do NOT include:*

* *data quality assessment*  
* *feature engineering details*  
* *data preparation steps\]*

*\[**Example:** Customer data is available from the CRM system and enterprise data warehouse, including transaction history, account status, and interaction records.\]*

## Infrastructure

*\[Describe the technical environments available for data storage, processing, and analysis.\]*

*\[Identify platforms, environments, and processing capabilities.*

*Do NOT include:*

* *architecture design decisions*  
* *scalability planning*  
* *performance benchmarking\]*

*\[**Example**: The organization uses a cloud-based data platform that supports distributed data processing and secure access to enterprise datasets.\]*

## Tools and Software

*\[Identify tools and software available for analysis, development, and collaboration.\]*

*\[List relevant tools used for:*

* *data analysis*  
* *model development*  
* *reporting and collaboration*

*Do NOT include:*

* *tool selection justification*  
* *comparison of alternative tools\]*

*\[**Example**: Python and SQL are used for data analysis, while BI tools support reporting and visualization. Collaboration is managed through shared documentation platforms.\]*

# Requirements, Assumptions, and Constraints

*\[Define the key conditions that shape the feasibility and direction of the initiative.\]*

*\[Structure all conditions into requirements, assumptions, and constraints.*

*Do NOT include:*

* *solution design decisions*  
* *implementation plans*  
* *detailed risk descriptions (covered in Risk Assessment)\]*

*\[**Example**: The initiative must comply with internal governance standards, relies on assumed data availability, and is constrained by infrastructure limitations.\]*

## Business Requirements

*\[Define expectations from a business perspective that the initiative must satisfy.\]*

*\[Capture requirements related to:*

* *business usability*  
* *decision-making support*  
* *interpretability*  
* *alignment with business processes*

*Do NOT include technical implementation details\]*

*\[**Example**: The solution must provide interpretable outputs that business users can act upon to support customer retention decisions.\]*

## Technical Requirements

*\[Define expectations related to technical feasibility, integration, and compliance.\]*

*\[Document requirements such as:*

* *system compatibility*  
* *data security and governance*  
* *integration constraints*  
* *performance expectations (high-level)*

*Do NOT include:*

* *architecture design*  
* *specific technologies to be selected\]*

*\[**Example**:  The solution must integrate with existing data platforms and comply with internal data security policies.\]*

## Assumptions

*\[Capture assumptions that influence project feasibility and direction.\]*

*\[List assumptions explicitly and ensure they are distinguishable from facts.*

*Do NOT include:*

* *validated findings*  
* *risks (uncertainties with impact \-\> Risk document)\]*

*\[**Example**: It is assumed that historical customer behavior is indicative of future churn patterns.\]*

## Constraints

*\[Identify limitations that restrict possible approaches or solutions.\]*

*\[Document constraints related to:*

* *data*  
* *resources*  
* *technology*  
* *regulations*

*Do NOT include:*

* *risks or uncertainties*  
* *future mitigation strategies\]*

*\[**Example**: Customer data must be anonymized, limiting the use of personally identifiable information in analysis.\]*

# Cost-Benefit Overview

*\[Provide a high-level economic perspective on the initiative to support early decision-making.\]*

*\[Assess costs and benefits at a conceptual level.*

*Do NOT include:*

* *detailed financial modeling*  
* *budgeting or funding approvals*  
* *ROI calculations requiring precise data\]*

*\[**Example**: The initiative is expected to deliver meaningful business value relative to moderate implementation effort.\]*

## Cost Drivers

*\[Identify the main sources of cost associated with the initiative.\]*

*\[Describe major cost components such as:*

* *human effort*  
* *infrastructure usage*  
* *data preparation*

*Do NOT include:*

* *exact cost figures (unless readily available)*  
* *financial planning details\]*

*\[**Example**: Primary cost drivers include data preparation effort, model development, and infrastructure usage.\]*

## Expected Benefits

*\[Describe the anticipated business value generated by the initiative.\]*

*\[Capture benefits such as:*

* *revenue improvement*  
* *cost reduction*  
* *efficiency gains*  
* *decision quality improvements*

*Do NOT include:*

* *quantified KPIs (covered in Business Objectives)*  
* *speculative or ungrounded claims\]*

*\[**Example:** Improved churn prediction is expected to enhance retention strategies and reduce customer acquisition costs.\]*

## Cost-Benefit Assessment

*\[Evaluate whether expected benefits justify the anticipated effort and cost.\]*

*\[Provide a qualitative assessment:*

* *relative scale (low/medium/high)*  
* *key value drivers*  
* *uncertainty factors*

*Do NOT include:*

* *detailed ROI calculations*  
* *financial approval decisions\]*

*\[**Example**: The initiative is assessed as high-impact with moderate effort, making it a strong candidate for implementation despite some uncertainty in data quality.\]*

# Dependencies and External Factors

*\[Identify external and organizational elements that influence the initiative but are not fully controlled within it.\]*

*\[Structure dependencies clearly and separate them from risks.*

*Do NOT include:*

* *risk descriptions*  
* *mitigation strategies*  
* *project scheduling dependencies\]*

*\[**Example**: The initiative depends on data availability and organizational collaboration across multiple teams.\]*

## Internal Dependencies

*\[Identify dependencies within the organization that may affect the initiative.\]*

*\[Document dependencies on:*

* *internal systems*  
* *teams*  
* *processes*

*Do NOT include:*

* *stakeholder analysis details*  
* *responsibilities\]*

*\[**Example**: The initiative depends on data access provided by the IT department and collaboration with the CRM team.\]*

## External Dependencies

*\[Identify dependencies on external entities or providers.\]*

*\[Include dependencies such as:*

* *third-party data providers*  
* *external vendors*  
* *regulatory bodies*

*Do NOT include:*

* *contractual details*  
* *risk evaluations\]*

*\[**Example**: The initiative relies on external demographic data providers to enrich customer profiles.\]*

## External Factors

*\[Identify external conditions that may influence the initiative without being direct dependencies.\]*

*\[Describe influencing factors such as:*

* *market trends*  
* *customer behavior shifts*  
* *regulatory changes*

*Do NOT include:*

* *speculative risks*  
* *internal organizational issues\]*

*\[**Example**: Customer churn behavior may be influenced by macroeconomic conditions and competitive market offerings.\]*
