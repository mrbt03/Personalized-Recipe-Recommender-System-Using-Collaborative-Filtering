# Personalized Recipe Recommender System Using Collaborative Filtering

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Data Sources](#data-sources)
- [Project Overview](#project-overview)
- [Future Improvements](#future-improvements)
- [Credits](#credits)

## Overview
The **Personalized Recipe Recommender System** is a machine learning project developed in R using Item-Based Collaborative Filtering (IBCF) to provide customized recipe recommendations based on user interactions (clickstream data). This system leverages user behavior data to predict and recommend recipes that users are most likely to engage with, enhancing their overall experience on recipe platforms.

## Features
- **Collaborative Filtering Approach**: Utilizes Item-Based Collaborative Filtering (IBCF) to generate personalized recipe recommendations based on user click behavior.
- **Optimized Model**: Hyperparameters are fine-tuned using grid search to minimize errors (RMSE and MAE) and achieve high prediction accuracy.
- **Interactive Web Application**: Deployed as a user-friendly Shiny app, allowing users to input their User ID and receive personalized recipe suggestions.
- **Integrated Metadata**: Combines recipe metadata such as recipe names, difficulty levels, and cooking methods for enriched recommendation details.

## Technologies Used
- **Languages**: R
- **Libraries**: `recommenderlab`, `tidytext`, `dplyr`, `shiny`
- **Tools**: RStudio, Shiny

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/recipe-recommender-system.git
## Usage
- **User Input**: Enter your User ID in the Shiny app interface.
- **Receive Recommendations**: Click on "Get Recommendations" to view a list of personalized recipe suggestions with their respective names, difficulty levels, and cooking methods.

## Data Sources
- **Clickstream Data**: User interaction data (`user_id`, `recipe_id`, click records).
- **Recipe Metadata**: Additional details like `recipeid`, `recipename`, `difficulty`, `cookmethod` sourced from a text file (`recipesamp.text`).

## Project Overview
This project is an extension of a class project to evaluate different recommender algorithms with a unique front-end design. The first file (`project.Rmd`) tests three different recommender algorithms—Item-Based Collaborative Filtering (IBCF), Singular Value Decomposition (SVD), and User-Based Collaborative Filtering (UBCF)—using different parameters (similarity metrics, normalization). The goal is to find the best algorithm with optimized hyperparameters by performing a grid search and identifying elbow points with the number of nearest neighbors.

## Future Improvements
- **Incorporate NLP and Textual Data**: Integrate Natural Language Processing (NLP) to analyze recipe titles and descriptions for more refined recommendations.
- **Ensemble of Recommender Systems**: Develop an ensemble of different recommender algorithms that could be further refined through user testing to improve recommendation quality.

## Credits
This project was created by Mark Ruiz as an extension of their class project to evaluate different recommender algorithms. All code and content were developed to build a personalized recipe recommender system with a unique front-end interface.
