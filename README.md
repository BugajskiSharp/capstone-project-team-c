# Project Title: 
Predicting Marathon Average Finishing Times: The Impact of Weather and Air Quality on Marathons

## Background: 
Research has shown weather conditions and air quality can significantly affect a runner's marathon performance.

This project explores how environmental factors—such as temperature, dew point, wind speed, precipitation, visibility, and air quality collectively impact average finishing times across different performance groups (elite, competitive, intermediate, recreational and slow runners) and genders. The goal is to determine whether these conditions can help predict how different groups of runners are affected by the environment in a given year.

Understanding these patterns can help:

- prepare security details and medical logistics along the course based on assumptions of where runners will be
- event organizers to prepare runner waves, hydration and cooling stations in the most effective ways
- runners to prepare their pacing and set their expectations as a result of given weather conditions 


## Research Question: 
Can weather and environmental factors—such as temperature, wind speed, precipitation, dew point, visibility, sea level pressure, and air quality—predict average marathon finishing times across different performance groups (elite, competitive, intermediate, recreational and slow runners) and genders? 

## Hypothesis & Predictions
 
**Hypothesis:** Poor weather conditions (e.g., higher temperatures, dew point wind speed, precipitation, sea level pressure, or worse air quality) are associated with slower average finishing times, particularly for non-elite runners.

**Predictions:**  Elite runners are expected to be less affected by challenging weather and air quality, competitive and slow runners will experience greater slowdowns as conditions worsen with slow runners experiencing greater slowdowns. Female runners will show slightly less performance declines under adverse weather and environmental conditions. Overall, favorable conditions—moderate temperatures, low humidity, and clean air are expected to be associated with faster finishing times for all groups.

## Folder Structure 

- `data`: Contains the raw datasets and data dictionary.
- `notebooks`: Contains the `final-marathon.Rmd` and `archived-notebooks`/ subfolder with older .Rmd files retained for reference.
- `reports`: Contains all project reports, including the final report (`Final-Marathon-Report.pdf`).
- `capstone-project-team-c.Rproj`: The RStudio Project file. Opening this file sets the project root directory.
- `README.md`: Project overview and instructions.
- `rev.lock`: Records the exact R package versions used to ensure reproducibility.
- `renv`: Directory managed by `renv` that stores the project’s R package library and environment metadata.

## Custom Functions
There are two custom functions written and executed within the notebook `final_marathon.rmd`:
- `clean_chip_time`: cleans and standardizes chip-time values during early data cleaning steps
- `evaluate`: creates a list based on inputted model returning RMSE, MAE, R2, preds, and actual that are used for evaluation and graphing of linear model

## Project Setup & Reproducibility

This project uses the **renv** package to ensure a reproducible R environment.

### Requirements
- R version 4.5.2 (or compatible)
- RStudio 

### How to Run
1. Clone the repository
2. Open the project - Open `capstone-project-team-c.Rproj` in RStudio (this sets the project root)
3. Restore the project’s R package environment:
        ```install.packages("renv")  # if not already installed
        renv::restore()```
4. Open the `notebooks` folder
5. Select `final-marathon.Rmd`
6. Knit or run the .Rmd to reproduce the analysis.

## Team Members
- Krisha Bugajski-Sharp
- Meghan Holden
- Zachary D'Urso

