# Gold Price Prediction

<img src="Images/gold.jpg" alt="Gold Image" width="500">


This is a project assigned from Future Ready Talent sponsored by Microsoft and NPTEL.

Here, I have forecasted gold prices for next 6 months using World Gold Council data for 19 different countries. The main notebook in which I have done data cleaning and model selection is [Indian Gold Price Prediction notebook](https://github.com/akritiupadhyay-au/NPTEL_Microsoft_Project/blob/main/Notebooks/IndianGoldPricePrediction.ipynb).

You can see how gold prices vary differently in different countries every year. The trend of gold price is irregular over all years. This gold price dataset is taken from world gold council and measured in national currency unit per troy ounce. 1 troy ounce is equal to the weight of the gold = 31.1 grams. This dataset contains all the currencies of the world.

## Azure Services Used

1. **Azure Machine Learning Studio**:
     I made a compute instance for the fast processing of my codes.
2. **Visual Studio Code**:
     The following processes I performed in the VS Code:
      (i)   Data cleaning
      (ii)  Model Selection
      (iii) Time Series Forecasting  
3. **Static Web Apps**: I wrote an [index.html](Images/index.html) file for my website, where I used the resulted forecasted plots for 6 months. I created static web app on azure and deployed using github. After deploying, I got the link of my output, and the workflow .yaml file.

## Data Cleaning
1. The data that I collected from [World Gold Council](https://www.gold.org/goldhub/data/gold-prices) has all the prices in object data types.
2. I converted the obejct data type to float data type.
3. I converted the Date to DateTime data type.
4. I selected the data of 10 years i.e., from 2013 till date (2nd October 2023) to predict the gold prices of 19 different countries. 

## Machine Learning Algorithms

I have used the following machine learning algorithms while selecting the model:
1. Logistic Regression
2. Decision Tree Regressor
3. Random Forest Regressor
4. XG Boost Regressor
5. Light GBM Regressor

After comparing all the models, **Random Forest Regressor** did the best with best training and testing accuracy, and there were no overfitting issues. The evaluation metric was **r2 score**. The **training score** was **0.99964** and the **testing score** was **0.997337**. 

## Forecasting using FB Prophet

Prophet has the ability to produce accurate forecasts with minimal effort. It decomposes a time series into three main components: trend, seasonality, and holidays. It automatically detects and handles various types of seasonal patterns, such as daily, weekly, monthly, and yearly seasonality. It can also handle irregular seasonalities.

After verifying the predicted gold price with the selected model, I forecasted the gold price of 19 different countries in 19 different notebooks.

### Output

The output of this implementation can be seen on the website which is made by using [Azure Static Web Apps](https://kind-pond-05f8bb410.3.azurestaticapps.net/). You can select the country to see the forecasted gold price for next 6 months.
