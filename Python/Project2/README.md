# Python: Data Management Tips Over Connectivity

<br>

![](http://arqmain.net/iris/nnet-GoodBad-plot.png)

## INTRODUCTION

"Management of Data Base" [Data Management or DM] is still one of the most important activities of the present times. All areas of human development anytime require performing some operations related to Data Management.

This project covers the specific topic of connectivity with some of the more frequently used database management systems for relational databases at the present time. 

The principal approach of this work lies in delivering efficient ways of connectivity.  At the same time, it is included specific examples for each case and uses some practical “queries" to get information from databases.

The database management systems considered here are SQLite, MySQL, MS-SQL, MS-ACCESS, and PostgreSQL.  

Python is a highly dynamic ecosystem and it is having a great expansion these days. So, this publication aims to be located as a contribution on the issue of Python connectivity with updated reference in January 2018.

## IMPORTANT GENERALITIES
The connectivity treatment is given mainly through the SQLAlchemy application and the Python PANDAS library. SQLAlchemy is used to make the connection to the databases and PANDAS to make the examples of queries that are included here.

It is very important to note that in this environment the commands are translated to SQL in the background and when forced to execute, then the compiled SQL is executed on the database side and only the resulting dataset is loaded to memory. This characteristic turns to be extremely handy when v.g. The whole dataset does not fit the computer memory.

Please do not make a mistake including PANDASQL in this cluster of data management connectivity. Pandasql is a great module to be used by the time we want to apply SQL on python data frames but not to get connectivity from python to data management system like the ones treated in this project. Pandasql is a Python package for running SQL statements on pandas DataFrames. It has a lot in common with the SQLDF package in R.

The following tables show the relationship between R-project and Python in regards to the connectivity and SQL data frame querying facilities.  


Aqui va tablaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa


En este projecto se asume que el lector conoce la problematica inherente a la coneccion de los administradores de bases de datos a traves de los "drives" respectivos.  En este contexto, de todas maneras los siguientes links pueden ser consultados para recordar y/o abordar la tematica respectica, en especial para el caso de MS-SQL.



En el caso de MySQL y POSTgre se debe extraer los parametros(password,host, user, etc) de la plataforma respectiva, segun sea la instalacion que el lector tenga activada en su computador. Por ejemplo, MySQL en my caso host='localhost', db='mybase1', password=''.


Finalmente, para SQLite basta seguir las indicaciones entregadas en este projecto al momento de tratar la conectividad con la base respectiva.  Esto es deido a que Python a traves de Pandas has some support for reading/writing DataFrames directly.

This project develops neural Network algorithm of machine learning to classifythe quality of the wine "Good" or "Bad" according to 12 variables that characterize the wine subject to classification. I use nnet R library with a linout default option to get a logistic output.

![](http://arqmain.net/iris/nnet-GoodBad-plot.png)


I used the wine data set from the UCI Machine Learning data repository. The data can be found here [ http://archive.ics.uci.edu/ml/datasets/Wine+Quality ]. 

The original data is separated into white and red datasets. I combined them and created one additional variable: "Class" indicating "white" or "red" wine. After that, I re-coded the "quality" variable to indicate scores greater than or equal to 6 (denoted as "Good") or to indicate scores smaller than 6(denoted as "Bad").

I used "dfffull" dataset that considers all registers but replaces outliers by a "threshold" value which is generated for each variable using the upper limit of its Box-plot.

The model performance is evaluated using R, K fold cross-validation, and the ROC metric. I consider 70% and 30% original dataset splitting for the training and testing datasets respectively.

The model performance is evaluated using R, K fold cross-validation, and the ROC metric. I consider 70% and 30% original dataset splitting for the training and testing datasets respectively.
<br>

### Table of Contents   (  [  Link to R codes notebook ]( http://nbviewer.jupyter.org/github/arqmain/Machine_Learning/blob/master/R_MLearning/MLearning_Classification_PWine_GoodBad_NNetwork_R_KFold/Project8_Portugal_WINE_TwoClass_GoodBad_NNetwork.ipynb))

#### I Introduction

#### II Loading, EDA and Data Preprocessing

##### 21 Loading the data

##### 22 Exploratory Data Analysis (EDA) and Data Preprocessing

#### III Getting train and test datasets

#### IV Neural Network

##### 41 Building Machine Learning Model

##### 42 Plotting the Neural Network selected model

#### V Making predictions

#### VI Conclusion


<hr>

><i>Hector Alvaro Rojas<br>
>Data Science, Data Analysis, Visualizations and Applied Statistics / January 20, 2018<br>
>Email: <arqmain2010@gmail.com> <br>
>Url: [http://www.arqmain.net]   /   GitHub: [https://github.com/arqmain]</i>
