# Final Project Rubric

**Group Members**

1. Palak Agarwal

**Project Repository**

- https://github.com/MUSA-550-Fall-2020/final-project-palak

**Grade: 75 / 80**

**Overall Comments**

# Grading

- **Concept (15/15)**:
  - **Criteria**
    - Is it sufficiently complex/challenging/sophisticated?
    - Is the final product useful/interesting/creative?
  - **Comments**
    - Good design and interesting research questions from a challenging dataset

* **Technical implementation (23/25)**:

  - **Criteria**
    - Was it well thought out?
    - Was each step done correctly?
    - Does it satisfy 2 of the guidelines listed below?
  - **Comments**
    - Impressive set of Panel dashboards, exploring 3 related and interesting aspects of the data
    - Good data wrangling of a challenging dataset
    - Dashboards are well-designed and include impressive interaction and charts
    - Better to have a separate "data processing" notebook that saves the cleaned dataframe "df_highlow" to a csv file. Then, you
      can simply load that CSV in your app notebooks rather than repeating the processing code in each notebook
    - The first app worked for me but app-2 and app-3 ran into issues reading the NOAA data — I saved the "df_highlow" dataframe from app1 and
      got everything to work well
    - Note that you can deploy these to Binder by including an "environment.yml" (similar to the one in the example Panel dashboards) in the
      repository (make sure you add noaa_coops to the environment file) and following [these directions](https://github.com/MUSA-550-Fall-2020/week-14/blob/master/DeploymentOptions.md)

- **Visualization (22/25)**:
  - **Criteria**
    - How well does the data visualization serve its purpose?
    - Does it tell a clear story?
    - Are the colors/layout/titles well-chosen?
  - **Comments**
    - Overall really well designed and thought out
    - Good use of visuals to explore the aspects of the data over time with a good use of user interaction
    - A few small comments that could improve visuals:
      - The map in the first app would be improved by a different projection (or removing Alaska) that focused on the lower 48
      - Years in altair charts are formatted as floats, which is misleading
      - The colormap repeats across cities which is confusing — better to use something like "tableau20" which has as many unique colors as cities

* **Writeup (15/15)**:
  - **Criteria**
    - Is all of the above explained clearly?
    - Does the 1-2 page writeup explain in depth all aspects of the project's implementation and final results?
  - **Comments**
    - Clear and detailed writeup

# Guidelines

The project is open-ended. The topic and technologies used are up to you.
However, the it must satisfy **at least two of the items below**:

- Data is collected through a means more sophisticated than downloading (e.g. scraping, API).
- At least one of the datasets contains more than 1,000,000 rows.
- It combines data collected from 3 or more different sources.
- The analysis of the data is reasonably complex, involving multiple steps
  (geospatial joins/operations, data shaping, data frame operations, etc).
- You use one of the analysis techniques for urban street networks (e.g., osmnx, pandana), clustering (e.g., scikit-learn), or raster datasets
- You perform a machine learning analysis with scikit-learn as part of the analysis.
- The webpage includes a significant interactive component (cross-filtering, interactive widgets, etc)
