# H1 Data Source Register and Initial File Inventory

## Official study

**Study:** Nigeria — Service Delivery Indicators Health Survey 2013, Harmonized Public Use Data  
**Survey period:** 2013–2014  
**Reference ID:** NGA_2013_SDI-H_v01_M_v02_A_PUF  
**DOI:** https://doi.org/10.48529/qz7v-4r76  
**Official catalogue:** https://microdata.worldbank.org/catalog/2559  
**Data dictionary:** https://microdata.worldbank.org/catalog/2559/data-dictionary  
**Related documentation:** https://microdata.worldbank.org/catalog/2559/related-materials  
**World Bank SDI health overview:** https://www.worldbank.org/en/programs/service-delivery-indicators/health

The World Bank Data Catalog reports that the survey visited 2,385 health facilities across 12 of Nigeria's 36 states between July 2013 and January 2014. It describes the data as representative at the state level. The study is public-use data under the World Bank Research Data License; review the current terms before redistribution.

## Initial data-file inventory

The Microdata Library catalogue lists these five Stata (.dta) files:

| File | Catalogue description | Cases | Variables | Initial relevance |
|---|---|---:|---:|---|
| `sdi_nigeria_2013_module1_anonymized.dta` | General information (facility level) | 2,480 | 170 | Primary starting file for facility characteristics, equipment, medicines and infrastructure |
| `sdi_nigeria_2013_module2_anonymized.dta` | Provider absence (healthcare provider level) | 22,152 | 25 | Provider attendance/absence |
| `sdi_nigeria_2013_module3_anonymized.dta` | Clinical vignettes (healthcare provider level) | 5,106 | 327 | Provider knowledge/clinical competence measured through case simulations |
| `sdi_nigeria_2013_module4_anonymized.dta` | Financial information (facility level) | 61,210 | 131 | Facility revenue and expenditure information |
| `sdi_nigeria_2013_weights.dta` | Sampling weights | 2,385 | 5 | Weighting for appropriate survey estimates |

**Important:** These files do not share one common row-level unit. Modules 1 and 4 are described as facility-level; Modules 2 and 3 are provider-level. Module 4 has many more records than the facility count, so inspect its questionnaire and data dictionary to establish exactly what each row represents before aggregation or merging. Do not assume the case count equals the number of facilities.

## Supporting documentation listed by the catalogue

- **Nigeria 2013 SDI Health Survey Questionnaire (Masked):** https://microdata.worldbank.org/catalog/2559/download/49988
- **Nigeria 2013 SDI Health Survey Report:** https://microdata.worldbank.org/catalog/2559/download/49991
- **SDI Health Anonymization Protocol:** https://microdata.worldbank.org/catalog/2559/download/49989
- **SDI Data Harmonization Protocol (February 2021):** https://microdata.worldbank.org/catalog/2559/download/49990

## Initial selection decision

Begin with **Module 1** because the first project objective concerns health-facility readiness and capacity. Its facility-level focus is the closest match to questions about facility characteristics, equipment, medicines and infrastructure.

Do not yet calculate indicators or merge modules. First download Module 1 and its documentation, inspect its variables and labels, and establish the facility identifier and any survey design information. Then decide whether Modules 2 and 3 can be linked appropriately for additional provider-level analysis. Treat Module 4 as a separate financial analysis component until its record structure is understood.

## Download and handling notes

- The source files are Stata `.dta` files, not Excel workbooks. They can be inspected with Stata, Python (`pandas.read_stata`), or R.
- Keep downloaded originals unchanged in `data/raw/` locally.
- Do not commit the raw microdata to this public GitHub repository until the exact licence terms and redistribution permission have been checked.
- Record the download date, exact filename, file size, and source version after downloading.
- This inventory is based on the official catalogue metadata and should be checked against the downloaded files before analysis.
