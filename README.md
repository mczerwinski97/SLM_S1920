# SLM_S1920
Repository for Statistical Learning Methods [223490-0286] - Summer semester 2019/20

**Requirements for final exam in Python (Group 105)**

Recommended versions of packages tested on `Python 3.7.4.`:
* IPython 7.13.0
* pandas 1.0.1
* numpy 1.18.1
* scikit-learn 0.22.2.post1 (please make sure you have version >=0.22 - required for CART cost-based pruning)
* seaborn 0.10.0
* matplotlib 3.2.0

---

**Points summary**

Below table summarizes points obtained through different assignments:
* Competition (extra points) - points for competition held on 20.06.2020. Seperate grading for groups 104 and 105. [Competition results](https://github.com/KrainskiL/SLM_S1920/blob/master/Competition/README.md)
* Exam - written laboratory exam scheduled for 03.06.2020
* Report - modeling problem report described in `Modeling problem report` section
* Homework (extra points) - task given during lectures focused on MNIST data
* DataFrames.jl course (extra points) - points for **finishing** DataFrames.jl course. Points are granted after sending course certificate (through email or MS Teams)

| Group | Index  | Competition | Exam | Report | Homework | DataFrames.jl course |
| ----- | ------ | ----------- | ---- | ------ | -------- | -------------------- |
| 102   | 102041 | 4           | \-   | \-     | \-       | \-                   |
| 103   | 72892  | 0           | \-   | 50     | \-       | \-                   |
| 104   | 63633  | 0           | \-   | \-     | \-       | 5                    |
| 104   | 67821  | 0           | \-   | \-     | \-       | Send certificate     |
| 104   | 68209  | 0           | \-   | 50     | \-       | 5                    |
| 104   | 68489  | 2           | \-   | 50     | \-       | 5                    |
| 104   | 72364  | 2           | \-   | 50     | \-       | Send certificate     |
| 104   | 72983  | 3           | \-   | \-     | \-       | 5                    |
| 104   | 73001  | 1           | \-   | \-     | \-       | \-                   |
| 104   | 73077  | 3           | \-   | 50     | \-       | Send certificate     |
| 104   | 73091  | 1           | \-   | \-     | \-       | \-                   |
| 104   | 73190  | 4           | \-   | \-     | \-       | \-                   |
| 104   | 85309  | 2           | \-   | \-     | \-       | Send certificate     |
| 104   | 102207 | 0           | \-   | \-     | \-       | 5                    |
| 104   | 102217 | 0           | \-   | \-     | \-       | \-                   |
| 104   | 102411 | 0           | \-   | \-     | \-       | \-                   |
| 104   | 105366 | 5           | \-   | \-     | 5        | 5                    |
| 105   | 59877  | 2           | \-   | \-     | \-       | Send certificate     |
| 105   | 72384  | 4           | \-   | \-     | \-       | Send certificate     |
| 105   | 72399  | 0           | \-   | \-     | \-       | Send certificate     |
| 105   | 72546  | 3           | \-   | 50     | \-       | 5                    |
| 105   | 73019  | 3           | \-   | 50     | 5        | 5                    |
| 105   | 73027  | 2           | \-   | 45     | \-       | Send certificate     |
| 105   | 73189  | 4           | \-   | \-     | 5        | Send certificate     |
| 105   | 83913  | 5           | \-   | \-     | \-       | 5                    |
| 105   | 102046 | 2           | \-   | \-     | \-       | 5                    |
| 105   | 102086 | 0           | \-   | \-     | \-       | \-                   |
| 105   | 102867 | 5           | \-   | \-     | \-       | \-                   |

---

**Modeling problem report**

Every student will be assigned to one dataset from [UCI Repository](https://archive.ics.uci.edu/ml/datasets.php).
The task is to analyze the data and produce a report with following structure:

`5pts` 1) Introduction, problem description (regression/classification/clustering/etc.), target variable and features explanation

`10pts` 2) Cleaning and preprocessing data - removing or imputing missing data, standarization, one-hot encoding, handling outliers, etc.

