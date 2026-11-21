# Childcare Cost and Affordability Analysis Across U.S. Counties

**DSC 640 – Data Presentation & Visualization**  
**Bellevue University**  
**Criselvi Lindsey | May 2026**

## Project Overview

This project analyzes childcare costs and affordability across U.S. counties using the U.S. Department of Labor's National Database of Childcare Prices.

The analysis examines how childcare expenses compare with median household income, how affordability has changed over time, and how childcare cost burdens vary geographically.

The project combines Python-based data preparation and exploratory analysis, an interactive Power BI dashboard, and a PowerPoint presentation designed to communicate findings to policymakers, researchers, and advocacy organizations.

## Business Problem

Childcare affordability is an important economic concern for working families. The financial burden varies across geographic regions and can affect household budgets and workforce participation.

This project addresses three questions:

1. How much of household income is required to cover infant childcare expenses?
2. How have childcare costs changed relative to household income over time?
3. Which counties experience greater childcare affordability pressures?

## Data Source

**U.S. Department of Labor – National Database of Childcare Prices**

https://www.dol.gov/agencies/wb/topics/featured-childcare

The analysis uses county-level childcare pricing, household income, and demographic information.

Selected variables include:

- State and county identifiers
- Study year
- Weekly infant, toddler, and preschool childcare costs
- Median household income
- Household employment characteristics
- Population measures

## Tools and Technologies

- **Python:** Data preparation, calculations, exploratory analysis, and visualization
- **Pandas and NumPy:** Data manipulation and derived metrics
- **Matplotlib and Seaborn:** Statistical charts and trend analysis
- **Plotly:** Interactive geographic visualization
- **Jupyter Notebook:** Analytical development and documentation
- **Power BI:** Interactive dashboard development
- **PowerPoint:** Presentation and communication of analytical findings

## Analytical Approach

### 1. Data Preparation

Selected relevant fields from the childcare pricing dataset and prepared county-level records for analysis.

Calculated monthly and annual childcare costs from reported weekly prices.

### 2. Affordability Analysis

Calculated infant childcare cost burden as annual infant childcare expenses divided by median household income, expressed as a percentage.

Evaluated the percentage of county records exceeding a 15% affordability benchmark.

### 3. Historical Trend Analysis

Examined childcare cost trends over time and compared changes in infant childcare costs with changes in median household income.

### 4. Geographic Analysis

Used county-level geographic identifiers to examine regional differences in childcare affordability.

### 5. Dashboard and Presentation Development

Developed a Power BI dashboard featuring summary metrics and supporting visualizations.

Created a presentation emphasizing key findings, historical trends, geographic disparities, and policy implications.

## Key Findings

**Widespread affordability challenges:** Many counties exceed commonly cited childcare affordability benchmarks.

**Increasing financial pressure:** Infant childcare costs have generally increased faster than median household income over the period examined.

**Geographic disparities:** Childcare affordability varies substantially across counties, indicating that financial burdens are not distributed evenly.

**Policy implications:** Regional differences suggest the potential value of geographically targeted affordability interventions.

These findings are descriptive and do not establish causal relationships.

## Project Deliverables

This repository contains:

- **Jupyter Notebook (.ipynb):** Python analysis, data preparation, and visualizations
- **Power BI Dashboard (.pbix):** Interactive childcare affordability reporting
- **PowerPoint Presentation (.pptx):** Findings and policy implications
- **Final Report (.pdf):** Analytical summary, visualization design decisions, findings, assumptions, and limitations

The notebook includes its saved execution outputs. The interactive county map is regenerated as `county_infant_cost_map.html` when the notebook runs, and a static preview (`county_infant_cost_map.png`) is shown in the notebook.

## How to Reproduce the Analysis

1. Download the Jupyter notebook from this repository.
2. Obtain the National Database of Childcare Prices from the U.S. Department of Labor.
3. Place the Excel dataset in the same directory as the notebook and name it `nationaldatabaseofchildcareprices.xlsx`, matching the notebook's file reference.
4. Install the required Python libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn plotly openpyxl
   ```

5. Open the notebook in JupyterLab or Jupyter Notebook.
6. Run the cells sequentially.

The notebook generates analytical visualizations and exports a prepared dataset named `childcare_cleaned_for_pbi_trend.csv`.

The county-level geographic visualization also retrieves a public GeoJSON file and therefore requires an internet connection.

The Power BI dashboard can be opened using Microsoft Power BI Desktop. Depending on the local environment and data-source paths, its data connections may need to be updated.

## Limitations and Considerations

- Median household income is used as an affordability indicator, but individual household circumstances differ.
- Affordability thresholds are analytical benchmarks rather than definitive measures of financial hardship.
- The underlying dataset does not fully capture childcare quality, availability, or local supply constraints.
- Geographic comparisons may benefit from further demographic segmentation, cost-of-living adjustments, and alternative weighting methods.
- Results should be interpreted as descriptive patterns rather than causal evidence.

## Visualization and Communication

The Power BI dashboard was designed to support interactive exploration by policymakers, researchers, and advocacy organizations.

The presentation provides a more focused narrative, progressing from the affordability problem to historical trends, geographic disparities, and policy implications.

Design considerations included consistent layouts, readable typography, visual hierarchy, restrained colors, and accessible chart presentation.

## Author

**Criselvi Lindsey**  
MBA, Business Analytics | M.S. Data Science  
Data & Analytics Leadership | Business Intelligence | Data Visualization

## References

- U.S. Department of Labor. National Database of Childcare Prices. https://www.dol.gov/agencies/wb/topics/featured-childcare
- U.S. Census Bureau. https://www.census.gov/
