# Step-3-Model-Selection
* In this step, I selected M.L. model that I am going to use in this project.
* Due to performance concerns of my GPU and easy-to read format of my deployment on Flask, I chose a sample data from my original dataset. Sample data composes of 10000 random data from my original dataset.
* I did model selection by TPOTClassifier because of 3 reasons.
1) I used TPOTClassifer instead of TPOTRegressor because our problem is a classification problem.
2) TPOTClassifier returns best hyperparameters for given accuracy metric.
3) TPOTClassfier also returns best pipeline steps; these steps could be a single algorithm or multiple algorithms by the shape of our data. In my case, it is `DecisionTreeClassifier` with `SelectPercentile` 
* I added model selection process as `TPOT.ipynb`