`10pts` 3) EDA with focus on exploring relations between features and target variable

`5pts` 4) Creating models, hyperparameter tuning

`10pts` 5) Graphical and descriptive model assessment

`10pts` 6) Summary, discussion on encountered problems and their solution e.g. how overfitting was avoided or imbalanced data mitigated

Code and descriptions/comments should be in Jupyter or R Markdown notebook. Both groups (104 and 105) are allowed to choose either R or Python (also remember there is Jupyter kernel for R). Please send reports to _lukasz.krainski123@gmail.com_ with following naming convention <index_number>_SLM_S1920_Report.< extension > before **03.06.2020r. EOD**. 
  
Each email should have 2 attachments: 
- for Jupyter: `.ipynb` file and `.html/.pdf` file generated from notebook, 
- for R Markdown:  `.Rmd` file and `.html/.pdf` file generated from notebook.

Below table of randomly picked datasets. If someone is missing on the list please contact me. If there is more than one dataset under given hyperlink, pick one.

| Index  | Dataset Name                                        | URL                                                                                          | Data Types                             | Default Task                | Attribute Types             | # Instances | # Attributes |
|--------|-----------------------------------------------------|----------------------------------------------------------------------------------------------|----------------------------------------|-----------------------------|-----------------------------|-------------|--------------|
| 59877  | Meta-data                                           | https://archive.ics.uci.edu/ml/datasets/Meta-data                                            | Multivariate                           | Classification              | Categorical, Integer, Real  | 528         | 22           |
| 63203  | Echocardiogram                                      | https://archive.ics.uci.edu/ml/datasets/Echocardiogram                                       | Multivariate                           | Classification              | Categorical, Integer, Real  | 132         | 12           |
| 63389  | Forest Fires                                        | https://archive.ics.uci.edu/ml/datasets/Forest+Fires                                         | Multivariate                           | Regression                  | Real                        | 517         | 13           |
| 63633  | Hepatitis C Virus (HCV) for Egyptian patients       | https://archive.ics.uci.edu/ml/datasets/Hepatitis+C+Virus+%28HCV%29+for+Egyptian+patients    | Multivariate                           | Classification              | Integer, Real               | 1385        | 29           |
| 67466  | Avila                                               | https://archive.ics.uci.edu/ml/datasets/Avila                                                | Multivariate                           | Classification              | Real                        | 20867       | 10           |
| 67821  | seeds                                               | https://archive.ics.uci.edu/ml/datasets/seeds                                                | Multivariate                           | Classification, Clustering  | Real                        | 210         | 7            |
| 68209  | Auto MPG                                          | https://archive.ics.uci.edu/ml/datasets/Auto+MPG                                           | Multivariate                           | Regression       | Categorical, Real     | 398         | 8           |
| 68418  | Mushroom                                            | https://archive.ics.uci.edu/ml/datasets/Mushroom                                             | Multivariate                           | Classification              | Categorical                 | 8124        | 22           |
| 68489  | Statlog (Heart)                                     | https://archive.ics.uci.edu/ml/datasets/Statlog+%28Heart%29                                  | Multivariate                           | Classification              | Categorical, Real           | 270         | 13           |
| 72364  | Turkiye Student Evaluation                          | https://archive.ics.uci.edu/ml/datasets/Turkiye+Student+Evaluation                           | Multivariate                           | Classification, Clustering  | 5820                        | 33          |              |
| 72384  | Page Blocks Classification                          | https://archive.ics.uci.edu/ml/datasets/Page+Blocks+Classification                           | Multivariate                           | Classification              | Integer, Real               | 5473        | 10           |
| 72399  | Parkinsons                                          | https://archive.ics.uci.edu/ml/datasets/Parkinsons                                           | Multivariate                           | Classification              | Real                        | 197         | 23           |
| 72546  | Wilt                                                | https://archive.ics.uci.edu/ml/datasets/Wilt                                                 | Multivariate                           | Classification              | 4889                        | 6           |              |
| 72892  | Bank Marketing                                      | https://archive.ics.uci.edu/ml/datasets/Bank+Marketing                                       |                                        | Classification              | Real                        | 45211       | 17           |
| 72983  | Japanese Vowels                                     | https://archive.ics.uci.edu/ml/datasets/Japanese+Vowels                                      | Multivariate, Time-Series              | Classification              | Real                        | 640         | 12           |
| 73001  | Leaf                                                | https://archive.ics.uci.edu/ml/datasets/Leaf                                                 | Multivariate                           | Classification              | Real                        | 340         | 16           |
| 73019  | Real estate valuation data set                      | https://archive.ics.uci.edu/ml/datasets/Real+estate+valuation+data+set                       | Multivariate                           | Regression                  | Integer, Real               | 414         | 7            |
| 73027  | Parkinsons Telemonitoring                           | https://archive.ics.uci.edu/ml/datasets/Parkinsons+Telemonitoring                            | Multivariate                           | Regression                  | Integer, Real               | 5875        | 26           |
| 73077  | Ecoli                                               | https://archive.ics.uci.edu/ml/datasets/Ecoli                                                | Multivariate                           | Classification              | Real                        | 336         | 8            |
| 73091  | Dow Jones Index                                     | https://archive.ics.uci.edu/ml/datasets/Dow+Jones+Index                                      | Time-Series                            | Classification, Clustering  | Integer, Real               | 750         | 16           |
| 73189  | MONK's Problems                                     | https://archive.ics.uci.edu/ml/datasets/MONK%27s+Problems                                    | Multivariate                           | Classification              | Categorical                 | 432         | 7            |
| 73190  | SPECTF Heart                                        | https://archive.ics.uci.edu/ml/datasets/SPECTF+Heart                                         | Multivariate                           | Classification              | Integer                     | 267         | 44           |
| 76417  | Audit Data                                          | https://archive.ics.uci.edu/ml/datasets/Audit+Data                                           |                                        | Classification              | Real                        | 777         | 18           |
| 83913  | Drug consumption (quantified)                       | https://archive.ics.uci.edu/ml/datasets/Drug+consumption+%28quantified%29                    | Multivariate                           | Classification              | Real                        | 1885        | 32           |
| 85309  | Absenteeism at work                                 | https://archive.ics.uci.edu/ml/datasets/Absenteeism+at+work                                  | Multivariate, Time-Series              | Classification, Clustering  | Integer, Real               | 740         | 21           |
| 102046 | Post-Operative Patient                              | https://archive.ics.uci.edu/ml/datasets/Post-Operative+Patient                               | Multivariate                           | Classification              | Categorical, Integer        | 90          | 8            |
| 102086 | Concrete Compressive Strength                       | https://archive.ics.uci.edu/ml/datasets/Concrete+Compressive+Strength                        | Multivariate                           | Regression                  | Real                        | 1030        | 9            |
| 102207 | Cryotherapy Dataset                                 | https://archive.ics.uci.edu/ml/datasets/Cryotherapy+Dataset+                                 | Univariate                             | Classification              | Integer, Real               | 90          | 7            |
| 102217 | Statlog (German Credit Data)                        | https://archive.ics.uci.edu/ml/datasets/Statlog+%28German+Credit+Data%29                     | Multivariate                           | Classification              | Categorical, Integer        | 1000        | 20           |
| 102411 | Lung Cancer                                         | https://archive.ics.uci.edu/ml/datasets/Lung+Cancer                                          | Multivariate                           | Classification              | Integer                     | 32          | 56           |
| 102867 | Carbon Nanotubes                                    | https://archive.ics.uci.edu/ml/datasets/Carbon+Nanotubes                                     | Univariate                             | Regression                  | Real                        | 10721       | 8            |
| 105261 | Abalone                                             | https://archive.ics.uci.edu/ml/datasets/Abalone                                              | Multivariate                           | Classification              | Categorical, Integer, Real  | 4177        | 8            |
| 105262 | Parkinson Dataset with replicated acoustic features | https://archive.ics.uci.edu/ml/datasets/Parkinson+Dataset+with+replicated+acoustic+features+ | Multivariate                           | Classification              | 240                         | 46          |              |
| 105333 | ISTANBUL STOCK EXCHANGE                             | https://archive.ics.uci.edu/ml/datasets/ISTANBUL+STOCK+EXCHANGE                              | Multivariate, Univariate, Time-Series  | Classification, Regression  | Real                        | 536         | 8            |
| 105366 | Phishing Websites                                   | https://archive.ics.uci.edu/ml/datasets/Phishing+Websites                                    |                                        | Classification              | Integer                     | 2456        | 30           |

