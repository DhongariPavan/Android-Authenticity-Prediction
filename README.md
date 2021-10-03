![image](https://user-images.githubusercontent.com/85613490/135740492-a98fd980-eae8-456d-a5cb-7c4447b5812b.png)

# Android App Malware Detection

AlmaBetter Verfied Project - AlmaBetter School
![image](https://user-images.githubusercontent.com/85613490/135740501-db741d42-0bdb-46ed-84ef-c938634a3089.png)

I have developed an android app malware prediction model in Python which classifies given Apps as malware or benign using the XGBoost Classifier.

# 💾 Project Files Description

This Project includes 1 ipynb notebook and 1 input CSV file:

# IPython Notebook:
Copy_of_TEAM_REALITY_ANDRIOD_AUTHENTICITY_PREDICTION.ipynb - Final IPython Notebook with explanation of steps in markdown.
# Input Files:
ANDROID AUTHENTICITY PREDICTION.csv - Input dataset having information about different apps available in Playstore.
     -----------------------------------------------------------------------------------------------------------------------------------

# 📖 Domain Knowledge

The open source nature of Android OS has attracted wider adoption of the system by multiple kinds of developers. This occurrence has further promoted an exponential in the number of devices running the Android OS into different sectors of the economy. Even if this progress brings some amazing technological improvements and simplicity of doing businesses and social relationships, they have however become powerful channel for the unconstrained cyberattacks and surveillance against business and the individual users of these mobile devices. Many cyberattacks techniques exist but attacks through the malicious applications have taken a jump in the recent years. Android malware has done progress in sophistications and intelligence that they have become highly immune to current detection systems.

Machine Learning techniques have emerged to provide more capable choice for tackling this kind of malware applications which are intelligent enough. The models created through Machine Learning algorithms work by first learning the patterns of malware behavior and then use this information to identify any such similar behavior from other applications.

# 📖 Project Description

In our project, Android Authentication prediction, our problem statement was to build a prediction model that would detect Malware Apps given it's features like Name, Package, Rating, Various Permission that it requires upon installation. Our approach was to understand the domain, clean the dataset, perform the EDA for better understanding of the dataset, try out NLP Modelling for Text Columns, build the final model, evaluate and improve accuracy and identify the future scopes.

Since we had a target class in the dataset, we went ahead with the typical methodology of solving a supervised Machine Learning Classification Problem. The first thing at hand was to clean the data by finding null values, dropping duplicates, handling outliers etc. After the cleaning, we tried out all possible visualizations for the different columns including count plots, word clouds for Text Columns, correlation plot with Target Class etc.

After performing EDA and inferring insights, we also carried out Chi-square test to identify feature importance beforehand to have an idea of what could be the most relevant features. Since our dataset had both Text Columns and numerical columns, specific emphasis on NLP was given at the beginning itself. NLP Modelling was tried out to see if Text columns alone could predict a Malware App. To our surprise, after fine tuning hyperparameters, Text columns itself gave a result of 71% accuracy using an XGBoost Model.

We were in a dilemma initially whether to include a Text column as dropping Text column would need enough reasoning and not dropping would add to complexity. Hence, we derived a new column from the NLP Model called Derived_prob_text that has predicted probabilities corresponding to a class for the whole dataset. We went ahead with two types of datasets, one with a text derived column and another one without it.

After having the 2 datasets, Modelling was given importance and out of all the models that we tried: KNN, Random Forest, GBM, XGBoost, Logistic Regression; XGBoost gave better accuracy, precision and recall. Plots like AUC-ROC Curve were also generated to validate this. Also, to our surprise, models performed well with the data frame having Text Derived Column and the feature importance was also high for this column.

To conclude, we were able to build a Malware App Classification Model with 89% accuracy (Text derived column increased accuracy by 8%). The future scopes and improvement of the project were also discussed in detail.

-----------------------------------------------------

# 📋 Execution Instruction

The given IPython Notebook can be either downloaded to be run on your local Jupyter Notebook or can be directly run on Google Colab.

-----------------------------------------------------

# 📜 Credits

Pavan Dhongari | Avid Learner | Data Scientist | Machine Learning Engineer | Deep Learning enthusiast

Contact me for Data Science Project Collaborations



-----------------------------------------------------

# 📚 References

Medium.com, 'How to Develop Your XGBoost Model in Python'. [Online].

Available: https://machinelearningmastery.com/develop-first-xgboost-model-python-scikit-learn/

analyticsvidhya.com, 'Complete Guide to Parameter Tuning in XGBoost with codes in Python'. [Online].

Available: https://www.analyticsvidhya.com/blog/2016/03/complete-guide-parameter-tuning-xgboost-with-codes-python/


