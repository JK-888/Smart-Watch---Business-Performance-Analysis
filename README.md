# Smart Watch - Business-Performance-Analysis

# Project Background

Cyclistic, a bike-share company in Chicago, launched its program in 2016. Since then, it has grown to a fleet of **5,824 bicycles** across **692 geotracked stations**. The system allows users to unlock bikes from one station and return them to any other station, providing flexibility and convenience.  
Cyclistic offers three types of pricing plans:  
- Single-ride passes
- Full-day passes
- Annual memberships

*Director of Marketing*, has identified a key opportunity to convert **casual riders** into **annual members** to ensure long-term growth and customer retention. I am parterning with the team of data analysts who are responsible for collecting, analyzing, and reporting data that helps guide cyclistic marketing strategy and to analyze casual riders vs. annual members' behavior for developing strategies to convert casual riders to annual memberships.

Insights and recommendations are provided on the following key areas:

- Average Rde Length by Bike Type
- Distinct member types
- Geographic Analysis
- Riding pattern by time
- Weekly Dynamics
  
Detailed report of SQL queries and the process of analysis can be founf here.[link](https://onedrive.live.com/?redeem=aHR0cHM6Ly8xZHJ2Lm1zL2IvYy8xNTZiMWExNjNmMDU2NmU5L0VTX1dHaE9haFdKRnFSdkpiVEJxR3NJQjNmNFFaaGpiTnYyb2prWlRBbm41dmc%5FZT1DWEtSdWg&cid=156B1A163F0566E9&id=156B1A163F0566E9%21s131ad62f859a4562a91bc96d306a1ac2&parId=156B1A163F0566E9%211366&o=OneUp)
Dashboard link of Tableau can be found here.[link](https://public.tableau.com/views/CyclistsBikeRides/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)


# Data Structure & Initial Checks
<img width="233" height="404" alt="Screenshot (8)" src="https://github.com/user-attachments/assets/7aed169f-1114-4293-b94f-b64d557d8b7b" />
<img width="253" height="403" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/04f05ad4-d8bb-4482-9ae8-c80fd54a514a" />
<img width="245" height="414" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/5176fb6f-c844-4ad7-8fb0-94418ab70cc6" />

# Executive Summary


1. **Ride Volume**  
   - Members dominate usage with **5,892 rides**, compared to only **1,808 rides** from casual riders.  
   - Indicates **higher loyalty and consistency** among members.  

2. **Ride Duration**  
   - Casual rides average **185 minutes**, slightly higher than members at **180 minutes**.  
   - Suggests casual users may use bikes for **longer leisure trips**, while members use them more frequently but for shorter commutes.  

3. **Bike Type Preferences**  
   - Members and casual riders both use **classic, docked, and electric bikes**, but **electric bikes show the longest ride durations**.  
   - Opportunity: Promote **premium electric bike benefits** in membership plans.  

4. **Time-of-Day Patterns**  
   - Members: Strong peaks during **morning (7–9 AM)** and **evening (5–7 PM)** → aligned with **commuting hours**.  
   - Casual Riders: More consistent usage throughout the day, indicating **leisure or tourism-driven rides**.  

5. **Weekly Dynamics**  
   - Member rides are consistent across weekdays, peaking on **Tuesdays and Wednesdays**.  
   - Casual riders increase usage on **weekends**, suggesting **recreational trips**.  

6. **Geographic Spread**  
   - Both groups ride heavily around **downtown Chicago and near lakefront areas**, but member rides are **more evenly spread** across the city.  
   - Highlights members use bikes for **everyday mobility**, while casual riders focus on **tourist hotspots**.
  

# Insights Deep Dive



<img width="1706" height="959" alt="Dashboard 1 (2)" src="https://github.com/user-attachments/assets/ad8f04b8-322f-4112-8c0b-d4dca1297c7d" />



Data indicates **members drive the majority of consistent usage**, while **casual riders lean toward leisure-oriented, longer trips**.  
Strategically targeting casual riders with **cost-saving, convenience, and lifestyle-driven campaigns** (especially around **weekends, electric bikes, and central Chicago locations**) can unlock significant membership growth.

<img width="801" height="302" alt="01" src="https://github.com/user-attachments/assets/659dfc9d-7b0f-46dc-8950-d8dc22702c5b" />


- **Ride Duration**  
  - Casual riders: **185 minutes per ride** (slightly longer).  
  - Members: **180 minutes per ride**.  
  - Despite similar durations, **casual rides are less frequent**.  
  - **Electric bikes**: Highest ride times for both groups.  
  - **Docked bikes**: Lowest ride times.



<img width="812" height="196" alt="02" src="https://github.com/user-attachments/assets/73a53ef6-162c-4386-ae63-eba3f48e36c7" />



- **Ride Volume**  
  - Total **member rides = 5,892**  
  - Total **casual rides = 1,808**  
  - Members contribute **3x more usage** compared to casual riders.

<img width="855" height="554" alt="03" src="https://github.com/user-attachments/assets/fe4099b8-7d30-4578-88df-f1f973d0112f" />

**Geographic Trends**  
  - Heavy ride activity is concentrated in **downtown Chicago**, near **tourist attractions and business hubs**.  
  - Members **dominate ride minutes** in these areas.

<img width="740" height="296" alt="04" src="https://github.com/user-attachments/assets/275637c2-d5e1-4c80-9ced-baec27aaa23b" />

- **Time of Day**  
  - Casual riders: **Midday & evening peaks** → leisure/tourism use.  
  - Members: **Morning & late afternoon peaks** → commuting patterns.  

<img width="830" height="342" alt="06" src="https://github.com/user-attachments/assets/c2c8e46c-6cc7-4f37-80e5-3da0df8af3b3" />


- **Day of Week**  
  - Casual riders: **More active on weekends**.  
  - Members: **Dominate weekdays**, with **steady usage** across the week.


# Recommendations

### 1. Convert Casual Riders into Members
- Casual riders account for only **1,808 rides vs. 5,892 rides by members** (3x lower).  
- Despite similar ride durations (**185 mins vs. 180 mins**), casual riders ride less frequently, indicating **potential for conversion** through value-driven campaigns.  
- Offer **discounted weekend passes**, **loyalty programs**, and **“trial-to-membership” promotions** to incentivize casual riders into subscribing.  


### 2. Leverage Weekend & Leisure Usage
- Casual riders are **more active on weekends** and during **midday/evening hours**, showing a **leisure and tourism-driven pattern**.  
- Ride peaks differ:  
  - Members = **morning/evening (commutes)**  
  - Casual = **midday/weekends (leisure)**  
- Create **weekend tourism packages** with local attractions, hotel tie-ins, or bundled **“weekend ride + events” offers** to increase casual usage and memberships.  


### 3. Promote Electric Bikes
- **Electric bikes record the longest ride times** among both casual and member users.  
- Longer ride times indicate **higher perceived value and satisfaction**, especially for **tourists/casuals**.  
- Changes as: 
  - Market electric bikes as **premium, time-saving, and convenient**.  
  - Introduce **exclusive weekend electric-bike passes** to attract high-value casual riders.  


### 4. Target Central Chicago Locations
- Heavy ride activity is concentrated in **downtown Chicago**, near **tourist attractions and business hubs**.  
- Members dominate in these locations, but casual riders are also present, suggesting **untapped conversion opportunities**.  
- Best to: 
  - Deploy **geo-targeted ads & app push notifications** near hotspots.  
  - Offer **location-specific ride discounts** (e.g., first ride free near Millennium Park).  


### 5. Differentiate Messaging for Members vs. Casuals
- Usage patterns are distinct:  
  - Members = **consistent weekday commute users**  
  - Casuals = **weekend & leisure-focused riders**  
- A one-size-fits-all campaign may miss opportunities.  
- For Riders:
  - **Members:** Highlight **time savings, reliability, cost efficiency for daily commutes**.  
  - **Casuals:** Highlight **fun, convenience, lifestyle & leisure benefits**.  