---
**Contact**

Name: Łukasz Kraiński

Email: lukasz.krainski123@gmail.com

---
**Lecturers**

• lecturer: Bogumił Kamiński

• laboratories: 

Groups 100 and 101 – Michał Kot, 

Group 102 – Kinga Siuta, 

Group 103 - Agata Skorupka, 

Groups 104 and 105 – Łukasz Kraiński

---
**Schedule**

• lectures: Tuesdays, 8:00-10:35, Aula IV

• laboratories: room A-113 (day and hour according to group division)

---
**Lectures**

|Date |Subject|
|-----|-------|
|25-02-20 | Introduction to data science; McKinsey case study|
|03-03-20 | Working with Git and Github|
|10-03-20 | Introduction to Julia programming for data science|
|17-03-20 | Introduction to predictive modeling|
|24-03-20 | Introduction to threading and distributed computing K-nearest neighbors algorithm|
|31-03-20 | Methods of evaluation of predictive model quality|
|07-04-20 | Working with data frames in Julia|
|21-04-20 | Methods of predictive model selection|
|28-04-20 | Regularization for predictive modeling|
|05-05-20 | Introduction to approximation and local predictive models|
|12-05-20 | Introduction to deep learning|
|19-05-20 | Causality modeling: introduction|
|26-05-20 | Causality modeling: algorithms|
|02-06-20 | Storytelling with data|
|09-06-20 | Data science in production environments + written examination|

