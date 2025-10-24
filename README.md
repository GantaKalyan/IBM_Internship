# Classifying PMGSY Scheme using AutoAI in Watsonx.ai
 This repository contains a Jupyter Notebook–driven machine learning project that classifies PMGSY projects into the correct scheme (PMGSY‑I, PMGSY‑II, RCPLWEA) using IBM Watsonx.ai AutoAI and IBM Cloud services.​
The work was completed as part of the IBM SkillsBuild internship program focused on skills‑based, career‑aligned learning pathways and applied projects.​

# Overview
- PMGSY is a national rural road connectivity program, and efficient classification of projects across phases helps monitoring, budgeting, and governance at scale.​

- The solution uses Watsonx.ai AutoAI to automate model selection and optimization, with deployment via IBM Cloud’s Watson Machine Learning for real‑time or batch inference workflows.​

- The artifacts follow an internship‑grade, reproducible ML workflow organized in Jupyter Notebooks within this repository.​​

# Problem statement
- Large volumes of PMGSY projects spanning multiple phases require consistent categorization, which is time‑consuming and error‑prone if done manually.​

- Automating the scheme classification improves operational efficiency and supports planning tools with data‑driven consistency.​

# Dataset
- Source: PMGSY dataset prepared for internship tasks with typical project attributes used for supervised learning.​

- Key fields typically include sanctioned amount, estimated cost, length, structure type, and district information, with PMGSY_SCHEME as the target label.​

# Methods
- AutoAI handles preprocessing, encoding, imputation, and feature engineering while exploring multiple modeling pipelines automatically.​

- Candidate models (e.g., Gradient Boosting, Logistic Regression, XGBoost, Random Forest) are ranked using cross‑validation on metrics such as Accuracy, F1‑score, and ROC‑AUC to select the best pipeline.​

# IBM stack
- Watsonx.ai AutoAI for automated model generation, selection, and experiment tracking.​

- Watson Studio for dataset management and experiment orchestration in a notebook‑friendly environment.​

- Watson Machine Learning to deploy the best pipeline as a REST endpoint for integration with external systems.​

# Repository structure
Jupyter Notebooks constitute the primary artifacts for data preparation, AutoAI experiments, model review, and deployment handoff notes.​​

# Getting started
- Upload the PMGSY dataset to Watson Studio within the Watsonx.ai environment and confirm PMGSY_SCHEME as the target column for classification.​

- Run an AutoAI experiment, reviewing leaderboards for top pipelines using Accuracy, F1‑score, and ROC‑AUC to guide selection.​

- Save the top pipeline and deploy it to Watson Machine Learning as a REST API for real‑time or batch scoring use cases.​

# Usage
- Notebook cells include steps to load data, configure AutoAI, train and compare pipelines, export the winning model, and note deployment parameters for inference.​

- After deployment, send feature payloads to the REST endpoint to obtain predicted scheme labels for each project record.​

# Evaluation
- AutoAI provides cross‑validated metrics, confusion matrix, and feature importance to assess model quality and interpret drivers of predictions.​

- The final pipeline demonstrated strong accuracy in differentiating schemes, suitable for operational tagging and validation workflows.​

# Results
- The experiment outcomes indicate high‑quality classification performance, with leaderboard metrics and artifacts available from the AutoAI run for auditability.​

- Feature importance highlights financially and physically meaningful attributes informing the scheme decision boundary.​

# Credits
- This project was executed as part of the IBM SkillsBuild internship, a free skills‑based learning initiative that offers structured modules, badges, and applied projects for learners.​

- Acknowledgement to program collaborators and delivery partners, including AICTE and the Edunet Foundation, for enabling access, mentorship, and hands‑on learning during the internship.​

Thanks to the IBM SkillsBuild learning platform for resources, pathways, and digital credentials that supported the development of this work.​

# Future work
- Add model explainability reports and governance notes to improve transparency of scheme assignments in production settings.​

- Incorporate geospatial and temporal features to capture regional and time‑based variability for potential performance gains.​

- Integrate the API with data entry dashboards to enable real‑time tagging of new PMGSY records and batch validation of existing datasets.​

# Author
#### Ganta Kalyan, JNTU College of Engineering Kakinada, Structural Engineering (M.Tech), internship project contributor.​
