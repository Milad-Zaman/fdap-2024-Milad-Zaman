# Analysis and Results
## Part 1: Determinants of Apartment Prices
The purpose of this analysis is to determine the factors affecting the rental prices of WG and apartments in Hamburg, Germany. As shown in the literature , there are studies that show that factors such as the size of the room or apartment and the location have an effect on the rental price (Ndegwa, 2018; Engerstam et al., 2020; Drafor Amenyah & Fletcher, 2013; Haider & Miller, 2000; Iacono & Levinson, 2011). For this purpose, the variables of size, number of rooms and location were selected from among the data collected from WG-gesucht scraping to examine their relationship with rental price. The data of these variables can be seen in the **final_data.xlsx**. OLS regression method has been used to examine this relationship, and its equation is as follows:

$$
Price = \beta_0 + \beta_1Size + \beta_2Rooms + \beta_3near-to-uni + \beta_4near-to-airport + \beta_5near-to-hbf + \beta_6near-to-city-center
$$

where:
- Price: the rental price in €.
- Size : size of the room in m².
- Rooms: number of rooms
- near-to-uni: dummy variable if the location of apartment is near to the university of Hamburg 1, otherwise 0.
- near-to-airport: dummy variable if the location of apartment is near to the airport 1, otherwise 0.
- near-to-hbf: dummy variable if the location of apartment is near to the central train stiation of Hamburg 1, otherwise 0.
- near-to-city-center: dummy variable if the location of apartment is near to the city center of Hamburg 1, otherwise 0.

The results of the OLS can be seen in this table:
![OLS price](/workspaces/fdap-2024-Milad-Zaman/Apartment_Analysis/6.Results/OLS price.PNG)