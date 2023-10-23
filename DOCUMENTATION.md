# Income Prediction

### `CATEGORY`: **Classification**
### `PROBLEM`: **Predict whether an individual can make less or equal to or more than $50,000/yr**

***This project is also found in my GitHub Repository:*** [`GitHub Repository`](https://github.com/korisnik-samson/income-predictor/)

## *File Structure*
The project contains three files namely:

* ### [`exploration.ipynb`](exploration.ipynb)
    #### IN DETAIL:
    * The first operation was to remove duplicates from the dataset, as it would aid in eliminating errors
    * Analysis in `age` was carried out, due to the fact that it was a critical field to take seriously as it was also a deciding factor
    * An Age Distribution based on Working class was also carried out, with a histogram showing that most people in their 20's
      earned `<= $50,000` per annum
    * Also and observation that the highest population of `> $50,000` earners were in their early-mid sixties
    * The dataset contained a high number of `<= $50,000` earners, working in the `Private` working class
        along with other observations discovered from the query
    * Other findings were made as a result of the numerous queries, between `$50,000 <= x > $50,000` on the dataset as follows:
      * `A Histogram plot on the FINAL WEIGHTS`
      * `A Pie Chart showing the dirstubution of various levels of education acquired`
      * `A Histogram showing the marital status of these individuals`
      * `A Pie chart showing the distribution of their various occupations along with a PieChart`
      * `A Histogram that analysed their relationship status`
      * `A bar chart showing the various races and sex of these individual`
      * `A capital gain & loss distribution` <br>
    There by eliminating the unknown fields `?` in the dataset
    <br></br>
    #### IN SUMMARY
    * Used for fetching the dataset used in this project. 
      In this file are various data operations that are 
      executed for:
      * *Data Visualization*: plotting different forms of graphs from `matplotlib` to further understand
      the data making it possible for the upcoming stages of the project
      * *Data Cleaning*: this was an essential operation to carry out due to the fact that there were 
      unknown values and fields in the dataset. Thereby further making it more ready for other operations.
      In this part, outliers and missing values were taken care of, as to which fields in the dataset were 
      more relevant and usable.
      * It's also good to note that other operations were carried out in this file aside from the listed above <br></br>
      * Finally, the cleaned and prepared dataset that was ready for the next stage was exported to the directory [`src/cleaned_adult.csv`](src/clean_adult.csv)
      ready to use by other files in this project
    <br></br>
  
* ### [`preprocessing.ipynb`](preprocessing.ipynb) 
    This was more of like an extension to [`exploration.ipynb`](exploration.ipynb)
    In this file only but a few operations were applied to the dataset which was the Correlation Matrix to understand the relationship
    between the respective fields in the dataset, and so this was achieved using a heatmap

* ### [`machine_learning.ipynb`](machine_learning.ipynb) 
    At this stage, the dataset was ready for the machine learning and prediction algorithms to be used on. <br>
    For every prediction, three tests were carried out
    * `CLASSIFICATION TESTS`
    * `CONFUSION MATRIX` and finally
    * `ACCURACY SCORES`<br><br>
    In this file, libraries were drawn from `scikit-learn` for this purpose:
  * `RandomForests()`
  * `XGBoostClassifier()`
  * `SVM() - Support VEctor Machines`
  * `LogisticRegression()`


## RESULTS:
* `RANDOM-FORESTS` = 0.8651246131291741<br>
* `XGBOOST CLASSIFIER` = 0.8669164359016126<br>
* `SUPPORT VECTOR MACHINES` = 0.8468805994461639<br>
* `LOGISTIC REGRESSION` = 0.8247271542596514<br>

***IT'S ALSO NOTED THAT THESE VALUES AREN'T CONSTANT BUT XGBOOST ALWAYS HAD THE HIGHEST ACCURACY...<br>
AS SO, IT'S SAFE TO ASSUME THE `XGBOOST` AS THE... WINNER :)***

***Hvala Vam!*** <br>
### Attributions: <br>
*Prof. Marina Marijanović* <br>
*Prof. Timea Bezdan* <br><br>
*Singidunum University - Artificial Intelligence* <br>
***©️2023 Samson Offorjindu - 2021230446***