# Analysis and Results
## Part 1: Determinants of Apartment Prices
The purpose of this analysis is to determine the factors affecting the rental prices of WG and apartments in Hamburg, Germany. As shown in the literature , there are studies that show that factors such as the size of the room or apartment and the location have an effect on the rental price (Ndegwa, 2018; Engerstam et al., 2020; Drafor Amenyah & Fletcher, 2013; Haider & Miller, 2000; Iacono & Levinson, 2011). For this purpose, the variables of size, number of rooms and location were selected from among the data collected from WG-gesucht scraping to examine their relationship with rental price. These variables can be seen in the **final_data.xlsx**. OLS regression method has been used to examine this relationship, and its equation is as follows:

$$
Price = \beta1Size + \beta2Rooms + \beta3near_to_uni + \beta4near_to_airport + beta5near_to_hbf + \beta6near_to_city_center
$$