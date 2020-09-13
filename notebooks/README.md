# Planning

## Data Cleaning

1. After opening the csv as a Pandas DataFrame, remove the following columns:

- Location
- Date
- Address
- URL
- Google
- Yelp
- Reviewer
- Notes
- Unreliable
- Rec

2. Fill NaN values in all float columns with the average of that column.
3. Treat Xs and xs as the same in specific food columns and convert to 1s
4. Convert NaN values in specific food columns to 0s.
5. Double Check all cardinal values for string issues and potential duplication.

## Building and Training Model

1. Determine mode baseline accuracy and baseline and ROC AUC score.
2. Shuffle the data
3. Encode cardinal values in pipeline (OneHotEncoder)
4. Begin with Logistic Regression, then work up the chain.
5. Pick model with the best accuracy or ROC AUC score.

## Building the App

1. Rewatch Ryan Herr's instructional video for Plotly

2. Design app to assume certain parameters such as Hunger, Synergy, Uniformity, and overall which the user would not know.

    - App will assume user is outside of San Diego unless box is checked in the affirmative.

    - If San Diego Box is checked, drop-down box for neighborhoods will be in the available

    - Float values will have forms will those tick-up-tick-up down boxes and set maxima and minima so that irrealistic values are impossible.

    - Each of the cardinal values will have tick boxes for the user to check whether or not to add an ingredient.