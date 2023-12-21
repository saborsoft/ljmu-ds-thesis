# ljmu-ds-thesis
LJMU Data Science Master's Thesis Project for Tamas Flesch

## Description
This project is about price analysis of FUT23 players' prices with Data Science technics.

### Dataset
https://www.kaggle.com/datasets/lucas142129silva/fifa-23-ultimate-team-players-database

### EDA project file
The first step is to run the EDA Jupyter notebook file on the original dataset, fifa23_players_2023-05-30.csv.

If someone doesn't want to walk through on the EDA steps, it is possible to use the futbin.csv, which is the cleaned dataset.

If someone runs the EDA notebook, the result will be the futbin.csv file.

### Linear regression step
When the futbin.csv is ready, you can run the linear-regression notebook. It will do some lin.reg. analysis on the data. There is an interesting thing in the data, there are regular players and very rare and valueable players. I decided to separate them, avg player who is under 100.000 FUT coin (in-game currency), star player who is above 100.000 FUT coin.

Lin.Reg. could be usable for the avg players with decent accuracy, but for star players and even for the full dataset, it doesn't seem a good model because the accuracies are very low (around 25% and 15%).

### Decision tree step
With the futbin.csv, the decision tree notebook will do some models, decision tree regressor, random forest, grid search cv with random forest regressor. After the hyper parameter tuning, the results were much better compared to the linear model.

### Neural Network step
With the same dataset, I created several neural networks for checking the model's perfomances. It has deeper and wider models as well. The results aren't as good as the decision tree results. The notebook is created under Google Colab, and saved the file from Colab to GitHub.
