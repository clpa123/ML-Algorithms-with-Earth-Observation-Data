# ML-Algorithms-with-Earth-Observation-Data
Climate Region Clustering &amp; ET Simulation: ML Algorithms with Earth Observation Data

Hydrological processes and climate patterns play a crucial role in water resource management and planning. In this project, machine learning is used in hydrology to analyze and interpret water-related data. Clustering techniques are used to group similar hydrologic variables to discover potential patterns and classifications; regression analysis is used to establish relationships between hydrologic variables and to make predictions or estimates based on known data.
This also focuses on the application of machine learning techniques in hydrology, specifically clustering climate regions and simulating evapotranspiration (ET) using Earth observation data. The study area is California, USA. Through clustering analysis, aim to identify distinct climate regions based on precipitation and air temperature. Regression analysis is then performed to simulate ET rates using machine learning algorithms.


2.Clustering
Clustering analysis is an unsupervised learning method and is basically done to find the subgroups of samples based on features. In this project, two different clustering algorithms are used to investigate the structure of data with clustering in the given dataset.
Data Acquisition	
The climate data for the study area was obtained from Google Earth Engine, specifically the ERA5 Land Monthly product, within the time frame of 2010 with a resolution of 0.1 degrees. The dataset contains monthly information on precipitation and air temperature covering California, USA.

<img width="457" alt="image" src="https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/b5935218-8941-4420-897c-95423d8c865b">

Figure 1: The plots depict the variation in temperature and precipitation pixels within the given study area.

#Clustering Algorithms
a)K-means Clustering 
b) Mini-Batch K-means Clustering

<img width="344" alt="image" src="https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/5260d965-c801-431e-adc6-290c86256f9b">

Figure 2: The plot illustrates the elbow method, depicting the relationship between sum of squared error ( SSE) and the number of clusters(K).


<img width="413" alt="image" src="https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/f7a9aea4-76ce-454d-b75c-be1849547f44">

Figure 2a: Clustering with k=3 (left: K-means, right: Mini-Batch K-means)

<img width="407" alt="image" src="https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/1dcbc587-8571-4502-bf40-f509e3f4bd43">

Figure 2b: Clustering with k=6 (left: K-means, right: Mini-Batch K-means)

Regression
Regression analysis involves the study of the relationship between the true value and predicted values. In this project, four  different algorithms are selected  for the regression analysis. These algorithms are used to make the predictions based on the input data and access accuracy compared to the actual values. To evaluate the performance of the regression models, metrics scores and learning curves are employed as indicators.

Metrics scores provide quantitative measures, such as mean squared error (MSE) or R-squared, to assess how well the models fit the data. Mathematically, the R2 value represents the proportion of the variance in the dependent variable (the variable being predicted, here latent heat) that is explained by the independent variables (the variables used for prediction) in the regression model. R2 ranges between 0 and 1, where 0 indicates that the model does not explain any of the variances, and 1 indicates a perfect fit where all the variance is explained, and incase of RMSE, 0 is the optimal score.
Learning curves, on the other hand, provide visual representations of the model's performance by plotting the training and validation scores against the number of training samples. These indicators allow for a comprehensive evaluation of the regression models and help in understanding their effectiveness in capturing the relationship between the true and predicted values.
Data Acquisition 
For data processing, the essentials steps in preparing data for regression analysis were acquired from FLUX dataset and Google Earth Engine (GEE).  FLUX datasets consist data  from five stations  with various time frame and precipitation and temperature data were downloaded from the Google Earth Engine (GEE). Processing further includes handling of missing values(-9999) and splitting the data into training and testing sets. The whole dataset is prepared after concatenating the FLUX variables such as  Incoming shortwave(Wm-2), incoming longwave radiation (Wm-2), pressure(kPa), wind speed(m/s), vapor pressure deficit(hpa) andlatent heat flux(lh)   with GEE variables i.e temperature and precipitation. 


<img width="452" alt="image" src="https://github.com/clpa123/ML-Algorithms-with-Earth-Observation-Data/assets/107925461/7760333c-1c77-4d2c-bb9b-ffd2799344a2">

Figure 3: The plot depicts the relationship between the target variable, latent heat, along the x-axis, and the independent variables represented on the y-axis.









