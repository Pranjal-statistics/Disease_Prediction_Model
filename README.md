# Disease_Prediction_Modeling


This project focuses on predicting diseases using various machine learning models. We import and clean the data, selecting features for our model. The dataset contains variables representing various clinical symptoms, with prognosis as the outcome, which is a result of the combination of symptoms. The dataset was sourced from Kaggle: Disease Prediction Using Machine Learning

The data is prepared by importing and cleaning, with all missing values addressed. Our final dataframe has no missing values and prognosis has 42 unique categorical values representing various diseases. All other variables are valued either 1 or 0.

In our feature selection phase, we use the Boruta package for feature selection and importance ranking. As a result of the Boruta feature selection, "fluid_overload" was rejected and removed from the data.

The data is then divided into training and test datasets, using a 70/30 split. This split is performed randomly but ensures balanced outcome classes.

## Modeling

We use various machine learning algorithms, including Decision Trees, Naive Bayes and Support Vector Machines (SVM), to create predictive models. The models are compared using various metrics.

The Decision Trees are a type of Supervised Machine Learning where the data is continuously split according to a certain parameter. This model achieved an accuracy of 89.70%.

The Naive Bayes classifier, a probabilistic model that uses Bayes' Theorem with strong (naïve) independence assumptions between the features, achieved an impressive accuracy of 100%.

The Support Vector Machines (SVM), a maximum margin classifier, also achieved an accuracy of 100%.

## Summary

In comparison, the SVM and Naive Bayes models performed better than the Decision Tree model in terms of accuracy, specificity, and sensitivity.

However, in a real-world scenario, it is impractical to achieve an accuracy of 100%. As a result, it can be inferred that the models are overfitting due to the unavailability of accurate data. This indicates a potential need for additional data or the application of regularization techniques to improve model performance.

By using these models, we can develop systems that are capable of predicting diseases based on a set of symptoms, potentially helping in providing early and more accurate diagnoses. However, it should be noted that these models should not replace professional medical advice but can provide valuable insights and supplement professional medical judgement.

The project is a stepping stone in the field of medical diagnosis using machine learning, with potential for further optimization and refinement. Contributions and suggestions for improvements are always welcome.