---
**Laboratories**
|# |Subject|
|--|-------|
|1 |Refresher on R and Python programming|
|2 |Methods of evaluation of classifiers|
|3 |Nonparametric regression models: smoothing spline, LOESS, GAM|
|4 |Classical machine learning models: CART, random forest|
|5 |Deep learning|
|6 |Modeling competition|
|7 |Computer exam|

---
**Literature**

Stephen Boyd and Lieven Vandenberghe, Introduction to Applied Linear Algebra
(http://vmls-book.stanford.edu/)

Gareth J., Witten D., Hastie T., Tibshirani R. (2013), An Introduction to Statistical Learning
with Applications in R (http://www-bcf.usc.edu/~gareth/ISL/)

Hastie T., Tibshirani R., Friedman J. (2013), The Elements of Statistical Learning
(http://www-stat.stanford.edu/~tibs/ElemStatLearn/)

Optional: Kamiński B., Zawisza M. (2012), Receptury w R. Podręcznik dla ekonomisty, Oficyna
Wydawnicza SGH (http://bogumilkaminski.pl/projekty/)

Optional: B. Kamiński, P. Szufel: Julia 1.0 Programming Cookbook, Packt Publishing, 2018
(https://www.packtpub.com/application-development/julia-10-programming-cookbook)

---
**Course evaluation criteria**

<s>• Written examination (50 points); during last lecture; no supporting materials are allowed</s>

• Modeling problem report (50 points); sent to your teaching assistant before last laboratory

• Laboratory examination (50 points); during last examination; you can bring your own printed
materials

• Possible extra points: homeworks, competition

---
**Grading rules**
|From |To|Final grade|
|-----|--|--------|
|0 |49| 2.0|
|50 |59 |3.0|
|60 |69 |3.5|
|70 |79 |4.0|
|80 |89 |4.5|
|90 |100 |5.0|
