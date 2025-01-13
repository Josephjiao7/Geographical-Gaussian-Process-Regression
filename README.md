<img src="https://github.com/user-attachments/assets/4e54d75f-a571-463d-b449-3ec13186445d" width="1400">

### Geographical Gaussian Process Regression
Geographical Gaussian Process Regression (GGPR): A Spatial Machine Learning Model Based on Spatial Similarity.
### Problem Statement
1.Most existing ML in spatial data can lead to overly optimistic performance and biased errors due to the conflict between spatial autocorrelation and the independent and identically distributed (i.i.d.) assumption.

2.Spatial ML models based on spatial dependence and spatial heterogeneity often require dense samples to satisfy the spatial stationarity assumption, making them inappropriate for small-sample prediction.

3.Few studies offered explainable tools to interpret black-box ML models and capture spatial effects for assisting the spatially decision-making research.

### Abstract
This study proposes a new spatial machine learning model called Geographical Gaussian Process Regression (GGPR). GGPR is extended from Gaussian Process Regression (GPR) by using the principle of spatial similarity for calibration, and it is designed to conduct spatial prediction and exploratory spatial data analysis (ESDA). GGPR addresses several key challenges in spatial machine learning. First, as a probabilistic model, GGPR avoids the conflict between spatial autocorrelation and the assumption of independent and identically distributed (i.i.d.), thus enhancing the model’s objectivity and reliability in spatial prediction. Second, GGPR is suitable for small-sample prediction that most existing models can hardly handle. Finally, integrated with GeoShapley, GGPR is an explainable model can measure spatial effects and explain the outcomes. Evaluated on two distinct datasets, GGPR demonstrates superior predictive performance compared to other popular machine learning models across various sampling ratios, with its advantage becoming particularly pronounced at smaller sampling ratios. As an ESDA model, GGPR demonstrates enhanced accuracy, better computational efficiency, and a comparable ability to measure spatial effects against both Multiscale Geographically Weighted Regression (MGWR) and Geographical Random Forests (GRF). In short, GGPR offers spatial data scientists a new method for predicting and exploring complex geographical processes. 

### Spatial Prediction
For spatial prediction, GGPR outperformed traditional GPR family models, RF, and XGBoost across both datasets, with its advantages being particularly evident in small-sample predictions.

The following figure illustrates the impact of noise on the performance of GGPR across two datasets. To ensure model robustness, we recommend setting the noise level for GGPR at or around 0.1.

### Exploratory Spatial Data Analysis 
As shown in following figure, by comparing the true spatially varying coefficients, we can observe that both MGWR and GGPR are capable of capturing spatial effects, and their coefficient estimation results are very similar. Although our simulated dataset includes more noise than Li (2024), they are essentially similar in nature. By comparing the ability of traditional machine learning models (GPR, XGBoost, RF, SVM) presented in Li (2024) to capture spatial effects, we observe that GGPR demonstrates significant advantages. This effectively highlights GGPR’s strength as a spatial machine learning model in understanding geographic processes.




### Reference:
Zhenzhi Jiao & Ran Tao (2025). Geographical Gaussian Process Regression (GGPR): A Spatial Machine Learning Model Based on Spatial Similarity. Geographical Analysis. (Accepted)
