# Phase 4 - Modeling

## Overview

The **Modeling phase** focuses on developing, training, and evaluating candidate models to solve the defined analytical task.

Its purpose is to:
- select appropriate modeling techniques  
- design validation strategy  
- train candidate models  
- evaluate model performance  
- document model behavior and configuration  

In this framework, Phase 4 acts as a **model development and evaluation layer**, ensuring that model selection is structured, reproducible, and aligned with predefined success criteria.

---

## Key Outcomes

By the end of this phase, the project must have:

- Developed and documented **candidate models**  
- Defined and applied a **model validation strategy**  
- Recorded **model evaluation results**  
- Selected a **final model based on evaluation results**  
- Documented **model configuration and training parameters**  

This ensures that the selected model is **validated, reproducible, and ready for formal evaluation**.

---

## CRISP-DM Task Mapping

| CRISP-DM Task | Deliverables |
|--------------|-------------|
| 4.1 Select Modeling Techniques | P04_Model_Selection_Report_T |
| 4.2 Generate Test Design | P04_Model_Validation_Design_T |
| 4.3 Build Models | Trained Models, P04_Model_Training_Specification_T, P04_Model_Description_Report_T |
| 4.4 Assess Models | P04_Model_Evaluation_Report_T, P04_Hyperparameter_Tuning_Log_L |

---

## Deliverables in This Phase

### Technical Artifacts (Level T)

These documents define modeling logic, evaluation approach, and ensure reproducibility.

- **P04_Model_Selection_Report_T**  
  Documents selected modeling approaches and rationale.

- **P04_Model_Validation_Design_T**  
  Defines validation methodology, datasets, and evaluation approach.

- **P04_Model_Training_Specification_T**  
  Specifies training process, parameters, and configurations.

- **P04_Model_Description_Report_T**  
  Describes model structure, features used, and behavior.

- **P04_Model_Evaluation_Report_T**  
  Provides comparative analysis of model performance.

---

### Logs & Checklists (Level L)

These artifacts track experimentation and tuning processes.

- **P04_Hyperparameter_Tuning_Log_L**  
  Records hyperparameter experiments and tuning results.

---

### Model Artifacts

- **Trained Models**  
  Set of trained candidate models evaluated during the phase.

---

## How This Phase Works

This phase operationalizes model development through structured experimentation and evaluation by:

- selecting appropriate modeling techniques aligned with analytical goals  
- defining validation strategy to ensure objective comparison  
- training multiple candidate models  
- tracking experiments and hyperparameter tuning  
- evaluating models using consistent metrics and datasets  

The separation of **model definition, training, and evaluation artifacts** ensures that:

- model selection is transparent  
- experiments are reproducible  
- decisions are evidence-based  

---

## Phase Gate

The phase is completed only after both conditions are met:

### 1. Outcome Validation

All key outcomes of the phase are achieved (see [**Key Outcomes**](#key-outcomes) section).

### 2. Model Readiness and Approval

- Candidate models are developed and documented  
- Model evaluation results are formally recorded  
- The selected model:
  - meets predefined success criteria  
  - is justified based on evaluation results  
- Model configuration and training parameters are finalized  

A formal decision is made to proceed to:  
**Phase 5 — Evaluation**

---

## Related Phases

Next: [Phase 5 - Evaluation](../phase-5-evaluation/)  
Previous: [Phase 3 - Data Preparation](../phase-3-data-preparation/)  
Full framework: [README](../README.md)
