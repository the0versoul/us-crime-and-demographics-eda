# Predicting Crime Using Demographics: An Exploratory Data Analysis (EDA) 

In this analysis, we are going to try and predict eventually crime rates for a given ZCTA (which closely aligns with USPS zip codes as of 2020) within the United States. We are going to do this using demographics, economic information, and more information from the US census at the ZCTA level. For now, we're going to focus on doing an exploratory data analysis. 

By building a highly interpretable linear model, we can get undeaneath the problem of crime and try and assess what might be driving it, and in what proportion. Is it poverty? Inequality? Crime? Demographic information? These questions hopefully will be answered over the course of this analysis. But first, we must prepare the data for this analysis which comes later. 

The data was sourced from the following sources: 

- https://crimegrade.org/ - This was what we used to obtain the zip-code level crime data. Note that an algorithmic approach is taken to assess crime in Zip codes that don't report crime, so essentially we may be "predicting a prediction" - but nonetheless it is the best dataset available given these constraints. It also doesn't specify what time period this data is from.
- https://console.cloud.google.com/marketplace/product/united-states-census-bureau/us-census-data?project=datarobot-vertex-pipelines - This is a compilation created by Google of publically available census data, which previously was spread out and very hard to aggregate manually. Luckily Google has done much of the hard work for us and created a very wide dataset (nearly 245 columns) for analysis at the ZCTA level. This is "5-year" data and labeled as 2020 level, so we assum that these are five year statistics ending in 2020.

We ultimately join this data together on ZCTA and perform our EDA. 

See the notebook for an intuitive walkthrough! Feel free to reach out with any questions. .