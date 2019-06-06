# Survival-Analysis:-
Statistical Modelling of survival rate
Technical Details of the Approach
1.Data Exploration
2.Data Preprocessing
3.Model selection
4.Training
5.Feature engineering
6.Evaluation
7.Prediction



Model selection:-
The important features that this particular dataset have are categorical variable or string.The feature selected for model building are as follow. I consider only those variable that I would be required to answer the question.
Feature_selected = ['sex','age','embarked','survived']
Output_variable=[‘survived’]
Except ‘age’ all the variables were categorical/string. 
1.The best choice based on data exploration is catboost  because CatBoost has the flexibility of giving indices of categorical columns so that it can be encoded as one-hot encoding using one_hot_max_size (Use one-hot encoding for all features with number of different values less than or equal to the given parameter value). 
2.The model built catboost has least bias and variance.
3. On comparing with other models Catboost performed very well.


Q.a).You have to predict if a person is male and have age above 18 then he will survive or not.
Ans. The man will not survive.(based on model prediction)
a={‘male’,age>18}
a=1 , on considering above condition on data, the rate 
Of survival is clearly explained by the bar plot

Q.b) You have to predict if a person is female and have age above 34 then she will survive or not.
Answer:- The woman will survive.(based on model prediction)
b={‘female’, ‘age’>34}
b=1 , on considering above condition on data. the rate 
Of survival is clearly explained by the bar plot   

Q.c) If you are a male and you are embarked as ‘C’, with age of 55 , then you will survive or not.
Answer:-A male embarked as ‘C’ with age of 55 will not survive.(based on model)
c={‘male’’, ‘age’=55, embarked= ‘C’}
c=1 , on considering above condition on data. the rate 
Of survival is clearly explained by the bar plot   

