# geomorphological-nomenclature-harmonisation
Supporting data and nomenclature crosswalk for harmonising Lombardy Region geomorphological datasets with the ISPRA Quaderno 13 framework.

# Supporting data for the harmonisation of geomorphological nomenclature using the ISPRA geodatabase

This repository contains the supporting workbook associated with the following article:

> Franceschi, L., Bosino, A., Cipolloni, C., & De Amicis, M. (2026). Methodological approach to harmonise geomorphological nomenclature through the ISPRA geodatabase: A case study on Lombardy Region datasets (Italy). *Geografia Fisica e Dinamica Quaternaria, 49*(1), 89–100. https://doi.org/10.4454/ke4qkt77

## Purpose of the repository

This repository documents the process used to harmonise the nomenclature of pre-existing environmental and geomorphological datasets from the Lombardy Region according to the Italian national guidelines for geomorphological mapping and the associated ISPRA Quaderno 13 geodatabase.

The workbook records the terminology found in the original datasets, the number of geometries associated with each value, the assessment of its geomorphological relevance, and the correspondence established with the Q13 nomenclature and codes.

It is intended to improve the transparency and reproducibility of the harmonisation workflow presented in the associated article.

## Repository contents

```text
.
├── data/
│   └── harmonisation_process_and_results.xlsx
├── CITATION.cff
├── LICENSE.md
└── README.md
```

The repository currently contains one Excel workbook with two worksheets:

1. `Original data`
2. `Harmonised data`

## Description of the workbook

### Original data

The `Original data` worksheet contains the terminology extracted from the attribute tables of the source datasets.

Each row represents a distinct combination of:

- source dataset;
- original spatial layer;
- value found in the attribute table;
- number of geometries associated with that value.

The worksheet also contains a concatenated identifier used to connect the original terminology with the corresponding record in the harmonised dataset.

The source material includes six dataset groups:

- `dissesti_IFFI`;
- `geoambientali`;
- `DUSAF`;
- `Opere_Difesa_Suolo`;
- `basi_ambientali_pianura`;
- `altri_dati`.

Overall, the workbook records 636 combinations of dataset, layer, and original attribute value, derived from 42 spatial layers.

### Harmonised data

The `Harmonised data` worksheet documents the assessment and harmonisation of the original terminology.

For each record, the worksheet reports:

- the source dataset;
- the source layer;
- the type of environmental information;
- whether the information is geomorphological;
- the corresponding Q13 morphogenetic process;
- the value found in the original dataset;
- the harmonised nomenclature, where correspondence was possible;
- the associated Q13 acronym;
- the number of geometries;
- the type of harmonisation relationship.

The worksheet also contains summary calculations describing the number of terms and geometries involved in the harmonisation process.

## Data classification

The original information was classified into four general data types:

- `GEOMORPHOLOGICAL DATA`;
- `LITHOLOGY`;
- `LAND USE`;
- `OTHER DATA`.

Records classified as geomorphological were subsequently compared with the nomenclature and database structure provided by ISPRA Quaderno 13.

## Q13 morphogenetic processes

The workbook uses the following Q13 morphogenetic-process codes:

| Code | Morphogenetic process |
|---|---|
| `LS` | Structural landforms |
| `TE` | Tectonic landforms |
| `VU` | Volcanic landforms |
| `GR` | Gravitational landforms |
| `FD` | Fluvial, fluvioglacial and runoff-related landforms |
| `CA` | Karst landforms |
| `GN` | Present-day glacial and nival features |
| `GL` | Glacial landforms |
| `PN` | Periglacial and nival landforms |
| `CO` | Coastal landforms |
| `EO` | Aeolian landforms |
| `AG` | Landforms of other origin |
| `AN` | Anthropogenic landforms |

The terminology used in this table follows the interpretation adopted in the harmonisation workflow. Users should consult ISPRA Quaderno 13 for the complete official definitions and database structure.

## Harmonisation categories

Each record was assigned to one of the following categories:

