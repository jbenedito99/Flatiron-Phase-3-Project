# Overview 

This repository houses documents for a project concerning H1N1 vaccination rates. The project’s purpose was to create an optimal classifier for H1N1 vaccine data in order to inform stakeholders on the types of groups to target for educational outreach and awareness efforts. The main features of the repository are: 
* 2 data files used for classification analysis:
  * <b>training_set_features.csv</b>: houses feature columns
  * <b>training_set_labels.csv</b>: houses target column
* A slides presentation for non-technical stakeholders 
* A Jupyter notebook with data preprocessing and classification analysis steps 

# Business Context
This repository is applicable to public health officials who are at the forefront of H1N1 vaccination awareness efforts. 

The business question the project aimed to answer was: 
* <b>What are the most important features when it comes to predicting whether a person will get the H1N1 vaccine or not?</b>  

# The Dataset
As touched upon previously, the datasets used for this project were <b>training_set_features.csv</b> and <b>training_set_labels.csv</b>. These two files were combined in the Jupyter notebook into a singular dataset called <b>h1n1_data</b>, which had about <b>25,000 rows</b> and <b>over 20 columns</b>, following data cleaning and preprocessing. The data is from the <b>National 2009 H1N1 Flu Survey</b>, which was a questionnaire given in the United States that asked people about their backgrounds, opinions on the H1N1 vaccine, and general health behaviors. <b>h1n1_vaccine</b> was the column used as the <b>target</b>, a binary variable stating whether a person got the H1N1 vaccine or not.  

The image below shows a graph that represents the vaccination rates featured in <b>h1n1_data</b>:

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/8adadb49-e791-46b6-8d15-b2d04d0ed98d)

# Modeling Results 
The final chosen classifier was a <b>random forest</b>, which was tuned for <b>max_depth</b> and <b>n_neighbors</b> hyperparameters. It had an <b>accuracy of 81.4%</b> and an <b>AUC of 0.6</b>. 

A <b>confusion matrix</b> and <b>classification report</b> for the final model are pictured below: 

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/d9c42ab6-2a39-4780-a0ab-ec37a823e187)

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/044d2c84-82d7-4aa3-9ce6-0aee89160622)

This is a bar graph of the classifier’s <b>most important features</b>:

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/d9283e00-5ff3-4b1d-9d91-9e010c126d87)

# Conclusions
Based on the final classifier's most important features, my suggestions are to focus vaccination awareness efforts on people who:
* Find the <b>risk of getting H1N1 very low</b>
* Think the <b>vaccine is not effective</b>
* Are <b>non-healthcare workers</b>

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/7757a1a0-3bd8-4abd-a7a3-b9c34a84f638)

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/9e6d5a84-0e86-4997-999e-bb3fcacdde41)

![image](https://github.com/jbenedito99/Flatiron-Phase-3-Project/assets/125815448/5ed61d06-5c29-47f3-b524-858d2ec7b796)

# Sources and References
* [Presentation](https://docs.google.com/presentation/d/11idQQxp08yuHkJdn-PUnoPRLKYkx3yPKOOZXnxXVGuY/edit?usp=sharing) 
* Data from [this source](https://www.drivendata.org/competitions/66/flu-shot-learning/page/210/) 
