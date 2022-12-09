# Senior_Project_Hannah

Author: Ziyue(Hannah) Zhang

Paper: Model Optimisation and Feature Selection of IBM HR Employee Attrition

Data: IBM HR Attrition: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

## Introduction
Employee is a valuable asset for many firms. The Human Resource department monitors the employee inventory for the firms and wants to reduce business risks. They need to collect and analyze the employee movement data on a regular basis to track the company's recruitment situation. However, recently as the unemployment rate goes higher after the COVID crisis, there is a significant increase in employee turnover in many industries and that led to a high extra cost for the firms. In order to make a long-term business plan to ensure the company’s health, employee attrition has been highlighted in HR’s work. It is an important topic for a company's development: a low turnover rate is usually linked to high productivity, expected profit, and stability of the firm. Therefore, it is important to understand what leads to this situation and what can we do to mitigate it. 

My research question for this paper is to find out what are the influential factors that make employees leave their current job, which we also called employee attrition. In this paper, we used IBM HR attrition dataset to conduct a feature selection research. This dataset is public data that has been used for research since 2018. A lot of research has been done based on other sectors of employee attrition, like the hotel industry, banking, and technology firms. Also, different algorithms had been tested using this dataset, from basic statistical analysis to deep learning. However, some may contain flaws, like performance comparison and linearity between variables, while others did not realize the importance of imbalanced data affecting the model results. In this paper, I highly emphasized the property of this imbalanced dataset and made adjustments to my models. I explored two methods to approach this dataset in this paper: one self-designed logistic regression (Cox, 1958) with K-nearest clustering (KNN) (Mucherino, 2009) and another commonly used Support Vector Machine (SVM) (Cortes, 1995) method. Then in this paper, I plan to compare the results of both and find out the most influential factors. The overall performance of my self-designed Logistic regression with the KNN model performs very well. And that model satisfied all the statistical assumptions, which can be applied in the future. The other goal of the paper is to identify a reliable model that can be duplicated and reused widely for other firms in the employee-oriented industry using their company data. 

# Tools and Platform

All the models had been built using Python, within the Jupyter Notebook environment. In this research, I mainly used the Scikit-learn package (Pedregosa et al., 2011) and Pandas (McKinney et al, 2010) package to load the dataset and perform machine learning models. We used Matplotlib (Hunter, 2007) library for data visualization. Numerical computation had been conducted by the NumPy package (Van Der Walt et al. ,2011). Stata had been used rarely for the data exploration part. All the codes and supplementary material can be found in the Ziyue(Hannah) Zhang's Github repository (Zhang, 2022). 


## Results

According to all the algorithms that we applied in this paper Logistic regression, KNN, and SVM, there is not the best solution. The choice of model depends on the specific needs of the company. Logistic regression generally works very well. It can provide a lot of coefficients that help our analysis. The model performance is relatively high for both cases. KNN did a great job predicting the active working class, but not excellent in terms of the termination group. In the other words, if we have a balanced dataset, KNN may be a good algorithm to attempt. However, the labels it provides are very straightforward and easy for people to read and use. SVM gave very solid performance scores, but it needed a long computation time and computer capacities. The parameters put into the SVM model will significantly affect the model performance and results. Thus, we need to consider all the backgrounds before we choose the model that we want to perform. In terms of the selected features, even though every model gave a different result, an employee's self-reported satisfaction score may be a good indicator of whether they plan to stay in the company for a long time. Other points to keep in mind include travel frequency, number of firms worked before, etc. The uncertainty of human-based research is significant. We can not simply use one criteria to find out the reasons. 



