# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
Title: Statistical Analysis and Visualization of Restaurant Data in the City of Vancouver

In this project, our focus is on conducting a comprehensive statistical analysis and visualization of restaurant data specifically in the vibrant city of Vancouver. The primary goal is to gain valuable insights into the restaurant landscape, identify popular cuisines, analyze the relationship between restaurant attributes and ratings, and visually represent the findings through meaningful charts and graphs.

To accomplish this, we will gather restaurant data from various sources, including the Yelp and Foursquare APIs, and preprocess it to create a structured and cohesive dataset. Through thorough exploratory data analysis (EDA), we will uncover patterns, trends, and outliers related to restaurant categories, ratings, and geographical distribution within the city.

We will categorize restaurants based on their cuisine types and determine the most sought-after cuisines among Vancouverites. Moreover, a regression model will be constructed to predict restaurant ratings using pertinent features such as location, category, and other relevant attributes.

The data visualization component of the project will involve creating informative and visually appealing charts, scatter plots, bar graphs, and heatmaps to effectively communicate the results of our analysis. The insights derived from this project will not only be of interest to restaurant owners but also valuable to city officials and policymakers, aiding them in making informed decisions to enhance Vancouver's culinary scene and overall dining experience.

By leveraging statistical analysis, and data visualization techniques, this project seeks to provide a comprehensive overview of the restaurant ecosystem in the City of Vancouver and offer actionable recommendations for further enriching the city's diverse(Bikers) and thriving culinary offerings.

## Process
Process:

1. Explore CityBikes API: Understand API structure, endpoints, and available data for bike sharing in various cities.

2. Select City: Choose a specific city covered by CityBikes API to focus on for data retrieval.

3. Query Bike Stations: Use API to retrieve bike station data for the selected city, including latitude, longitude, and available bikes.

4. Connect to Foursquare and Yelp APIs: Establish connections to both APIs for retrieving POI data.

5. Retrieve POI Data: For each bike station, query Foursquare and Yelp APIs to get nearby POI information.

6. Create Dataframes: Parse JSON responses into Pandas dataframes for both Yelp and Foursquare results.

7. Compare APIs: Analyze the coverage and completeness of POI data from Yelp and Foursquare APIs.

8. Merge Data: Join bike station data with POI data to create a comprehensive dataframe.

9. Data Visualization: Utilize charts and visualizations to explore spatial patterns and POI distributions.

10. Build Regression Model: Employ stats models to create a regression model to establish bike-POI relationships.

11. Interpret Model Output: Derive insights from the model to understand how POIs influence bike usage.

12. Explore Classification Approach: Consider transforming regression into a classification problem for further analysis.

13. Create SQLite Database: Establish an SQLite database to store collected POI information.

14. Validate Database: Ensure data integrity and validate the database against the merged dataframe.

15. Generate Insights: Draw valuable conclusions about urban mobility and POI characteristics' impact on bike sharing.

16. Project Documentation: Summarize the process, outcomes, and insights in a clear and concise report.

## Results
Results:

In our analysis, we compared the coverage and quality of data obtained from two APIs, Yelp and Foursquare, for a selected area in the City of Vancouver. We found that both APIs provided valuable information about nearby Points of Interest (POIs) in the vicinity of bike stations. However, there were some differences in the quantity and variety of POIs offered by each API.

Yelp API tended to have more comprehensive coverage of restaurants and eateries, offering detailed information such as reviews and ratings. On the other hand, Foursquare API appeared to excel in providing information about various types of POIs, including parks, landmarks, and recreational facilities.

Regarding the regression model, we attempted to understand the relationship between the number of bikes at bike stations and the characteristics of nearby POIs. However, the model encountered significant challenges due to limited data observations and high multicollinearity among variables. As a result, the model could not provide meaningful insights into the impact of POIs on bike availability.

In conclusion, both Yelp and Foursquare APIs offer valuable data for exploring urban mobility and optimizing bike-sharing services. However, the regression model's limitations call for further data collection and alternative modeling approaches to gain deeper insights into the relationship between bike stations and surrounding POIs. The analysis highlights the importance of data quality and appropriate model selection for accurate and informative urban planning decisions.

## Challenges 
Challenges:

The project encountered challenges due to limited data availability from the CityBikes API, where bike counts were not directly accessible, and we had to use POI counts as a proxy. Varying coverage and quality of POI data from Yelp and Foursquare APIs introduced potential bias. Working with APIs for the first time posed a learning curve for understanding API structure and data extraction. The regression model faced difficulties with few observations versus numerous independent variables, impacting parameter estimation. Multicollinearity further complicated the model, affecting stability and interpretability. These challenges emphasize the need for data quality, validation, and careful consideration of model assumptions for meaningful analysis.

## Future Goals
Future Goals:

Given more time, addressing the limitations and improving the analysis would involve exploring additional data sources or APIs to obtain more accurate and direct information on bike counts at each station. Conducting data validation and cleaning would ensure the accuracy and reliability of the results. Experimenting with different regression models, including non-linear approaches, would be beneficial to better capture the relationship between bike counts and POI characteristics. Additionally, incorporating additional factors such as weather, time of day, and day of the week would enhance the predictive power of the model. These enhancements would lead to a more comprehensive and insightful analysis of the bike-sharing data and its relationship with nearby POIs.
