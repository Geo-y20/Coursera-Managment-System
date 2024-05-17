# Coursera Course Dataset

This repository contains the Coursera Course Dataset and the accompanying analysis and recommendation system developed as part of a Data Science project.
## Link Dataset:
https://www.kaggle.com/datasets/septa97/100k-courseras-course-reviews-dataset 

## Project Overview

This project aims to create an intelligent course recommendation system for learners seeking the right course on Coursera. By analyzing the dataset scrapped from the Coursera website, we can provide personalized course recommendations based on various factors such as course ratings, difficulty levels, and enrollment numbers.

## Dataset Description

The dataset contains 890 courses with the following columns:

- **course_title**: Title of the course.
- **course_organization**: The organization offering the course.
- **certificate_type**: Types of certification available for the course.
- **course_rating**: Ratings associated with each course.
- **course_difficulty**: Difficulty level of the course.
- **course_students_enrolled**: Number of students enrolled in the course.

## Data Cleaning and Preprocessing

The initial steps in our data analysis include:

1. Deleting the first unnamed column.
2. Renaming the column "course_Certificate_type" to "certificate_type".
3. Removing duplicate values.
4. Handling missing data (NaN and None values).
5. Extracting numerical values from the "course_students_enrolled" column.
6. Modifying the "course_difficulty" column for further use.

## Exploratory Data Analysis (EDA)

Our EDA process involves:

- Calculating the sum, mean, median, min, and max of the "course_rating" column.
- Plotting a histogram of "course_rating".
- Creating a scatter plot of "course_rating" vs "overall_rating".
- Generating a heatmap to visualize correlations between different variables.

## Feature Selection

For building the recommendation model, we selected the following features:

- **course_rating**
- **course_students_enrolled_modified**
- **course_difficulty_modified**

## Model Building and Evaluation

We developed a linear regression model using the selected features and evaluated its performance using the Mean Absolute Error (MAE) metric.

### Key Metrics

- **Mean Squared Error**: 4.415
- **Mean Absolute Error**: 4.017
- **R-Squared**: 1.0

## Recommendations

Based on the model's performance, we recommend the following improvements:

1. **Use more diverse features**: Include additional features such as course duration, language, and topic to improve the model's accuracy.
2. **Improve data quality**: Ensure the dataset is accurate and up-to-date, with no missing or incorrect values.

We also recommend courses with ratings over 8.5 as highly beneficial for learners.

## Conclusion

By implementing these recommendations, we can enhance the performance of the course recommendation system, providing more accurate and personalized suggestions to learners.

## Team Members

- George Youhana
- Pavli Bahaa

## Supervisors

- Dr. Essam Seddik
- Eng. Aya Mohamed

## Acknowledgments

We would like to thank our supervisors and the Arab Academy for Science Technology & Maritime Transport College of Artificial Intelligence for their support and guidance throughout this project.
