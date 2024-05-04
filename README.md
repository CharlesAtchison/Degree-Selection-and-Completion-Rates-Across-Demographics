# 📊 Decadal Insights: An Exploration of Degree Selection and Completion Rates Across Demographics (2000-2022)

![Project Banner](images/project_banner.png)

## 🎓 Project Overview

This project conducts a comprehensive analysis of higher education data spanning from 2000 to 2022. It aims to uncover how demographic attributes such as gender, race, and immigration status influence degree selection and completion rates across different academic disciplines and award levels.

### 🎯 Objectives

- **Analyzing Trends**: Identify how different demographic groups select degrees and the influence of demographic attributes on these decisions.
- **Comparing Completion Rates**: Evaluate how demographic factors impact the rates of degree completion, identifying disparities and factors contributing to success or challenges in higher education.
- **Providing Insights**: Deliver actionable insights to educational institutions to enhance academic offerings and support services for a diverse student body.

### 🔍 Analytical Question

How do demographic attributes such as gender, race, and immigration status influence degree selection and completion rates across different academic disciplines and award levels in higher education institutions from 2000 to 2022?

### 🗂️ Dataset

The data for this analysis was sourced from the Integrated Postsecondary Education Data System (IPEDS), available through the National Center for Education Statistics. You can access the dataset from the following [link](https://nces.ed.gov/ipeds/datacenter/DataFiles.aspx?year=2000&surveyNumber=3&sid=c610fb17-7be5-4a97-8c02-99076b161130&rtid=7).

## 🏗️ System Architecture

1. **Data Ingestion**:
   - Automated aggregation of datasets from 2001 to 2022 into a unified data framework.
   - Data acquired by scraping annual datasets from IPEDS.
   - Individual datasets concatenated into a single DataFrame.
   - Final aggregated data stored in a Parquet file for efficient handling of large datasets.

2. **Data Cleanup and Transformation**:
   - Standardization and cleansing of raw data using Pandas and NumPy.
   - Creation of a `column_mappings` dictionary to align new, uniform column names with various labels in the dataset.
   - Handling of duplicates and missing values by selecting the first non-null value for each entry.
   - Retention of `cipcode` as numerical values for initial analysis, with plans to map them to meaningful descriptions later.

3. **Data Storage**:
   - Raw data stored locally in CSV format, merged into a combined DataFrame stored in Parquet format.
   - Processed data stored in Parquet format on the local filesystem for efficient retrieval and processing.

4. **Data Analytics**:
   - Utilization of SQLite for SQL-based analysis, enabling precise data manipulation and extraction.
   - Employment of Matplotlib and Seaborn for static charts, alongside Plotly for dynamic, interactive visualizations.
   - Descriptive analysis and visualizations such as histograms, box plots, and correlation matrices for comprehensive understanding of the dataset.

## 📈 Analytics and Visualization Highlights

- **Descriptive Analysis**: Insights into the dataset's characteristics, including mean, median, standard deviation, and quartiles of key variables.
- **Detailed Visualizations**: Distribution plots, box plots, and correlation matrices provide a deeper understanding of the data structure and relationships between variables.
- **Degree Popularity Analysis**: Examination of trends in degree popularity over time across various demographics, highlighting disparities and potential explanations.

## 📊 Results

The analysis reveals significant trends and disparities in degree popularity across demographics and genders. Key findings include:

- **Gender Disparities**: Notable differences in enrollment patterns for Business Administration and Nursing between men and women.
- **Racial and Ethnic Disparities**: Varying trends in Liberal Arts enrollment, STEM field enrollment, and vocational program enrollment across racial and ethnic groups.
- **Intersectional Considerations**: The importance of considering the multidimensional nature of students' identities when analyzing educational choices and experiences.

## 🚀 Deployment and Maintenance

The project follows a structured deployment strategy, including code review, testing, environment setup, data migration, continuous integration and deployment (CI/CD), monitoring, and documentation. Maintenance and support processes ensure the long-term sustainability and reliability of the data analytics system.

## 📖 Conclusion

This comprehensive data analytics project serves as a powerful tool for understanding and addressing disparities in higher education. By leveraging data-driven insights, educational institutions and policymakers can make informed decisions to promote equity, inclusivity, and student success. The project's scalable architecture, comprehensive analysis, and focus on continuous improvement lay the foundation for ongoing research and data-driven decision-making in the field of higher education.

## 👨‍💻 Author

- Name: Charles Atchison
- Date: May 4, 2024

Feel free to explore the project repository for more detailed information, code, and additional resources. If you have any questions or feedback, please don't hesitate to reach out. Happy analyzing! 😄
