# Netflix Analysis Project

## Table of Contents

- [Project Overview](#project-overview)
- [Data](#data)
- [Repository Structure](#repository-structure)
- [Analysis Steps](#analysis-steps)
- [Key Findings](#key-findings)
- [Future Improvements](#future-improvements)
- [License](#license)

## Project Overview

This project explores trends in Netflix's catalog and builds predictive models to understand factors influencing user ratings. The structure of the project is:

1. **Data Cleaning**
2. **Data Analysis**
3. **Feature Engineering & Modeling**
4. **Conclusions**

The primary goals are:

- Study the composition of Netflix's movie catalogue.
- Investigate the relationship between release year and user ratings.
- Try to build and compare regression models to predict user scores.

## Data

- **Source**: `netflix.csv`.
- **Key Fields**:
  - `release_year`: Year of release
  - `user_rating_score`: Average user rating
  - `ratinglevel`: MPAA or TV rating category

## Repository Structure

```
├── LICENSE
├── README.md
├── requirements.txt
├── netflix.csv
├── netflix_analysis.ipynb
│ 
```

## Analysis Steps

1. **Data Cleaning**: Handling missing values.
2. **EDA**: Visualizing catalogue time distribution, rating distributions.
3. **Modeling**:
   - Linear & Polynomial Regression
   - Random Forest Regression
   - K-Nearest Neighbors
4. **Evaluation**: Comparing models via MSE and R², using k-fold cross-validation for non linear models.

## Key Findings

- The majority of the movies on Netflix in the catalogue were made after 2000s.
- No strong linear relationship between release year and user score.
- KNN outperform linear models, even though it is far for optimal (R^2=0.42).
- Cross validations show that the nonlinear algothitms are not performing well.

## Future Improvements

- Incorporate additional features (genre, runtime etc... which are absent in the csv) to find a better regression model. 
## License

This project is licensed under the [Apache License 2.0](LICENSE). Feel free to reuse and modify.
