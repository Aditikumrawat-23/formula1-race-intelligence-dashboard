# Formula 1 Race Intelligence Dashboard

## Task 1: Downloading the Dataset

**Project:** Formula 1 Race Intelligence Dashboard Analysis Report

### Dataset Source
The dataset was provided through the SkillWallet Data Analytics with Tableau capstone project.

### Download and File Format
The provided dataset was opened in Google Sheets and downloaded in Microsoft Excel (.xlsx) format.

### Dataset Contents
The workbook contains the following sheets:
- circuits
- championship_standings
- lap_intelligence
- qualifying_results
- race_results

### Purpose
The dataset will be used to analyze Formula 1 race performance, driver and team standings, qualifying results, and lap-related information using Tableau.

## Task 2: Connect Dataset with Tableau

The Excel workbook is being connected to Tableau Public. The data source and workbook will be verified before this task is submitted for review.

## Tools Used
- Google Sheets
- Microsoft Excel (.xlsx)
- Tableau Public
- GitHub

## Task 2: Prepare the Data for Visualization

### Overview
Prepared the Formula 1 racing dataset in Tableau for visualization and dashboard development. The dataset contains multiple sheets covering race results, circuits, qualifying results, lap intelligence, and championship standings.

### Data Preparation Activities

**1. Data Connection and Relationship**
- Connected the F1 Racing Project Dataset (Excel) to Tableau.
- Established a relationship between `race_results` and `circuits` using `Circuit Id`.
- Kept `championship_standings` independent for team championship analysis.

**2. Data Type Validation**
- Verified the data types of important fields.
- Checked date, numerical, and categorical fields to ensure they were suitable for analysis.

**3. Calculated Fields**
- **DNF Count:** Created a calculated field to identify Did Not Finish (DNF) records using the `Dnf` field.
- **Points Cumulative:** Created a running-total calculation using `RUNNING_SUM(SUM([Points]))` for cumulative points analysis.

**4. Top N Parameter and Filter**
- Configured the `Top N Parameter` as an integer parameter.
- Set the default value to 10, minimum to 1, maximum to 20, and step size to 1.
- Created the `Top N Filter` calculated field using the points ranking and parameter.
- Made the parameter control available in the Tableau worksheet.

**5. Filters**
- Added a `Dnf Reason` filter to explore different reasons for drivers not finishing races.
- Added a year-based filter using `Race Date`.
- Kept all available values selected by default.

### Deliverable
- Tableau workbook: `F1_Race_Intelligence_Dashboard.twbx`
- The workbook has been uploaded to this GitHub repository for review.

### Outcome
Completed the initial data preparation setup in Tableau, including data relationships, field validation, calculated fields, parameter configuration, and filters. These preparations establish the foundation for the next stage: data visualization and dashboard development.

*Note: The calculated fields and their behavior should be validated in the final workbook before submission.*
