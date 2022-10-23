# Yerin_Education
Education Data Science Portfolio

# 💯 Project 1: Student Grade Prediction 
## Personalized grade prediction system to maximize individual learning outcomes 
### Data: [Data_Source](https://archive.ics.uci.edu/ml/datasets/student+performance)

![](/images/Grade_Prediction.png)

### Method:
1. Exploratory Data Analysis
 * Analyzed data sets using graphs and heatmap to find overall pattern, outliers, and correlations
 * Performed T-test and ANOVA
2. Feature Engineering
 * Merged existing features
 * Outlier detection
 * One-hot Encoding
3. Models
 * Linear Regression
 * XGBoost
 * Ridge, Lasso: to reduce the influence of highly correlated features with regularization
4. Results
 * Compared RMSE of each model (Best model: 1.59)
 * Visualized the actual scores and the predicted ones to compare both
 
# :books: Project 2: Personalized recommendation of children's books
## Created a tool that recommends books of the same age group with similar main ideas to each child's favorite books
### Data: [Data_source](https://www.kaggle.com/datasets/modhiibrahimalmannaa/1000-children-books-on-amazom)
### Method
1. Feature Engineering
 * Regex function: Cleaned texts from 'age' & 'description' features using regex function
 * Concept hierarchy generation: Considered age groups for children's books and the US school system and created age groups for four. 
                                 (i.e., 0-3(Infant, toddler books)/4-7(Picture books for children)/8-11(Chapter books for children)/over12(Young adult books))
 * Weighted rating: Transformed rating to weighted rating using IMDB's former weighted rating equation
2. Model
 * Cosine Similarity: Created a tool that analyzes book descriptions and outputs books with high cosine similarities to the description.
