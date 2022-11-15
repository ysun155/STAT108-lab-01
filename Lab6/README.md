The dataset in this lab contains the SAT score (out of 1600) and other
variables that may be associated with SAT performance for each of the 50
states in the U.S. The data are based on test takers for the 1982 exam.
The following variables are in the dataset:

-   **`SAT`**: average total SAT score
-   **`State`**: U.S. State
-   **`Takers`**: percentage of high school seniors who took exam
-   **`Income`**: median income of families of test-takers ($ hundreds)
-   **`Years`**: average number of years test-takers had formal
    education in social sciences, natural sciences, and humanities
-   **`Public`**: percentage of test-takers who attended public high
    schools
-   **`Expend`**: total state expenditure on high schools ($ hundreds
    per student)
-   **`Rank`**: median percentile rank of test-takers within their high
    school classes

We first did model selection using adjusted R-squared, BIC, and AIC, and
decided to use the best subset selected by AIC to be our final model.
Then, we did model diagnoses using leverage plots, standardized residual
plot, and Cook’s distance. One influential point was found but we
decided to keep it. Finally, we checked multicollinearity with VIF.
