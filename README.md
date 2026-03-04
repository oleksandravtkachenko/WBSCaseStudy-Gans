# WBSCaseStudy-Gans
Case Study #4 performed during the WBS DataScienceBootcamp building a local pipeline and migrating it to the cloud

## Project Overview
Gans is a startup developing an e-scooter-sharing system. It aspires to operate in the most populous cities all around the world. In each city, the company will have hundreds of e-scooters parked in the streets and allow users to rent them by the minute.

However, Gans has seen that its operational success depends on something more mundane: having its scooters parked where users need them.

Ideally, scooters get rearranged organically by having certain users moving from point A to point B, and then an even number of users moving from point B to point A. However, some elements create asymmetries. Here are some of them:

In hilly cities, users tend to use scooters to go uphill and then walk downhill.
In the morning, there is a general movement from residential neighbourhoods towards the city centre.
Whenever it starts raining, e-scooter usage decreases drastically.
Young tourists travelling with cheap flights are a big potential group of users, but they need to find scooters downtown or nearby touristic landmarks.

Challenge is going to be:
* to collect data from external sources that can potentially help Gans predict e-scooter movement.
* to assemble and automate a data pipeline in the cloud.
* ***
## Tools Used
Phase 1: Local pipeline:
* Data Collection: web scraping and APIs
* Data Storage: SQL database
Phase 2: Cloud Pipeline:
* GCP MySQL
* Cloud Functions
* Cloud Scheduler
***
## Project Files
* 1_scraping_cities.irynb describes the process of scraping data (cities info (Berlin, Hamburg and Munich)) from websites (Wikipedia) (extract), then transform the data and load to MySQL. 
* 2_api_weather.irynb describes the process of extracting weather data (5 days) for defined cities  (Berlin, Hamburg and Munich) using API and authentication, then transform the data and load to MySQL. 
* 3_api_flights.irynb describes the process of extracting flights data (tomorrow) for 3 cities (Berlin, Hamburg and Munich) using API and authentication, then transform the data and load to MySQL. 
* 4_functions_cloud_sql.irynb describes functions prepared to automate pipeline (weather and flights) on the cloud (Cloud SQL).
***
## Pre-conditions
Setting up accounts for the project: 
1. Sign up for an OpenWeatherMap account
2. Sign up for a Google Cloud Platform (GCP) account

