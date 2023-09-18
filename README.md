# ML-Algorithms-with-Earth-Observation-Data
Climate Region Clustering &amp; ET Simulation: ML Algorithms with Earth Observation Data

Hydrological processes and climate patterns play a crucial role in water resource management and planning. In this project, machine learning is used in hydrology to analyze and interpret water-related data. Clustering techniques are used to group similar hydrologic variables to discover potential patterns and classifications; regression analysis is used to establish relationships between hydrologic variables and to make predictions or estimates based on known data.
This also focuses on the application of machine learning techniques in hydrology, specifically clustering climate regions and simulating evapotranspiration (ET) using Earth observation data. The study area is California, USA. Through clustering analysis, aim to identify distinct climate regions based on precipitation and air temperature. Regression analysis is then performed to simulate ET rates using machine learning algorithms.

2.Clustering
Clustering analysis is an unsupervised learning method and is basically done to find the subgroups of samples based on features. In this project, two different clustering algorithms are used to investigate the structure of data with clustering in the given dataset.
Data Acquisition	
The climate data for the study area was obtained from Google Earth Engine, specifically the ERA5 Land Monthly product, within the time frame of 2010 with a resolution of 0.1 degrees. The dataset contains monthly information on precipitation and air temperature covering California, USA.

![01ppt_temp](https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/2d4fdf6c-e63c-453e-81fb-99cab7da79a5)


Figure 1: The plots depict the variation in temperature and precipitation pixels within the given study area.

#Clustering Algorithms
a)K-means Clustering 
b) Mini-Batch K-means Clustering


![5](https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/477e7a35-0565-4c69-8653-390ec5181e67)

Figure 2: The plot illustrates the elbow method, depicting the relationship between sum of squared error ( SSE) and the number of clusters(K).


![2](https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/8aa3ba2d-af70-494a-b12f-75771f99b05f)

Figure 2a: Clustering with k=3 (left: K-means, right: Mini-Batch K-means)


![3](https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/3f6a9c66-ae1c-44ec-9273-749acf09ce33)
Figure 2b: Clustering with k=6 (left: K-means, right: Mini-Batch K-means)

Regression
Regression analysis involves the study of the relationship between the true value and predicted values. In this project, four  different algorithms are selected  for the regression analysis. These algorithms are used to make the predictions based on the input data and access accuracy compared to the actual values. To evaluate the performance of the regression models, metrics scores and learning curves are employed as indicators.

Metrics scores provide quantitative measures, such as mean squared error (MSE) or R-squared, to assess how well the models fit the data. Mathematically, the R2 value represents the proportion of the variance in the dependent variable (the variable being predicted, here latent heat) that is explained by the independent variables (the variables used for prediction) in the regression model. R2 ranges between 0 and 1, where 0 indicates that the model does not explain any of the variances, and 1 indicates a perfect fit where all the variance is explained, and incase of RMSE, 0 is the optimal score.
Learning curves, on the other hand, provide visual representations of the model's performance by plotting the training and validation scores against the number of training samples. These indicators allow for a comprehensive evaluation of the regression models and help in understanding their effectiveness in capturing the relationship between the true and predicted values.
Data Acquisition 
For data processing, the essentials steps in preparing data for regression analysis were acquired from FLUX dataset and Google Earth Engine (GEE).  FLUX datasets consist data  from five stations  with various time frame and precipitation and temperature data were downloaded from the Google Earth Engine (GEE). Processing further includes handling of missing values(-9999) and splitting the data into training and testing sets. The whole dataset is prepared after concatenating the FLUX variables such as  Incoming shortwave(Wm-2), incoming longwave radiation (Wm-2), pressure(kPa), wind speed(m/s), vapor pressure deficit(hpa) andlatent heat flux(lh)   with GEE variables i.e temperature and precipitation. 


![4](https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/54e5dee5-dbc4-4485-b2be-3f7f0c9a7077)
Figure 3: The plot depicts the relationship between the target variable, latent heat, along the x-axis, and the independent variables represented on the y-axis.









