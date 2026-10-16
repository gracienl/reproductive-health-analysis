# Insurance Coverage and Fertility-Related Medical Help
## DATA 400 Individual Mini-Project 
### Gracie Nguyen

## Research Question

Is current insurance type associated with ever receiving medical help to become pregnant, after accounting for age, income, and education?

## Data and Analysis

This project uses the **2022 - 2023 National Survey of Family Growth (NSFG) Female Respondent Public-Use File** from the CDC. The original dataset contains 5,586 respondents, with 5,195 included in the final analysis.

The analysis includes survey-weighted descriptive statistics and visualizations, comparisons of private and Medicaid respondents across income groups, and survey-weighted logistic regression controlling for age, income, and education. 


**Main finding:** Approximately 12.9% of privately insured respondents reported receiving fertility-related medical help, compared with 4.3% of Medicaid respondents. After accounting for age, income, and education, Medicaid respondents had approximately 46% lower estimated odds of reporting medical help (adjusted OR = 0.54, 95% CI: 0.36-0.81). See the *written report* for detailed results, discussion, and limitations.

## Project Structure

```text
reproductive-health-analysis/
├── README.md
├── code/
│   └── reproductive_health_analysis.ipynb
├── data/
│   ├── Data Codebook/
│   └── NSFG_2022_2023_FemRespPUFData.csv
├── output/
│   ├── figures/
│   └── tables/
├── presentation/
│   └── insurance fertility.pptx
└── report/
    └── Written Report - Insurance Coverage and Fertility-Related Medical Help.docx
```

- `code/`: Jupyter notebook containing the complete analysis.
- `data/`: Original NSFG dataset and data codebook.
- `output/`: Generated figures and summary tables.
- `presentation/`: Project presentation.
- `report/`: Final written report.

## How to Reproduce the Analysis

1. **Download the data:** Visit the [CDC NSFG website](https://www.cdc.gov/nchs/nsfg/nsfg-2022-2023-puf.htm) and download the Female Respondent Public-Use CSV. Save it in the `data/` folder as `NSFG_2022_2023_FemRespPUFData.csv`.

2. **Install dependencies:** Use Python 3.11 or later and install the required packages:

   ```bash
   pip install jupyter svy polars pyarrow pandas numpy matplotlib
   ```

3. **Run the notebook:** Open `code/reproductive_health_analysis.ipynb` in Jupyter Notebook or VS Code. Select **Restart Kernel and Run All Cells** to execute the analysis.

4. **Review the results:** Generated figures and tables are saved in `output/figures/` and `output/tables/`. See the written report in `report/` for detailed interpretations.

**Note:** If the notebook cannot find the CSV file, check that the dataset filename and path match the location specified in the notebook.

## Data Source

National Center for Health Statistics. *National Survey of Family Growth, 2022–2023: Public use data file and documentation.* https://www.cdc.gov/nchs/nsfg/nsfg-2022-2023-puf.htm