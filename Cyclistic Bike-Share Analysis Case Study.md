**Cyclistic Bike-Share Analysis Case Study**

**Business Task**  
A bike-sharing company, Cyclistic, wants to increase the number of annual memberships. The marketing team aims to convert casual riders into annual members, as they are more profitable long term.

Therefore, the key question for this analysis is:  
How do casual riders and annual members use Cyclistic bikes differently?

**Data Source**  
The data used for this analysis includes 12 months of trip data containing the following details:

- Ride ID  
- Rideable type  
- Start and end timestamps  
- Start and end stations  
- Rider type (member or casual)

The data is publicly available and is provided by Motivate International Inc.

**Data Processing**  
The data was cleaned and prepared for analysis using Python (pandas).

The cleaning process included:

- Importing and combining the 12 monthly CSV files into one dataframe.  
- Converting *started\_at* and *ended\_at* columns to datetime format.  
- Creating a *ride\_length* column to calculate trip duration in minutes.  
- Removing rides shorter than 1 minute to eliminate invalid data.  
- Remove duplicates based on the *ride\_id* column.  
- Removing rows with missing start and end station names.  
- Creating more new columns such as *day\_of\_week, month,* and *hour*.

**Analysis**  
The primary focus of the analysis was on comparing usage patterns between casual riders and annual members.

Key metrics analysed:

- Average ride length  
- Total number of rides  
- Rides by day of month  
- Rides by month  
- Rides by hour  
- Bike type usage

**Key Insights**

- Casual riders have a higher average ride duration compared to members, suggesting they use bikes for leisure rather than commuting.  
- Members take more trips, indicating consistent and repeated usage.  
- Members ride more on weekdays, especially during commuting hours.  
- Casual riders ride more on weekends.  
- While both groups show an increase in bike usage during summer months, the increase is more significant for casual riders, indicating recreational use.

**Visualizations**  
A Tableau dashboard was created to present the findings.

The dashboard includes:

- Total rides by user type  
- Average ride duration by user type  
- Weekly usage pattern  
- Monthly trends  
- Peak riding hours

[*https://public.tableau.com/views/CyclisticBike-ShareAnalysis\_17738341915250/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display\_count=n&:origin=viz\_share\_link*](https://public.tableau.com/views/CyclisticBike-ShareAnalysis_17738341915250/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

**Recommendations**  
Based on the analysis, the following recommendations are proposed:

- Since casual riders are more active on weekends, Cyclistic should promote membership plans during these periods.  
- Seeing the usage increasing during summer months, discounts or limited-time memberships could be introduced.  
- Highlighting cost savings and convenience of membership for frequent riders could also boost membership sales.

