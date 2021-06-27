# Bike sharing demand
 **In this project I've tried to apply different models on Bike sharing demand Dataset from Kaggle**
 - Logistic Regression
 - Random Forest
## 1.Data Visualitsation and Feature Engineering (FE)
 - Correlation of the features gives us really important imformations to decide which features can be used in our model.
 - Feature Engineering Techniques affects our model's efficiency.
    1. `OneHotEncoder()` for Categorical / Ordinal variables. It encodes values several one-hot-columns(0,1).
    2. `SimpleImputer()` for Metric(Mean) / Categorical(Mod) / Ordinal (Mode). It imputes values according to Mean, Mode etc.
    ### The Pipeline
    - It helps to use several FE techniques to a feature at the same time.

        `make_pipeline()` -> you can find the example of usage in bike_sharing_demand.ipynb
    ### The ColumnTransformer
    - It is really powerfull transformer. Applies transformers to columns of an array or pandas DataFrame.

        `ColumnTransformer([(name, transformer, column-names)])` -> you can find the example of usage in bike_sharing_demand.ipynb

## 2.Machine Learning Models
 **These models in this Project have almost same process**
  1. Initialize the Model -> `model = LogisticRegression()`
  2. Fit the model -> `model.fit(X_train, y_train)`
  3. Predict -> `y_train_pred = model.predict(X_train)`
  4. Evaluate the model -> Confusion Matrix



## 3.Comparing Accuracy between LogReg, DecisionTrees, RandomForest
    I get the highest score on RandomForestRegresson

