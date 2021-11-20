# SQLAlchemy - Surfs Up!

![surfs-up.png](https://github.com/PeiDay/SQLAlchemy-Challenge/blob/main/Images/surfs-up.png?raw=true)

## Background
This project is designed to explore and analyze data of climate database by using **SQLAlchemy ORM queries**, and **Pandas** and **Matplotlib** in Python. A **Flask API** is created to store all the information.

## Climate Analysis and Exploration

### Precipitation Analysis
Retrieve, summarize, and plot the most recent 12 months of precipitation data. 

![precipitation_analysis](https://github.com/PeiDay/SQLAlchemy-Challenge/blob/main/Images/Precipitation_analysis.png?raw=true)


### Station Analysis
Retrieve, summarize, and plot the most recent 12 months of temperature observation data of the most active station.

![station.png](https://github.com/PeiDay/SQLAlchemy-Challenge/blob/main/Images/Station.png?raw=true)


## Climate App
The Weather App Home Page includes available API routes as below:
**/api/v1.0/precipitation**
**/api/v1.0/stations**
**/api/v1.0/tobs**
Enter a start date to retrieve the weather info : **/api/v1.0/yyyy-mm-dd**
Enter a start and end date to retrieve the weather info : **/api/v1.0/yyyy-mm-dd/yyyy-mm-dd**


## Other Analysis

### Temperature Analysis I
#### Is there a meaningful difference between temperatures between the months of June and December?

* **T-test** was used to calculate the means of two different independent samples: __the temperature for June__ vs __temperature for December__ across all available years in the dataset.

* **T-test Results**: t = 30.624201480767336, p = 6.622829250184814e-178

* **Conclusion**: With the __p-value__ is extremely close to 0, there is not sufficient evidence to conclude that there is a significant difference in means between June and December temperatures across all the data years available.
