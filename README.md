# prophet-challenge
# Module 8 Challenge

## Background
> [!Note]
> You’re a growth analyst at Mercado LibreLinks to an external site.. With over 200 million users, Mercado Libre is the most popular e-commerce site in Latin America. You've been tasked with analyzing the company's financial and user data in clever ways to make the company grow. So, you want to find out if the ability to predict search traffic can translate into the ability to successfully trade the stock.
>
> The instructions for this Challenge are divided into four steps, as follows:
>
> Step 1: Find unusual patterns in hourly Google search traffic.
> 
> Step 2: Mine the search traffic data for seasonality.
> 
> Step 3: Relate the search traffic to stock price patterns.
> 
> Step 4: Create a time series model with Prophet.
>

# Instructions

## Step 1: Find Unusual Patterns in Hourly Google Search Traffic

> [!TIP]
> The data science manager asks if the Google search traffic for the company links to any financial events at the company. Or, does the search traffic data just present random noise? To answer this question, pick out any unusual patterns in the Google search data for the company, and connect them to the corporate financial events.
> 
> To do so, complete the following steps:
> 
> Read the search data into a DataFrame, and then slice the data to just the month of May 2020. (During this month, MercadoLibre released its quarterly financial results.) Visualize the results. Do any unusual patterns exist?
> 
> Calculate the total search traffic for the month, and then compare the value to the monthly median across all months.
> 
> Did the Google search traffic increase during the month that MercadoLibre released its financial results? Write your answer in the space provided in the starter file.
> 

## Step 2: Mine the Search Traffic Data for Seasonality

> [!TIP]
> Marketing realizes that they can use the hourly search data, too. If they can track and predict interest in the company and its platform for any time of day, they can focus their marketing efforts around the times that have the most traffic. This will get a greater return on investment (ROI) from their marketing budget.
> 
> To that end, you want to mine the search traffic data for predictable seasonal patterns of interest in the company. To do so, complete the following steps:
> 
> Group the hourly search data to plot the average traffic by the hour of day. Does the search traffic peak at a particular time of day or is it relatively consistent?
> 
> Group the hourly search data to plot the average traffic by the day of the week (for example, Monday vs. Friday). Does the search traffic get busiest on any particular day of the week?
> 
> Group the hourly search data to plot the average traffic by the week of the year. Does the search traffic tend to increase during the winter holiday period (weeks 40 through 52)?
> 
> Are there any time based trends that you can see in the data? Write your answer in the space provided in the starter file.
>

## Step 3: Relate the Search Traffic to Stock Price Patterns

> [!TIP]
> You mention your work on the search traffic data during a meeting with people in the finance group at the company. They want to know if any relationship between the search data and the company stock price exists, and they ask if you can investigate.
> 
> To do so, complete the following steps:
> 
> Read in and plot the stock price data. Concatenate the stock price data to the search data in a single DataFrame.
> 
> Market events emerged during the year of 2020 that many companies found difficult. But, after the initial shock to global financial markets, new customers and revenue increased for e-commerce platforms. Slice the data to just the first half of 2020 (2020-01 to 2020-06 in the DataFrame), and then plot the data. Do both time series indicate a common trend that’s consistent with this narrative?
> 
> Create a new column in the DataFrame named “Lagged Search Trends” that offsets, or shifts, the search traffic by one hour. Create two additional columns:
> 
> “Stock Volatility”, which holds an exponentially weighted four-hour rolling average of the company’s stock volatility
> 
> “Hourly Stock Return”, which holds the percent change of the company's stock price on an hourly basis
> 
> Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns? Write your answer in the space provided in the starter file.
>

## Step 4: Create a Time Series Model with Prophet

> [!TIP]
> Now, you need to produce a time series model that analyzes and forecasts patterns in the hourly search data. To do so, complete the following steps:
>
> Set up the Google search data for a Prophet forecasting model.
> 
> After estimating the model, plot the forecast. How's the near-term forecast for the popularity of MercadoLibre?
> 
> Plot the individual time series components of the model to answer the following questions in the space provided in the starter file:
> 
> What time of day exhibits the greatest popularity?
> 
> Which day of the week gets the most search traffic?
> 
> What's the lowest point for search traffic in the calendar year?
> 

# Requirements

## Find unusual patterns in hourly Google search traffic (25 points)

> [!IMPORTANT]
> Read the search data into a DataFrame. (5 points)
> 
> Slice the data to just the month of May 2020. (5 points)
> 
> Calculate the total search traffic for the month.(5 points)
> 
> Compare the value to the monthly median across all months. (5 points)
> 
> Did the Google search traffic increase during the month that MercadoLibre released its financial results? Write your answer in the space provided in the starter file. (5 points)
>

## Mine the search traffic data for seasonality (20 points)

> [!IMPORTANT]
> Group the hourly search data to plot the average traffic by the hour of day. (5 points)
>
> Group the hourly search data to plot the average traffic by the day of the week (for example, Monday vs. Friday). (5 points)
> 
> Group the hourly search data to plot the average traffic by the week of the year. (5 points)
> 
> Are there any time based trends that you can see in the data? Write your answer in the space provided in the starter file. (5 points)
>

## Relate the search traffic to stock price patterns (35 points)

> [!IMPORTANT]
> Read in and plot the stock price data. (5 points)
>
> Concatenate the stock price data to the search data in a single DataFrame. (5 points)
> 
> Slice the data to just the first half of 2020 (2020-01 to 2020-06 in the DataFrame), and then plot the data. (5 points)
> 
> Create a new column in the DataFrame named “Lagged Search Trends” that offsets, or shifts, the search traffic by one hour. (5 points)
> 
> Create two additional columns:
> 
> “Stock Volatility”, which holds an exponentially weighted four-hour rolling average of the company’s stock volatility. (5 points)
> 
> “Hourly Stock Return”, which holds the percent change of the company's stock price on an hourly basis. (5 points)
> 
> Does a predictable relationship exist between the lagged search traffic and the stock volatility or between the lagged search traffic and the stock price returns? Write your answer in the space provided in the starter file. (5 points)
>

## Create a time series model with Prophet (20 points)

> [!IMPORTANT]
> Set up the Google search data for a Prophet forecasting model. (5 points)
>
> After estimating the model, plot the forecast. (5 points)
>
> Plot the individual time series components of the model. (5 points)
> 
> Answer the following questions in the space provided in the starter file:
> 
> What time of day exhibits the greatest popularity? (2 points)
> 
> Which day of the week gets the most search traffic? (2 points)
> 
> What's the lowest point for search traffic in the calendar year? (1 point)
> 
