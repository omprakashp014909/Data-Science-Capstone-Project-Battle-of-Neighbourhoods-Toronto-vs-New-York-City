# Data-Science-Capstone-Project-Battle-of-Neighbourhoods-Toronto-vs-New-York-City
----
This project is part of IBM Data Science Professional Certificate and aims to reveal some insights for the people who wants to immigrate to Toronto or New York City.

# Problem
---

> **Say, You are planning immigration to either Toronto, Canada or New York City, USA for better life prospects like education, earnings, security and many more. You live in India and love your neighbourhood mainly beacause of all the great amenities and venues that exist in your neighbourhood such as fast food centres, pharmacies, schools, markets, shopping malls, parks, hospitals and so on. You want to know, which city among Toronto and New york city will be economical, safer and similar to your current neighborhood.**


* **`Factors to consider`**
    > **For comparing the similarities between the two cities, we will consider the venues available in  neighborhoods and the housing prices. These are some of the most crucial factors one should take into account while immigration.**

---

# Data

---
  
* We will need the location data such as postal codes, boroughs, latitude and longitude, housing price data and crime data of the neighborhoods of respective cities. As the sources of the data for both the cities will be different, for fair comparison we need to make sure that  parameters should be common to both the cities and lie in same time frame.

### `1.Location Data`
* **`About data`**
> * For New York City, all the data is available in .csv format
> * For Torornto, we will web srape the wikipedia page to grab postal codes, boroughs and neighborhoods and then will merged them with a dataset containing respective latitudes and longitudes.
> * It will be used for segmenting the neighborhoods based on the venues and plot maps for rest of the data.
> * Foursquare REST API will be used to grab the venues in the neighborhood
* **`Sources`**
> * New York City(JSON) : https://cocl.us/new_york_dataset
> * Toronto's Postal Code, Borough and Neighborhoods data : https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M
> * Toronto's Geospatial data : https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/labs_v1/Geospatial_Coordinates.csv


### `2.Housing Data`
* **`About data`**
> * For New York city, we will use web scrapping to scrape the information from city-data and then use the uszipcode library to grab the zipcodes.
> * For Toronto, the housing dataset is hosted on Kaggle
> * For fair comparison, the prices will be converted to same unit and will be maintained within limit.
* **`Source`**
> * New York City : http://www.city-data.com/zipmaps/New-York-New-York.html
> * Toronto : https://www.kaggle.com/mnabaee/ontarioproperties

* **We will compare the two cities based on the venues and the housing prices available in their neighborhoods and will find which is better for immigration**
