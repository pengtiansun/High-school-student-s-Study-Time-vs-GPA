# Study Time and GPA Analysis in R

This project investigates whether weekly study time is associated with GPA among high school students. Using a dataset of 2,392 students, the analysis begins with a simple linear regression to examine the direct relationship between study time and GPA, and then extends to a multiple regression model that includes absences, parental support, and tutoring.

## Project Objective

The main research question is:
Is weekly study time correlated with GPA among high school students?

This project was designed to examine whether students who spend more time studying each week tend to have higher GPAs, and whether that relationship remains meaningful after accounting for other academic and support-related factors.

## Dataset

- Dataset: Student Performance and Study Habits
- Source: Kaggle
- Creator: Rabie El Kharoua
- License: CC BY 4.0
- Observations: 2,392 students

The dataset is synthetic and includes student demographics, study habits, parental involvement, academic support, and GPA outcomes.

## Variables Used

Primary variables used in this analysis include:

- StudyTimeWeekly – hours spent studying per week
- GPA – grade point average on a 0–4 scale
- Absences – number of absences
- ParentalSupport – level of parental support
- Tutoring – whether the student receives tutoring

## Analysis Workflow

1. Loaded and inspected the dataset  
2. Checked for missing values and duplicate rows  
3. Selected relevant variables for analysis  
4. Visualized the relationship between weekly study time and GPA  
5. Calculated the correlation between study time and GPA  
6. Fit a simple linear regression model: GPA ~ StudyTimeWeekly
7. Tested the significance of the slope coefficient  
8. Evaluated regression assumptions using residual diagnostics  
9. Extended the analysis with a multiple regression model: GPA ~ StudyTimeWeekly + Absences + ParentalSupport + Tutoring
10. Compared the interpretation of the simple and multiple regression models  

## Methods

This project uses both exploratory and inferential methods to analyze student academic performance.

### Simple Linear Regression

The first model examines whether weekly study time alone predicts GPA.

**Model:**
GPA ~ StudyTimeWeekly

This stage focuses on:

- direction of the relationship
- slope interpretation
- statistical significance
- residual diagnostics
- practical versus statistical significance

### Multiple Regression

To deepen the analysis, the project expands the model by adding additional predictors that may also influence academic performance:

- Absences
- ParentalSupport
- Tutoring

**Model:**
GPA ~ StudyTimeWeekly + Absences + ParentalSupport + Tutoring

This extension allows for a more realistic interpretation of GPA as an outcome shaped by multiple factors rather than study time alone.

## Key Findings

### Simple Regression

The simple linear regression showed a **positive but weak relationship** between weekly study time and GPA.

- Correlation: approximately 0.179
- Estimated slope: approximately 0.029
- Interpretation: each additional hour of weekly study time is associated with about a 0.03-point increase in GPA
- The relationship is statistically significant, but the practical effect is modest

This suggests that study time alone explains only a small portion of GPA variation.

### Multiple Regression

The multiple regression model showed that weekly study time remained a statistically significant positive predictor of GPA even after controlling for absences, parental support, and tutoring.

The expanded model also suggested that:

- more absences are associated with lower GPA
- higher parental support is associated with higher GPA
- students who receive tutoring tend to have higher GPA than those who do not

Overall, the multiple regression results indicate that academic performance is multifactorial and should not be interpreted as a function of study time alone.

## Assumptions Checked

For the simple linear regression model, the project discusses the standard assumptions:

- Linearity: the relationship between study time and GPA is approximately linear
- Normality of errors: residuals are roughly centered around zero
- Constant variance: the residual spread is approximately stable across fitted values
- Independence: each student contributes one observation and is treated as independent

These assumptions were evaluated using the scatterplot, residual plot, and model summary.

## Why This Project Matters

This project demonstrates how regression can be used not only to detect statistically significant relationships, but also to evaluate whether those relationships are practically meaningful.

It also shows the importance of moving beyond a single-predictor model. While study time is positively associated with GPA, student performance is better understood when additional contextual factors such as attendance, parental support, and tutoring are included.

From a data science perspective, this project highlights:

- data cleaning and validation
- exploratory data analysis
- regression modeling
- statistical inference
- model interpretation
- critical discussion of limitations and effect size

## Limitations

This project has several limitations:

- The dataset is synthetic, so the relationships may be cleaner or stronger than in real-world educational data
- GPA is influenced by many factors that cannot be fully captured in a single model
- The analysis focuses on association and does not establish causation

## Files

- `Study Time and GPA Analysis in R.html` — rendered project report
- `study-time-gpa-analysis.Rmd` — source R Markdown file
- `README.md` — project overview

## Contributors

- Pengtian Sun
- Rachel Baron
- Stavan Sagala
- Xinyue Wang
