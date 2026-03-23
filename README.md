# Reproducible R Pipeline for Standardizing Clinical Phenotype Data for dbGaP

A fully reproducible R workflow for cleaning, harmonizing, anonymizing, and formatting clinical phenotype data for dbGaP submission.

---

## Project Overview

This project focuses on transforming raw phenotype datasets into standardized, dbGaP-compliant formats.

- Differentiates subject-level and sample-level data  
- Performs systematic data cleaning and validation  
- Resolves duplicate entries and data inconsistencies  
- Implements two-step de-identification for participant and sample IDs  
- Produces submission-ready datasets and comprehensive data dictionaries  

All operations are implemented programmatically using tidyverse workflows to ensure reproducibility and scalability.

---

## Key Features

### Data Import and Cleaning
- Loads Excel-based phenotype tables and associated data dictionaries  
- Standardizes missing values and harmonizes variable formats  

### Data Transformation
- Aligns variables with the data dictionary structure  
- Separates subject-level and sample-level datasets  

### Data Quality Control
- Detects duplicate subjects and samples  
- Corrects inconsistent categorical and numeric entries  

### De-identification Pipeline
- Generates randomized, dbGaP-compliant subject and sample IDs  
- Implements two-step anonymization to protect participant privacy  

### Data Integration
- Incorporates external key files while preserving referential integrity  
- Ensures consistency across all datasets  

### Feature Engineering
- Aggregates repeated measurements (e.g., average gestational age)  
- Creates derived variables required for dbGaP submission  

### dbGaP File Generation
- Subject-level phenotype dataset (DS)  
- Subject-sample mapping file (SSM)  
- Data dictionary (DD) with correctly formatted VALUE fields  

### Visualization
- Interactive Plotly visualizations for exploring phenotype relationships  
- Customizable tooltips for easy data inspection  

---

## Technologies Used
- R  
- tidyverse (dplyr, tidyr, ggplot2)  
- readxl  
- here  
- plotly  
- dbGaPCheckup  
- openxlsx  

---

## Outputs

The workflow produces dbGaP-ready files:

- `5a_SubjectPhenotypes_DS.txt`  
- `5b_SubjectPhenotypes_DD.xlsx`  
- `3a_SSM_DS.txt`  
- `subjectKey.txt`  
- `sampleKey.txt`  

---

## Reproducibility

- No manual editing of source data  
- Uses `here` for portable, project-relative paths  
- Fully script-based for seamless reruns on updated datasets  

---

## Key Skills Demonstrated

- Advanced data wrangling and transformation (tidyverse)  
- Clinical and genomic data standardization  
- Reproducible research practices  
- Comprehensive data validation and QC  
- Pipeline development in R  
- dbGaP submission preparation  

---

## Notes

This pipeline was developed as an academic exercise simulating real-world workflows for genomic data submission.

---

## Author

**Gagan Heda**
