# IRT calibration of PISA 2025 science trend items: Wales and England

In this project I ran an item response theory calibration of the 80 PISA 2025 science trend items for students in Wales and England, in R using the mirt package.

## Questions
1. How do the 80 science trend items perform for students in Wales and England?
2. Is a Rasch model adequate, or do items differ in discrimination?
3. How well does this calibration agree with the official PISA 2025 international item parameters?

## Methods
- Data preparation from the PISA 2025 international database: item selection verified against the codebook and Technical Report, matrix-sampled and adaptive design, missing-data rules
- Classical item facility by test route (linear vs adaptive)
- Rasch/PCM and 2PL/GPCM models, compared by likelihood-ratio test and information criteria
- Item parameters, item characteristic curves and partial-credit category functioning
- Rasch infit and outfit
- EAP ability estimates, empirical reliability, and validation against official plausible values and Annex A item parameters
- Test information and targeting

## Key findings
- The 2PL/GPCM model fitted better than the Rasch model (χ²(79) = 851.15, p < .001).
- Most items discriminated well; two had weak discrimination and no items showed underfit.
- Estimates agreed closely with the official PISA parameters (r = .90 for difficulty, .86 for discrimination) and with official science scores (r = .83).
- The item pool was well targeted to students in Wales and England (test information peaked at θ = −0.22).

## Files
- `index.html`: rendered report
- `report.Rmd`: analysis code and text

## Data
PISA 2025 international database (OECD): https://www.oecd.org/en/data/datasets/pisa-2025-database.html. Access requires completing the OECD's short user form. The data cannot be redistributed and so i have not included it here. To reproduce the analysis, download the cognitive item and student questionnaire files (SPSS), prepare the data as shown in the report, and save it to `data/`.

Data source acknowledgement: Programme for International Student Assessment (PISA), Organisation for Economic Co-operation and Development (OECD), Paris.

## Next steps
Differential item functioning (DIF) analysis between Wales and England.
