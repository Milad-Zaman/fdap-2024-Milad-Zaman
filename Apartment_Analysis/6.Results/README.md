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

The results of the OLS can be seen in the first table in **Data analysis.ipynb**.

As can be seen in the table, the number of observations is 350 and it means the regression conducted with data of 350 Ads of WG and apartments in WG-gesucht in Hamburg. The intercept **(const =490.7953)** representing the baseline rental price when all other variables are zero. This is the price of an apartment that is not near any of the listed locations and has zero size and rooms, which is more of a statistical artifact rather than a practical scenario.

The **Size (2.9803)** shows that each additional square meter of the room size is associated with an increase in rent by approximately €2.98, holding other factors constant and it is significant statistically. **Rooms (18.7484)** means each additional room is associated with an increase in rent by approximately €18.75, holding other factors constant. This is also significant statistically.

Apartments near the university **(near_to_uni=50.2030)** are associated with an increase in rent by approximately €50.20, significant at the 5% level. Proximity to the airport **(near_to_airport =-0.7245)**  has a negligible and statistically insignificant effect on rent (p = 0.986). Proximity to the central train station **(near_to_hbf =11.9299)** has a positive but statistically insignificant effect on rent (p = 0.719) and **near_to_city_center (5.4630)** has a small and statistically insignificant effect on rent (p = 0.849).

Based on these results larger apartments with more rooms have higher rents, as they offer more living space and possibly more amenities. This is consistent with the economic principle that more desirable and larger housing units have higher prices. In addition apartments near the university are significantly more expensive, likely due to high demand from students and university staff. This area may have additional amenities and services catering to the university community, increasing its attractiveness and rental prices.

In conclusion, the size of the apartment, the number of rooms, and how close it is to the university are key factors in setting rental prices in Hamburg. But it also suggests that being close to the airport, the centeral train station, or the city center doesn't significantly affect rent prices. This might mean that more research or different factors need to be considered to understand their impact better.