## Competition rules SLM Summer semester 19/20
### Teams
Teams should consist of 1-3 members (Groups 104) and 1-2 members (Group 105). Please name the team - name will appear in table with results.

### Dataset and competition's goal
Goal of the competition is to achieve highest **accuracy** (percent of correctly classified observations [TP+TN/(TP+TN+FP+FN)]) in prediction of target variable **is_canceled**. To create a model please use **hotels_train.csv** and predict labels for **hotels_test.csv** data. Description of dataset features can be found in **hotels_description.txt**.

### Results
Please send the results to _lukasz.krainski123@gmail.com_ . Deadlines: Group 104 - 21:10, Group 105 - 23:00. In the e-mail please specify name of the group and members. Required attachments are:
1. R/Python/Julia script with used code
2. CSV file named **[group_name]_Hotels_prediction.csv** with one column named **Prediction** containing 5000 predictions with values 1/0 or TRUE/FALSE for dataset **hotels_test.csv**. Please make sure predictions order is the same as rows in test data.  

Ranking table will appear in below README file. Best team in each group will receive 5 points, next 4 points, etc.

### Ranking

**Group 104**

|Team             |Accuracy|Points|Model              |Language|
|-----------------|--------|------|-------------------|--------|
|Alone            |99.78   |5|Boosted Trees      |R       |
|Drzewce          |99.60    |4|CART               |Python  |
|M&M              |97.56   |3|Random Forest      |R       |
|Atena            |93.62   |2|CART               |R       |
|Trojca           |90.00      |1|Random Forest      |R       |
|102207_102217    |86.54   |0|Neural Network     |Python  |
|DreamTeam        |83.62   |0|CART               |R       |

**Group 105**

|Team             |Accuracy|Points|Model              |Language|
|-----------------|--------|------|-------------------|--------|
|XD               |97.28   |5|K-Nearest Neighbors|Python  |
|Jarosławy        |91.02   |4|Random Forest      |Python  |
|Dzikie Chrząszcze|85.54   |3|Boosted Trees      |Python  |
|Trash Pandas     |68.64   |2|Random Forest      |R       |

