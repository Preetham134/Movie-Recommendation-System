# Movie Recommendation System

## Overview
A personalized movie recommendation system built using R and Shiny that utilizes Pearson correlation coefficients to suggest movies based on user preferences. The system processes user movie ratings to generate tailored recommendations through an interactive web interface.

## Technologies Used
- R Programming Language
- R Shiny for Web Interface
- Pearson Correlation Coefficient for Similarity Calculation
- R Markdown (.Rmd) for Implementation

## Project Structure
The project consists of two main R Markdown files:
1. `Testing_Single.Rmd`: Generates the necessary data files
2. `Shiny_application.Rmd`: Contains the Shiny web application code

## Generated Files
Running `Testing_Single.Rmd` produces three important data files:
- `correlation_matrix.rds`: Contains movie similarity scores
- `movies.rds`: Movie database information
- `reviews.rds`: User review data

## Installation Requirements
1. R (Latest version recommended)
2. RStudio
3. Required R packages:
   - shiny
   - tidyverse
   - recommenderlab
   - Matrix
   - data.table

## Steps to Run the Project
1. **Generate Data Files**
   - Open `Testing_Single.Rmd` in RStudio
   - Run the entire R Markdown file
   - Verify that three .rds files are generated:
     - correlation_matrix.rds
     - movies.rds
     - reviews.rds

2. **Launch the Application**
   - Place the generated .rds files in the same directory as `Shiny_application.Rmd`
   - Open `Shiny_application.Rmd` in RStudio
   - Run the R Markdown file
   - The Shiny application will open in a new window

3. **Using the Application**
   - Enter your preferred movies in the interface
   - The system will generate personalized movie recommendations based on your selections

## Usage Tips
- Ensure all required R packages are installed before running the project
- Keep all generated .rds files in the same directory as the Shiny application
- Make sure you have a stable internet connection while running the Shiny application

## How It Works
The system uses the Pearson correlation coefficient to:
1. Calculate similarities between movies based on user ratings
2. Generate a correlation matrix for all movies in the database
3. Use these correlations to recommend similar movies to users

## Troubleshooting
- If the Shiny application doesn't launch, verify that all .rds files are in the correct directory
- Check that all required R packages are properly installed
- Ensure you have the latest version of R and RStudio installed
