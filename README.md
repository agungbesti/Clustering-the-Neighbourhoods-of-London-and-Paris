# Clustering the Neighbourhoods of London and Paris (Project from Coursera)


## Information Obtained :

### Introduction

- A Tale of Two cities, a novel written by Charles Dickens was set in London and Paris which takes place during the French Revolution. These cities were both happening then and now. A lot has changed over the years and we now take a look at how the cities have grown. London and Paris are quite the popular tourist and vacation destinations for people all around the world. They are diverse and multicultural and offer a wide variety of experiences that is widely sought after. We try to group the neighbourhoods of London and Paris respectively and draw insights to what they look like now


### Business Problem


- The aim is to help tourists choose their destinations depending on the experiences that the neighbourhoods have to offer and what they would want to have. This also helps people make decisions if they are thinking about migrating to London or Paris or even if they want to relocate neighbourhoods within the city. Our findings will help stakeholders make informed decisions and address any concerns they have including the different kinds of cuisines, provision stores and what the city has to offer.


### Data Description


- We require geographical location data for both London and Paris. Postal codes in each city serve as a starting point. Using Postal codes we use can find out the neighborhoods, boroughs, venues and their most popular venue categories.


### Methodology

- Data Collection
  - In the data collection stage, we begin with collecting the required data for the cities of London and Paris. We need data that has the postal codes, neighbourhoods and boroughs specific to each of the cities.

- Data Preprocessing
  - For London, We replace the spaces with underscores in the title.The borough column has numbers within square brackets that we remove.

- Feature Selection
  - For both of our datasets, we need only the borough, neighbourhood, postal codes and geolocations (latitude and longitude).

- Feature Engineering
  - Both of our Datasets actually contain information related to all the cities in the country. We can narrow down and further process the data by selecting only the neighbourhoods pertaining to 'London' and 'Paris'.

- Visualizing the Neighbourhoods of London and Paris
  - Now that our datasets are ready, using the Folium package, we can visualize the maps of London and Paris with the neighbourhoods that we collected. 
  - Neighbourhood map of London:
    
    
   ![1](https://user-images.githubusercontent.com/35904444/102927555-c63e0280-44c9-11eb-9883-44c28c40aa86.PNG)
  
  
  - Neighbourhood map of Paris:
  
  
    ![2](https://user-images.githubusercontent.com/35904444/102927502-b6262300-44c9-11eb-8170-48abe271deee.PNG)
  
  
- One Hot Encoding
  - Since we are trying to find out what are the different kinds of venue categories present in each neighbourhood and then calculate the top 10 common venues to base our similarity on, we use the One Hot Encoding to work with our categorical datatype of the venue categories. This helps to convert the categorical data into numeric data.
  
  ![3](https://user-images.githubusercontent.com/35904444/102927520-bc1c0400-44c9-11eb-9dfc-fef0cc595c42.PNG)
  
  
- Top Venues in the Neighbourhoods
  - In our next step, We need to rank and label the top venue categories in our neighborhood.
  
- Model Building - KMeans
  - Moving on to the most exicitng part - Model Building! We will be using KMeans Clustering Machine learning algorithm to cluster similar neighbourhoods together. We will be going with the number of clusters as 5.
 
 - Visualizing the clustered Neighbourhoods
 
 
 ![4](https://user-images.githubusercontent.com/35904444/102927524-bcb49a80-44c9-11eb-9066-70a15d1d9972.PNG)
 
 
 ![5](https://user-images.githubusercontent.com/35904444/102927543-c211e500-44c9-11eb-972f-30b5bec63dac.PNG)


### Results and Discussion

The neighbourhoods of London are very mulitcultural. There are a lot of different cusines including Indian, Italian, Turkish and Chinese. London seems to take a step further in this direction by having a lot of Restaurants, bars, juice bars, coffee shops, Fish and Chips shop and Breakfast spots. It has a lot of shopping options too with that of the Flea markets, flower shops, fish markets, Fishing stores, clothing stores. The main modes of transport seem to be Buses and trains. For leisure, the neighbourhoods are set up to have lots of parks, golf courses, zoo, gyms and Historic sites. Overall, the city of London offers a multicultural, diverse and certainly an entertaining experience.

Paris is relatively small in size geographically. It has a wide variety of cusines and eateries including French, Thai, Cambodian, Asian, Chinese etc. There are a lot of hangout spots including many Restaurants and Bars. Paris has a lot of Bistro's. Different means of public transport in Paris which includes buses, bikes, boats or ferries. For leisure and sight seeing, there are a lot of Plazas, Trails, Parks, Historic sites, clothing shops, Art galleries and Museums. Overall, Paris seems like the relaxing vacation spot with a mix of lakes, historic spots and a wide variety of cusines to try out.

### Conclusion
  
The purpose of this project was to explore the cities of London and Paris and see how attractive it is to potential tourists and migrants. We explored both the cities based on their postal codes and then extrapolated the common venues present in each of the neighbourhoods finally concluding with clustering similar neighbourhoods together.

We could see that each of the neighbourhoods in both the cities have a wide variety of experiences to offer which is unique in it's own way. The cultural diversity is quite evident which also gives the feeling of a sense of inclusion.

Both Paris and London seem to offer a vacation stay or a romantic getaway with a lot of places to explore, beautiful landscapes, amazing food and a wide variety of culture. Overall, it's upto the stakeholders to decide which experience they would prefer more and which would more to their liking.  
