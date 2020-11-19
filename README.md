# Housing Rental & Venues in Gainesville, FL
## Description & Discussion of the Background
Gainesville is a Metropolitan Statistical Area (MSA) and is the largest city in North Central Florida. This city is the county seat and the largest city in Alachua County, Florida. In 2019 the US Census Bureau estimated Gainesville’s population at 133,997, a 7.6% increase compared to 2010, and the MSA population at 288,212.

Gainesville is the home to the University of Florida (UF). The University of Florida is the largest Florida university by student population, and is the fifth largest single-campus university in the United States with 56,567 students enrolled for the fall 2019 semester. Out of all 56,567 students, 3797 were enrolled through UF online. That means 52,770 students were going to the university in person, making 39.38% of the Gainesville population. 

This project will be focused on helping students who are looking to rent an off-campus apartment, but this could help anyone who is looking to rent an apartment in Gainesville. With this, students could find affordable apartments to live near or far from the university. They could also find the most popular venues around their house or university.The students who live with their parents could use this to find the most popular places or if they make a decision to find an apartment to live by themselves, this could facilitate the process. 

## Data Description 
For this project I will be using data from:
* To find apartments for rent in Gainesville I used the [Realtor API](https://rapidapi.com/apidojo/api/realtor). For the apartment data, I only used the address, zip code, latitude, longitude, price minimum, price maximum, sqft minimum, and sqft maximum. I added the average price for each apartment using the min price and the max price, and for the average sqft I used the sqft min and sqft max.
* I used the [Foursquare API](https://developer.foursquare.com) to get the most common venues in a 0.5 miles radius around each apartment given address, latitudes, longitudes, avg prices. Here is my [(dataset)](/Data/apt_and_venues_in_gainesville.csv)
* For Gainesville geo boundaries I used the [UA Census Zip Code Tabulation Areas, 2000 - Florida](https://geo.nyu.edu/catalog/harvard-tg00flzcta). The JSON file had geo-coordinates of all the cities in Florida. To use this file I had to clean the data and reduced it to the city of Gainesville, FL because the file was big and it had data that I didn't need. I used this data to create the choropleth map of the Housing Rental Price Index of Gainesville, FL. Here is my [(dataset)](/GeoJSON/gainesville_geo.json).

## References
* [Gainesville, Fl -Wikipedia](https://en.wikipedia.org/wiki/Gainesville,_Florida)
* [University of Florida - Fall 2019 Enrollment](https://ir.aa.ufl.edu/uffacts/enrollment-1/)
* [Venues in Gainesville, FL - Foursquare API](https://developer.foursquare.com)
* [Apartment for rent in Gainesville, FL - Realtor API](https://rapidapi.com/apidojo/api/realtor)
* [UA Census Zip Code Tabulation Areas, 2000 - Florida](https://geo.nyu.edu/catalog/harvard-tg00flzcta)
