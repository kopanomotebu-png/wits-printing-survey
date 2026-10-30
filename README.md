# STAT4102 Mini Project: Wits Printing Survey

## Overview
This repository contains the reproducible R code, data, and survey instrument for the STAT4102 Applied Sampling mini-project. The project simulates a finite population of 10,000 Wits University students and estimates monthly printing/photocopying demand using a faculty-stratified sampling design with Neyman allocation.

## Files
| File | Description |
|------|-------------|
| `Questionnaire.pdf` | The proposed survey instrument for data collection. |
| `01_population_simulation.Rmd` | Generates the 10,000 student population (seed 4102). |
| `02_sample_size_section_B.Rmd` | Calculates sample sizes, Neyman allocation, and sensitivity analysis. |
| `03_sample_implementation_section_C.Rmd` | Draws the stratified sample (seed 4104) and calculates weights. |
| `04_design_based_estimation_section_D.Rmd` | Calculates estimates, standard errors, and compares with SRSWOR. |
| `05_simulation_assessment_section_E.Rmd` | Runs the 1,000-repetition Monte Carlo simulation (seed 4106). |
| `wits_printing_population_with_auxiliary.csv` | The full simulated finite population (10,000 rows). |
| `wits_printing_sample.csv` | The realised stratified sample of 414 students. |

## How to Reproduce
1. Open the `.Rmd` files in RStudio.
2. Ensure the `survey` package is installed (`install.packages("survey")`).
3. **Important:** Run the files in sequential order (`01` -> `02` -> `03` -> `04` -> `05`). 
   - *Note: File 03 must be run before 04 and 05, as it generates the auxiliary CSV file required by the later sections.*
4. Knit the files to view the HTML outputs and generate the final CSV files.

## Author
Kopano Motebu-2610723
