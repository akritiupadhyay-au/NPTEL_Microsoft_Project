# Gold Price Prediction

<img src="Images/gold.jpg" alt="Gold Image" width="500">


This is a project assigned from Future Ready Talent sponsored by Microsoft and NPTEL.

Here, I have forecasted gold prices for next 6 months using World Gold Council data for 19 different countries. The main notebook in which I have done data cleaning and model selection is [Indian Gold Price Prediction notebook](https://github.com/akritiupadhyay-au/NPTEL_Microsoft_Project/blob/main/Notebooks/IndianGoldPricePrediction.ipynb).

You can see how gold prices vary differently in different countries every year. The trend of gold price is irregular over all years. This gold price dataset is taken from world gold council and measured in national currency unit per troy ounce. 1 troy ounce is equal to the weight of the gold = 31.1 grams. This dataset contains all the currencies of the world.

## Forecasting using FB Prophet

Prophet has the ability to produce accurate forecasts with minimal effort. It decomposes a time series into three main components: trend, seasonality, and holidays. It automatically detects and handles various types of seasonal patterns, such as daily, weekly, monthly, and yearly seasonality. It can also handle irregular seasonalities.

### Output

The output of this implementation can be seen on the website which is made by using [Azure Static Web Apps](https://kind-pond-05f8bb410.3.azurestaticapps.net/)
