# Education-Data-Analysis
These projects aim to improve learning outcomes by leveraging student data to provide personalized educational support.

# 💯 [Project 1: Student Grade Prediction](https://nbviewer.org/github/YerinKwak/education-data-analysis/blob/main/Student%20Grade%20Prediction%20%28Regression%29.ipynb) 
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
 
 
# :books: Project 2: Recommendation of children's books
## Created a tool that recommends books of the same age group with similar main ideas to each child's favorite books
### Data: [Data_source](https://www.kaggle.com/datasets/modhiibrahimalmannaa/1000-children-books-on-amazom)
### Method
1. Feature Engineering
 * Text cleaning: Cleaned texts from 'age' & 'description' features using regex function
 * Concept hierarchy generation: Considered age groups for children's books and the US school system and created age groups for four. 
                                 (i.e., 0-3(Infant, toddler books)/4-7(Picture books for children)/8-11(Chapter books for children)/over12(Young adult books))
 * Weighted rating: Transformed rating to weighted rating using IMDB's former weighted rating equation
2. Text mining
 * K-Means clustering: Clustered documents with similar text composition
 * Cosine Similarity: Created a tool that analyzes book descriptions and outputs books with high cosine similarities to the description.
3. Model
 * Received a book title, the model will return a list of the top 30 books with the highest cosine similarity and the same age group.
