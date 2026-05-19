# Nigeria Standard Treatment Guidelines (NSTG) 2022 Dataset

## Description
This dataset contains a comprehensive collection of clinical guidelines processed and merged from the **Nigeria Standard Treatment Guidelines (NSTG) 2022**. It provides structured medical information for healthcare professionals, researchers, and developers building clinical decision support systems for the Nigerian context.

The dataset includes over 250 conditions, ranging from infectious diseases and maternal health to chronic non-communicable diseases.

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