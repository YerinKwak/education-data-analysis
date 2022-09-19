# Yerin_Education
Education Data Science Portfolio

# Project 1: Student Grade Prediction
## Created a tool that predict students' grade to help 
### Data: 

![](/images/Grade_Prediction.png)

### Method:
1. Exploratory Data Analysis
 * Analyzed data sets using graphs and heatmap to find overall pattern, outliers, and correlations
2. Feature Engineering
 * Skewed data: Log formation
 * Highly correlated features: Integration
3. Models
 * Linear Regression
 * XGBoost
 * Ridge, Lasso: to reduce the influence of highly correlated features with regularization
4. Results
 * Compared RMSE of each model (Best model: 1.59)
 * Visualized the actual score and the predicted one to compare both


# Project 2: Personalized recommendation of children's books
## Created a tool that recommends books of the same age group with similar main ideas to each child's favorite books
### Data: [](https://www.kaggle.com/datasets/modhiibrahimalmannaa/1000-children-books-on-amazom)
### Method
1. Feature Engineering
 * Regex function: Cleaned texts from 'age' & 'description' features using regex function
 * Concept hierarchy generation: Considered age groups for children's books and the US school system and created age groups for four. 
                                 (i.e., 0-3(Infant, toddler books)/4-7(Picture books for children)/8-11(Chapter books for children)/over12(Young adult books))
 * Weighted rating: Transformed rating to weighted rating using IMDB's former weighted rating equation
2. Model
 * Cosine Similarity: Created a tool that analyzes book descriptions and outputs books with high cosine similarities to the description.
