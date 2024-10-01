
# Birth Weight Analysis Project

## Table of Contents
- [Birth Weight Analysis Project](#birth-weight-analysis-project)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Project Structure](#project-structure)
  - [Data Description](#data-description)
    - [Key Variables](#key-variables)
  - [Data Modeling](#data-modeling)
    - [Relational Model](#relational-model)
  - [Analysis Process](#analysis-process)
  - [Results](#results)
  - [Conclusion](#conclusion)
  - [How to Run the Project](#how-to-run-the-project)
  - [Dependencies](#dependencies)
  - [References](#references)

## Introduction
This project aims to understand and analyze the factors that influence the birth weight of newborns. The study is based on demographic and health data from the United States for births occurring in 2018. Using Python, SQL, and data modeling techniques, the project examines how various factors impact birth weight, which is an essential indicator of infant health.

## Project Structure
The project consists of the following main files:
<!-- - `report.pdf`: A detailed report that presents the analysis and findings of the study. -->
- `python.ipynb`: A Jupyter Notebook containing the data processing, analysis, and visualization using Python.
- `sql.ipynb`: A Jupyter Notebook demonstrating the database creation and queries using SQL.

## Data Description
The dataset used for this study includes information on newborns, their parents, and various health-related factors. It can be found [here](https://data.nber.org/nvss/natality/csv/2018/natality2018us.csv). It contains variables such as:
- **Demographic Data**: Age of parents, race, education level, etc.
- **Health Data**: Birth weight, duration of pregnancy, prenatal consultations, maternal health conditions (e.g., diabetes, hypertension).

The data was sourced from birth certificates recorded by the National Center for Health Statistics (NCHS) in collaboration with different states.

### Key Variables
- `age_mere`: Mother's age
- `duree_grossesse`: Duration of pregnancy
- `poids_bebe`: Birth weight
- `mere_fumeuse`: Whether the mother is a smoker
- `rf_gdiab`: Gestational diabetes presence
- `rf_phype`: Hypertension before pregnancy

A complete dictionary of variables is available [here](https://data.nber.org/) for detailed descriptions.

## Data Modeling
The project employs the MERISE methodology to design a conceptual and relational data model for the study. The data model includes entities such as `BEBE`, `MERE`, `PERE`, `ZONE`, and `MALADIE`, with relationships that represent the associations between them.

### Relational Model
The key tables in the relational model are:
- `BEBE`: Contains data on newborns, such as weight, birth order, and health conditions.
- `MERE`: Contains information about the mother, including age, education level, and health conditions.
- `PERE`: Contains details about the father, including age and education level.
- `ZONE`: Represents the geographical origin of parents.
- `MALADIE`: Represents health conditions of the mother and child.

The SQL notebook demonstrates how these tables were created and populated.

## Analysis Process
The analysis was conducted using Python for data cleaning, processing, visualization, and statistical analysis. The key steps included:
1. **Data Preprocessing**: Cleaning, recoding, and handling missing values.
2. **Descriptive Analysis**: Using Python libraries to generate summary statistics and visualizations.
3. **Statistical Analysis**: Conducting econometric analysis to identify factors affecting birth weight.

The analysis was implemented in the `python.ipynb` notebook.

## Results
The analysis confirmed that the birth weight of a newborn is influenced by several factors, including:
- Mother's age
- Duration of pregnancy
- Prenatal visits
- Presence of diabetes in the mother
- Hypertension
- Plurality of the pregnancy
- Smoking habits of the mother

Detailed results, along with graphs and tables, are available in the `python.ipynb` notebook.

## Conclusion
The project concludes that birth weight is significantly affected by both maternal and pregnancy-related factors. These findings align with existing literature on the subject and emphasize the importance of monitoring and managing these factors to ensure healthy birth outcomes.

## How to Run the Project
1. Clone this repository.
2. Ensure you have all necessary dependencies installed (see [Dependencies](#dependencies)).
3. Open the `sql.ipynb` notebook to view the data modeling and database creation process.
4. Open and run the `python.ipynb` notebook to perform the data analysis.

## Dependencies
The following libraries are required to run this project:
- Python 3.x
- Jupyter Notebook
- Pandas
- Numpy
- Matplotlib
- Seaborn
- SQLite3

You can install the necessary packages using:
```bash
pip install pandas numpy matplotlib seaborn
```

## References
- [CDC National Center for Health Statistics](https://www.cdc.gov/rdc/index.htm)
- [SwissMom - Factors Influencing Birth Weight](https://www.swissmom.ch/fr/bebe/aspects-medicaux/le-nouveau-ne/taille-et-poids/quest-ce-qui-influence-le-poids-a-la-naissance/)
- [PubMed Article on Birth Weight](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4163183/)

---

This README provides a comprehensive guide to the project, detailing the objectives, data, analysis process, and findings. 