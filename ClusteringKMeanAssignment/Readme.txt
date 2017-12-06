The Datasets: placesLatitudeAndLongitude.txt
The NoteBook: assignmentWeek3Clustering.ipynb

Data Description: 
 I used the DataSet I found and downloaded in the book Machine Learning in Action of Peter Harrington . The dataSet use  two features the latitude
 and the longitude of 69 observations (addresses)f or clustering.
  
 First it use 69 addresses and the Yahoo!PlaceFinder API to get longitude, the latitude and others information for a given address.
 Second it keep only the latitude and the longitude for the clustering.
  
 So we have 2 features the latitude and the longitude for 69 observations.
  
Descriptive Analysis and Data Validation 
Lack of time to do descriptive analysis on the Features by visualising their distribution and to do some data validation.
  
Result:
Nomber of clusters: 5

Centroids:
[array([  45.59011757, -122.72072414]), 
array([  45.52503436, -122.65800607]), 
array([  45.46639582, -122.761804  ]), 
array([  45.47418175, -122.6232765 ]),
array([  45.52189292, -122.53877368])]

Interpretation
  
  
Data Samples:
PortlandClub.txt (Addresses)
  
Dolphin II	10860 SW Beaverton-Hillsdale Hwy	Beaverton, OR
Hotties	10140 SW Canyon Rd.	Beaverton, OR

Data obtained via Yahoo!PlaceFinder API
Places.txt (Address, Latitude longitude and latitude)

Dolphin II	10860 SW Beaverton-Hillsdale Hwy	Beaverton, OR	45.486502	-122.788346
Hotties	10140 SW Canyon Rd.	Beaverton, OR	45.493150	-122.781021

DataSet Transformed for Kmeans  (clustering)
placesLatitudeAndLongitude.txt (Latitude longitude and latitude for 69 observations)

latitude	longitude
45.486502	-122.788346
45.493150	-122.781021

