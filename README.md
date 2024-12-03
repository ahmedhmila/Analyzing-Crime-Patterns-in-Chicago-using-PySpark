
# Chicago Crime Analysis: Temporal Patterns and Hotspots

### Overview

This project was undertaken as part of a Big Data course at university. The objective is to analyze and visualize crime patterns in Chicago using the Chicago Crimes Dataset from 2001 to the present using PySpark. The analysis focuses on identifying temporal patterns and crime hotspots to provide insights that could assist in crime prevention strategies.
[Canva presentation]([/guides/content/editing-an-existing-page](https://www.canva.com/design/DAGYRIB8p_c/3YxtFf2OJ9AVEb9yBXdKAw/view?utm_content=DAGYRIB8p_c&utm_campaign=designshare&utm_medium=link&utm_source=editor))

### Dataset Description

- **Source:** Chicago Police Department's CLEAR (Citizen Law Enforcement Analysis and Reporting) system.
- **Time Frame:** 2001 to Present (excluding the most recent seven days).
- **Number of Records:** Over 8 million crime incident reports.
- **Features:** 22 columns including:
  - **ID:** Unique identifier for each incident.
  - **Date:** Date and time when the incident occurred.
  - **Primary Type:** Primary classification of the crime (e.g., THEFT, BATTERY).
  - **Description:** Detailed description of the crime.
  - **Location Description:** Type of location where the crime occurred.
  - **Arrest:** Indicates whether an arrest was made.
  - **Domestic:** Indicates whether the incident was domestic-related.
  - **Latitude & Longitude:** Approximate coordinates of the incident location.

### Project Structure

- **data/**: Contains the Chicago Crimes Dataset (CSV files).
- **notebooks/**: Jupyter notebooks with data exploration, analysis, and visualizations.
- **visualizations/**: Generated plots and charts.
- **README.md**: Project overview and instructions.
- **requirements.txt**: List of required Python packages.
- **LICENSE**: Project license information.

### Hypotheses

1. **Crime Rates Vary by Month and Season**
   - **Analysis:** Investigate whether certain months or seasons have higher crime rates.
   - **Expectation:** Crimes might increase during summer months due to warmer weather and increased outdoor activities.

2. **Specific Crime Types Are Concentrated in Certain Locations**
   - **Analysis:** Identify hotspots for specific crime types by analyzing crime frequency by location description.
   - **Expectation:** Certain locations experience higher frequencies of specific crime types.

3. **Patterns of Domestic vs. Non-Domestic Crimes Differ**
   - **Analysis:** Compare the characteristics of domestic crimes versus non-domestic crimes, such as times and locations.
   - **Expectation:** Domestic crimes may have higher occurrences during evenings and in residential areas.

4. **Crime Rates Vary by Hour of the Day**
   - **Analysis:** Examine crime occurrences by the hour to identify peak times.
   - **Expectation:** Crimes may be more frequent during certain hours due to factors like nightlife or work routines.

### Getting Started

#### Prerequisites

- Python 3.x
- Apache Spark with PySpark
- Jupyter Notebook
- Required Python packages listed in `requirements.txt`

#### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/ahmedhmila/chicago-crime-analysis.git
   cd chicago-crime-analysis
   ```

2. **Set Up the Environment**

   - Install Python packages:

     ```bash
     pip install -r requirements.txt
     ```

   - Ensure that Apache Spark and PySpark are properly installed and configured.

3. **Download the Dataset**

   - Due to size constraints, the dataset may not be included in the repository.
   - Download the "Crimes - 2001 to Present" dataset from the [Chicago Data Portal](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2).
   - Place the CSV file(s) in the `data/` directory.

### Usage

#### Running the Analysis

- **Jupyter Notebooks**
  - Navigate to the `notebooks/` directory.
  - Open and run the notebooks to explore the data and view the analysis and visualizations.

    ```bash
    jupyter notebook
    ```

#### Visualizations

Generated visualizations can be found in the `visualizations/` directory or can be reproduced by running the notebooks or scripts.

### Analysis and Findings

#### Hypothesis 1: Certain crime types have higher arrest rates than others.

- **Findings:** By calculating the average arrest rate per crime type, we can identify which crimes are more likely to result in an arrest.
- **Visualization:** A bar Violent crimes such as homicide or assault may have higher arrest rates compared to property crimes.

#### Hypothesis 2: Crime Rates Vary by Month and Season

- **Findings:** Crime rates are higher during summer months, with a noticeable increase from June to August.
- **Visualization:** A bar chart showing crime counts by month illustrates the seasonal trend.

#### Hypothesis 3: Specific Crime Types Are Concentrated in Certain Locations

- **Findings:** Certain crime types are more prevalent in specific locations (e.g., thefts on streets and in residences).
- **Visualization:** A clustered bar chart displays the top crime types across top locations.

#### Hypothesis 4: Patterns of Domestic vs. Non-Domestic Crimes Differ

- **Findings:** Domestic crimes peak during late evening hours, while non-domestic crimes are more evenly distributed.
- **Visualization:** A line plot compares domestic and non-domestic crime counts by hour.

#### Hypothesis 5: Crime Rates Vary by Hour of the Day

- **Findings:** Crime occurrences fluctuate throughout the day, with peaks in the late afternoon and evening.
- **Visualization:** A line plot shows crime counts by hour of the day.

### Conclusions

The analysis supports the hypotheses, revealing:

- **Seasonal and Hourly Patterns:** Higher crime rates during summer months and specific hours.
- **Location-Based Hotspots:** Concentrations of certain crime types in specific locations.
- **Differences in Crime Types:** Distinct patterns between domestic and non-domestic crimes.

These insights can assist in developing targeted strategies for crime prevention and resource allocation.

### Tools and Technologies

- **PySpark:** For scalable data processing and analysis.
- **Pandas:** For data manipulation and conversion to facilitate visualization.
- **Matplotlib and Seaborn:** For creating informative visualizations.

### Author

*This project was completed by [Ahmed Hmila](https://github.com/ahmedhmila) as part of the Big Data 2 course at EPI Digital School.*
##### Contact : ahmedhmiladev@gmail.com 
### License

This project is licensed under the MIT License. See the LICENSE file for details.

### Acknowledgments

- **Chicago Police Department:** For providing access to the crime dataset.
- **Course Instructors:** For guidance throughout the project.
