# H1 — Nigeria Health-Facility Service Delivery Assessment

## Project status

**Stage:** Project structure established  
**Dataset:** To be obtained and verified  
**Analysis:** Not yet started

## Research focus

This project will examine selected dimensions of health-facility service delivery in Nigeria using the World Bank Service Delivery Indicators (SDI) health survey data.

The analysis will be guided by the variables and coverage actually available in the downloaded dataset and its documentation. Potential areas of investigation include facility readiness, staffing, availability of essential resources, and measures of provider knowledge or clinical competence where the relevant modules support them.

## Proposed research objective

To assess selected dimensions of health-facility readiness and service-delivery capacity in Nigeria using the available SDI health survey evidence.

## Initial research questions

These are provisional questions. They will be refined after reviewing the questionnaire, codebook, sampling documentation, and actual data files.

1. What does the survey measure about health-facility readiness and service delivery?
2. What patterns are visible in the availability of selected staff, equipment, medicines, and basic facility resources?
3. How do the measured indicators vary across facility types or locations, where the dataset supports these comparisons?
4. What limitations should be considered when interpreting the results?

## Data source

Planned source: World Bank Service Delivery Indicators (SDI), Nigeria health survey, 2013–2014.

The exact dataset files, modules, survey coverage, sample design, and usage conditions must be verified against the official catalogue and accompanying documentation before analysis begins.

## Unit of analysis

The primary unit is expected to be the health facility for facility-level measures. Some modules may have other units of observation, such as health workers or patient observations. The unit will be specified separately for each analysis.

## Project workflow

1. Obtain the official data and documentation.
2. Inventory the files and identify the relevant modules.
3. Read the questionnaire, codebook, sampling information, and data-use conditions.
4. Establish the units of analysis and linkable identifiers, if any.
5. Assess data quality and missingness.
6. Prepare analysis-ready datasets without losing the original raw files.
7. Define and calculate indicators transparently.
8. Analyse and visualise the evidence.
9. Document findings, limitations, and recommendations.

## Repository structure

- `data/raw/` — original downloaded files; not committed unless permitted and appropriate.
- `data/processed/` — documented, analysis-ready datasets; only publish if permitted.
- `documentation/` — source notes, questionnaires, codebooks, methodology, and data dictionary.
- `scripts/` — reproducible cleaning and analysis code.
- `analysis/` — research questions, analytical notes, and interpretation.
- `outputs/` — charts, tables, and report materials.

## Research integrity

- Do not upload restricted, confidential, or personally identifiable data.
- Preserve original data unchanged.
- Cite the official data source and comply with its terms of use.
- Do not infer causality from descriptive comparisons.
- Clearly distinguish measured indicators from interpretation.
- Do not report findings until the data have been obtained, checked, and analysed.

## Current next action

Obtain the official Nigeria SDI health data package and its supporting documentation, then verify the contents before selecting variables or writing analysis code.
