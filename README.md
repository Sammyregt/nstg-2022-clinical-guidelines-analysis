# Nigeria Standard Treatment Guidelines (NSTG) 2022 Dataset - Nigeria Clinical Guidelines: Clinical Analysis

## Description
This dataset contains a comprehensive collection of clinical guidelines processed and merged from the **Nigeria Standard Treatment Guidelines (NSTG) 2022**. It provides structured medical information for healthcare professionals, researchers, and developers building clinical decision support systems for the Nigerian context.

The dataset includes over 250 conditions, ranging from infectious diseases and maternal health to chronic non-communicable diseases.

-------------------------------------------------------------------------

## Overview
A comprehensive bioinformatics and clinical analysis of the
Nigeria Standard Treatment Guidelines (NSTG) 2022 — covering 270 conditions
across 20 disease categories, published by Nigeria's Federal Ministry of Health

## Key Findings
- 84.8% of the guideline covers non-communicable diseases — evidence of Nigeria's epidemiological transition
- Amoxicillin is the most broadly used drug (26 conditions, 9.6% of all conditions)
- Only 57.4% of conditions have documented prevention strategies — a critical policy gap
- Geriatric care has only 3 conditions despite Nigeria's ageing population

## Tools & Techniques
Python · pandas · scikit-learn · NetworkX · WordCloud · Matplotlib · Power BI

## Repository Structure
nstg_outputs/        → 10 publication-quality charts

nstg_powerbi_exports/           → 10 cleaned CSV exports for Power BI

nstg_analysis.ipynb        → Jupyter notebook with markdown inferences

NSTG_Dashboard.pbix        → Interactive Power BI dashboard (open with free Power BI Desktop)

## Setup Instructions
1. Create a Virtual Environment

    `python -m venv venv`

2. Activate the Virtual Environment
    - Windows
        `venv\\Scripts\\activate`
    - Mac/Linux
        `source venv/bin/activate`
3. Install Project Requirements
    `pip install -r requirements.txt`
4. Launch Jupyter Notebook
    `jupyter notebook`

Open and start working on:

`nstg_analysis.ipynb`

----------------------------------------------------------------

## Files Included and Format
- **File:** `nigeria_clinical_guidelines_2022.json`
- **Format:** JSON Array (UTF-8 Encoded)
- **Status:** Validated, Merged, and Cleaned.

## Variables and Schema
Each condition object in the array contains the following fields:

| Field Name | Type | Description |
|------------|------|-------------|
| `condition_name` | String | The official name of the medical condition (e.g., "Abortion"). |
| `condition_slug` | String | A URL-friendly identifier for the condition. |
| `source` | String | The clinical source document (NSTG 2022). |
| `introduction` | String | An overview of the disease/condition pathology and prevalence. |
| `clinical_features` | List (Objects) | Symptoms and signs categorized by type (e.g., "General", "Symptomatic"). |
| `investigations` | List (Strings) | Recommended laboratory and radiological tests. |
| `treatment` | Object | Structured therapeutic advice split into `goals`, `non_drug`, and `drug` measures. |
| `differential_diagnoses` | List (Strings) | Alternative medical conditions with similar presentations. |
| `complications` | List (Strings) | Potential negative outcomes if left untreated. |
| `prevention` | List (Strings) | Methods for avoiding the condition or its hazards. |
| `prognosis` | String/Null | Expected outcome of the treatment. |

## License and Source
- **Source:** Nigeria Federal Ministry of Health, Nigeria Standard Treatment Guidelines (NSTG) 2022.
- **License:** Creative Commons Attribution 4.0 International (CC BY 4.0).

---
**Prepared by:** Anda Usman / Datum Africa (Data Outreach Team)
**Date:** April 2026

**Data Source & Citation:**
Chisom Rutherford (2026). *NSTG Nigeria Treatment Guidelines Dataset*. Datum Africa.
https://datum.africa/datasets/nstg-nigeria-treatment-guidelines-dataset


### © [Adeoye Samuel] 2026 · CC BY 4.0
### Original analysis of NSTG 2022 — Nigeria Standard Treatment Guidelines
### Repository: https://github.com/Sammyregt/
### Cite as: [Adeoye] (2026). NSTG 2022 Clinical Guidelines Analysis.
### GitHub. https://github.com/Sammyregt/nstg-2022-clinical-guidelines-analysis.git
