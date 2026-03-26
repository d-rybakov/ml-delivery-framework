# ML Delivery Framework

Artifact-driven ML delivery framework based on CRISP-DM.

## Problem

As data science teams scale, delivery tends to fragment:

- workflows diverge across initiatives  
- milestone expectations become implicit  
- the definition of "done" varies by project  

The bottleneck is not technical capability - it is lack of structure.

## Solution

This framework transforms CRISP-DM from a modeling methodology into a structured delivery system.

Key principles:

- CRISP-DM phases define explicit outputs  
- Outputs are formalized as artifacts  
- Artifacts serve as review and control checkpoints  
- Checkpoints enable predictable and controlled delivery  
- The lifecycle remains iterative and adaptable to project complexity  

## Documentation Architecture

Each artifact is classified by governance level:

| Level | Type                     | Description                                                  |
|------|--------------------------|--------------------------------------------------------------|
| G    | Governance Artifacts     | Formal documents requiring approval and version control      |
| T    | Technical Artifacts      | Structured technical documentation ensuring reproducibility  |
| L    | Logs & Checklists        | Operational tracking artifacts supporting execution          |

This structure ensures:

- clear ownership and accountability  
- traceability of decisions and transformations  
- separation between governance and execution layers

## Example Context

All examples in this repository are based on a fictional **Customer Churn Prediction** project.

The examples are:

- illustrative, not production scenarios  
- intentionally independent across documents  
- designed to demonstrate how templates should be completed  

## Notes on Template Usage

Text in square brackets `[ ... ]` represents guidance for completing the document, including:

- intent of the section  
- instructions for writing content  
- illustrative examples  

In actual project usage, these sections are replaced with real content.

## Framework Structure

The framework follows CRISP-DM phases:

- [Phase 1 - Business Understanding  ](./phase-1-business-understanding/)
- [Phase 2 - Data Understanding  ](./phase-2-data-understanding/)
- [Phase 3 - Data Preparation  ](./phase-3-data-preparation/)
- [Phase 4 - Modeling  ](./phase-4-modeling/)
- [Phase 5 - Evaluation ](./phase-5-evaluation/)
- [Phase 6 - Deployment  ](./phase-6-deployment/)

Each phase contains:

- structured deliverables  
- task-to-artifact mapping  
- documentation templates  

## Positioning

This framework is designed as:

- a delivery backbone for Data Science teams  
- a governance layer for ML lifecycle management  
- a reference model for reproducible ML workflows  

It can be adapted to:

- different team sizes and maturity levels  
- varying project complexity  
- integration with MLOps tooling  

## Status

Initial version.  
The framework is being progressively expanded with templates and examples.

## Author

Dmitry Rybakov  
Data / AI Delivery

## References

Based on the [original CRISP-DM](https://web.archive.org/web/20220401041957/https://www.the-modeling-agency.com/crisp-dm.pdf) framework  
(Chapman et al., 2000).

Adapted for structured ML delivery and practical implementation.  

## Additional Resources

Full template set with detailed guidance and examples is available in Google Drive.

<link>
