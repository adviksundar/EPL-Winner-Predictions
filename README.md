# Predicting English Premier League Soccer Match Winners

### Introduction: 
We built a machine learning model that would help us predict English Premier League (EPL) soccer match outcomes. Our main aim for this model is to provide clear insights into future EPL matches. The tool leverages a predictive model to forecast winners. Through a series of different steps, we built our machine learning model by utilizing Python libraries, eventually developing our own prediction tool.

### Step 1: Data 
Our first step was to load a CSV file (matches.csv) that contains over 1000 matches. The file contains information about the football matches such as the date/time of the match, the teams that played, and the result of the match. Once we fully explored our dataset, we split the data into training and testing sets based on the date.

### Step 2: Model Training
Once we split the data into training and testing sets based on the date, we built a Random Forest classifier with specific hyperparameters. The model was trained using the provided training data, which includes features and the target variable.  

### Step 3: Model Evaluation 
Once we developed our Random Forest classifier model, we began evaluating our model by generating predictions for the testing data. We then assessed the model's performance by calculating metrics like precision, which helps us understand how well the model predicts football match outcomes in the English Premier League.

### Step 4: Rolling Averages
We then began to develop a function that computes the rolling averages for team-related statistics. The function processes each team's match history, sorting it by date in ascending order. The rolling averages, calculated for specific columns, provide a smoothed trend of team performance over time. Once the function loops through the whole data frame, it will update the original dataset with these rolling averages and drop any missing values.

### Step 5: Team Name Translation
We developed a team name dictionary where we created a class that handles missing team names in a translation dictionary. Additionally, the dictionary maps the team names in our dataset. By developing a dictionary with translated team names, we make sure that our analyses are accurate and precise. 

### Step 6: DataFrame Merging 
We merged our translated team names to our existing data frame. This merging process helps create a combined data frame, making it easier to analyze match predictions, actual outcomes, and important match details.

### Step 7: Outcome Analysis
After merging our data, we analyzed our results and established a specific condition to filter matches where the model predicts Team X wins but Team Y loses. The actual outcomes of these matches were then counted.

### Step 8: Results Display
After completing our outcome analysis, the final merged DataFrame showcases predictions, actual outcomes, and relevant match details. These indicators affirm the functionality of our machine learning model in predicting football scores.
