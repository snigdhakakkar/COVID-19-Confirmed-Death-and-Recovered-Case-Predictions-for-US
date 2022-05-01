# COVID-19-Confirmed-Death-and-Recovered-Case-Predictions-for-US <br />
COVID-19-Confirmed, Death and Recovered Case Predictions for US (As a part of Assignments in Data And Knowledge Management Course at University of Waterloo) <br />

**Steps Implemented** - <br />
1. Technologies: Python, Keras, Scikit-learn, Pandas, Numpy <br />
2. **Data preprocessing steps**__: <br />
 
Checking for Missing values in Columns. <br />
Checking for duplicate records and dropping it if any. <br />
Removing features that are highly dependent upon each other. In Covid Dataset we have [State ID], so we do not need [State, Long, Lat] and dropping these features. <br />
Type Casting the [Resident Population 2020 Census] and [Population Density 2020 Census] data into float data type. <br />
Adding the relative difference of specific quanititative attributes with respect to the state. <br />
Checking for outliers - Data point that differs significantly from other observations.By plotting Histograms, we look at data distribution for a variable and find values that fall outside the distribution. <br />
Performing Z Score Regularization - score helps to understand if a data value is greater or smaller than mean and how far away it is from the mean. If the Z score of a data point is more than 3, it indicates that the data point is quite different from the other data points. Such a data point can be an outlier. <br />
Outliers Removal: - Removing those rows that have [Incident_Rate] greater than 2.5 Z-Score value or lesser than -2.5 Z-Score value Removing those rows that have [Case_Fatality_Ratio] greater than 3 Z-Score value or lesser than -3 Z-Score value. <br />
Applying PCA on the covid features and creating a hybrid dataset with a combination of original features along with first five PCA components. <br />

3. Used hyperparameter selection <br />
4. **Segregated into 2 parts** - <br />

**Part 1**: <br />
Applied Machine learning algorithms (Decision Tree, Naive Bayes, Random Forest, XgBoost and GradientBoost) and compared their performance <br />
**Part 2**: <br />
Applied Deep learning techniques (Deep Neural Networks Model, Custom - LSTM )<br />
