# Titanic Survival Prediction - Project Summary

## Introduction
This machine learning project analyzes the Titanic dataset to predict passenger survival. Before starting this project, I didn't know the specific statistics of the Titanic story, but I was curious to understand exactly what types of passengers were more likely to survive this historical event. I wanted to apply machine learning techniques to discover patterns in the data and build models that could predict survival based on passenger characteristics.

## Project Goals
My main goals for this project were to:
- Learn about the Titanic disaster through data analysis.
- Discover which passenger factors most influenced survival chances.
- Apply machine learning to build predictive models.
- Practice the complete data science workflow, from exploration to modeling.

## Project Overview
This project explores the famous Titanic dataset to understand what factors influenced passenger survival. Using machine learning, I built models that can predict survival based on passenger information like gender, age, and ticket class.

## Dataset Description
- Source: Kaggle Titanic dataset
- Passengers: 891 people aboard the Titanic
- Features: Age, gender, passenger class, fare, family members, and survival status.
- Goal: Predict whether a passenger survived based on their characteristics.

## Key Findings from Data Exploration
During my analysis, I discovered several major survival patterns:
- Gender Made the Biggest Difference: 74% of women survived compared to only 19% of men.
- First Class Advantage: 63% of first-class passengers survived versus only 24% of third-class.
- Age Mattered: Younger passengers, especially children, had better survival chances.
- Wealth Helped: Passengers who paid higher fares survived more often.

## Confirmed Hypotheses
My initial predictions were largely confirmed by the data:
- Women survived much more often than men.
- First-class passengers had a significant survival advantage.
- Younger passengers had better survival chances.

## Data Quality Notes
I noticed that age information was missing for about 20% of the passengers, and most cabin information was unavailable (77% missing). The dataset provided good information about demographics and travel details. One challenge I faced was deciding how to handle the missing Age values. I initially wasn't sure if I should just delete those rows, but I eventually decided to fill them with the median age so I wouldn't lose valuable passenger data.

## Machine Learning Results

### Models Built and Tested
I tested three different approaches to see which worked best:
1. Baseline Model: Always predicts "did not survive" (61.5% accuracy).
2. Logistic Regression: A simple, interpretable model (81.6% accuracy).
3. Random Forest: A more complex model (82.1% accuracy).

### Validation Approach
I used 5-fold cross-validation to ensure my results were reliable. The models showed consistent performance across different data splits.

### Model Performance Summary
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|--------|----------|
| Baseline | 61.5% | 0% | 0% | 0% |
| Logistic Regression | 81.6% | 78% | 75% | 76% |
| Random Forest | 82.1% | 80% | 74% | 77% |

### Most Important Survival Factors
The models confirmed what I found in my initial analysis:
1. Gender (most important)
2. Ticket Fare
3. Age
4. Passenger Class

## What Worked Well
The models successfully learned meaningful patterns from the passenger data. Both the simple and complex models performed much better than random guessing. It was satisfying to see that my initial insights from the data exploration phase were confirmed by the machine learning models.

## Limitations and Future Improvements

### Limitations:
- Missing Data: I had to estimate missing age values for 20% of the passengers.
- Small Dataset: With only 891 passengers, there is a limit to how complex the models can get without overfitting.

### Future Improvements:
If I were to continue this project, I would:
- Extract more features from passenger names (like titles: Mr., Mrs., Dr.).
- Try more advanced methods for handling missing age values.
- Add information about family groups traveling together.

## Conclusion
This project successfully demonstrated how machine learning can uncover important patterns in historical data. The models achieved 82% accuracy in predicting survival, confirming that gender, wealth, and social class were major factors in who survived the Titanic disaster. Through this project, I learned a great deal about the Titanic story while successfully applying machine learning techniques to real-world data.