| Code | Meaning |
|---|---|
| `D` | Direct correspondence with Q13 |
| `F1` | Lexical variation, such as singular or plural forms |
| `F2` | Lack of correspondence within Q13 |
| `F3` | Indirect correspondence from a broader original term to a more specific Q13 term |
| `F4` | Geomorphological feature not represented in Q13 |
| `NGMF` | Feature not classified as geomorphological |

These categories describe the relationship between the terminology in the original regional datasets and the Q13 reference nomenclature. They do not represent an assessment of the scientific quality of the original datasets.

## Interpretation of the harmonisation

The harmonised nomenclature represents the correspondence selected during the workflow described in the associated article. Some mappings required interpretative decisions, particularly when:

- the original term was generic;
- the original terminology described a broader concept than the Q13 entry;
- more than one Q13 feature could potentially correspond to the original value;
- Q13 did not provide an equivalent geomorphological term;
- the original information was not primarily geomorphological.

The workbook should therefore be interpreted as a documented methodological crosswalk rather than as an automatic or universally applicable conversion table.

## Formula compatibility

The workbook contains formulas based on Excel functions including:

- `CONCAT`;
- `XLOOKUP`;
- `UNIQUE`;
- `SUMIF`;
- `COUNTIF`.

Some formulas may not be recalculated correctly in older versions of Microsoft Excel or in other spreadsheet software. Users interested only in the harmonisation correspondences should refer to the stored values in the main data columns.

Future releases may also include static CSV versions to improve long-term accessibility and software independence.

## Reuse

The workbook can be used to:

- examine the terminology present in the selected Lombardy Region datasets;
- reconstruct the correspondence between original terms and Q13 nomenclature;
- identify direct, indirect, and unresolved correspondences;
- support the development of similar harmonisation workflows in other regional contexts;
- compare nomenclature structures across environmental and geomorphological datasets.

The proposed correspondences should be reviewed by a geomorphologist before being applied to other datasets. The workflow cannot automatically identify or correct geometric, positional, or interpretative errors contained in the original sources.

## Limitations

The workbook was developed using a specific collection of regional datasets. Its direct transferability to other regions, scales, attribute structures, or mapping traditions has not yet been systematically tested. Semantic mappings retain an interpretative component, especially where original terms are generic or Q13 does not provide an unambiguous equivalent. Harmonisation improves terminological consistency and data documentation but does not replace expert validation of the original geomorphological information.

## Data provenance and rights

The harmonisation decisions and methodological classifications were produced by the authors of the associated study.

Names, codes, and attribute values originating from regional and national datasets remain subject to the terms and attribution requirements of their respective data providers. The licence assigned to this repository applies only to material for which the repository authors hold the necessary rights.

Users should consult the original data providers and ISPRA documentation before redistributing or reusing third-party content.

## Recommended citation

When using this workbook, please cite both the archived dataset and the associated article.

### Dataset

> Franceschi, L., Bosino, A., Cipolloni, C., & De Amicis, M. (2026). *Supporting data for “Methodological approach to harmonise geomorphological nomenclature through the ISPRA geodatabase: A case study on Lombardy Region datasets (Italy)”* (Version 1.0.0) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.XXXXXXX

The placeholder DOI will be replaced after the publication of the first Zenodo release.

### Associated article

> Franceschi, L., Bosino, A., Cipolloni, C., & De Amicis, M. (2026). Methodological approach to harmonise geomorphological nomenclature through the ISPRA geodatabase: A case study on Lombardy Region datasets (Italy). *Geografia Fisica e Dinamica Quaternaria, 49*(1), 89–100. https://doi.org/10.4454/ke4qkt77

## Versioning

The repository follows semantic versioning:

- `v1.0.0`: first curated public release;
- patch releases correct errors without changing the structure of the crosswalk;
- minor releases add documentation or compatible fields;
- major releases indicate substantial changes to the workflow, classification, or data structure.

The DOI of the specific dataset version used should be cited whenever possible.

## Contact

For questions, corrections, or suggestions concerning the harmonisation workflow, please open an issue in this GitHub repository or contact the corresponding dataset creator through the institutional information provided in the associated article.
