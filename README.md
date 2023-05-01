# Tennis_match_prediction
- This respitory is dedicated to predicting the winner of a tennis match.
- Use 4 different machine learning algorithms: Logistic Regression, Gaussian Naive Nayes, QuadraticDiscriminantAnalysis, RidgeClassifier.
- Metrics: Accuracy, Precision, and Recall.

## Preparation of data
- I only picked matches that are completed.
- The original dataset 
![image](https://user-images.githubusercontent.com/89664955/235504749-4e0f3354-185f-4ffe-b54f-8ddbceb877c5.png)
- I create a new feature called winning rate, which is the probability of winning of a player based on a serie and court environment. Then, I prepare the dataset so that it is ready for analysis and machine learning.
- Apply permutation for randomization of targets while keeping it accurate.
- Features: Players' ranking points, their winning rates, serie, and environment.
- Target: Winner of the match.
![image](https://user-images.githubusercontent.com/89664955/235507046-b6513e60-15e3-4a1b-908f-0b214734d330.png)

## Data analysis
#### Yearly Difference of ranking points
- Difference = Winner's point - Loser's point.
- The higher the difference, the better the model.
![image](https://user-images.githubusercontent.com/89664955/235507758-2348cb81-39fe-45e8-8b20-85996aaab664.png)
- Most of the time, the difference is high. However, around 25% of the players that win matches with less points.
![image](https://user-images.githubusercontent.com/89664955/235508059-c04f337e-ee94-49ab-97a0-fc98c1670073.png)
- High standard deviation due to outliers.

## Machine Learning prediction
![image](https://user-images.githubusercontent.com/89664955/235512237-c0737e84-8269-4667-9d5f-09f7dd3c641e.png)
- Based on the graph, logistic regression has the best performance.
- 
## Challenge
- There are not enough features such as players' injuries, playstyles, etc. that can affect the result of the match.
