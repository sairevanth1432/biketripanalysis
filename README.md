# **Bike Share Case Study: Analysis of Ride Patterns and User Behavior**

This project is prepared from this data sheet
[[https://docs.google.com/spreadsheets/d/1v11BtTAuR-FhgKZJSHmoqgIeyiapbV5sYzWDtKT3ZDY/edit?usp=sharing]{.underline}](https://docs.google.com/spreadsheets/d/1v11BtTAuR-FhgKZJSHmoqgIeyiapbV5sYzWDtKT3ZDY/edit?usp=sharing)

This sheet was cleaned and manipulated using power query in MS Excel

## **Executive Summary**

This case study analyzes a comprehensive dataset from a bike share
program, detailing ride counts, rideable types, user categories (casual
and member), and ride durations across days and months. The dataset,
covering a full year, includes 5,906,269 rides, with 3,741,315 by
members and 2,164,954 by casual users. The analysis reveals distinct
patterns in ride frequency, user preferences for rideable types, and
seasonal trends, providing actionable insights for optimizing operations
and marketing strategies.

## **Introduction**

The bike share program offers three rideable types: classic bikes,
electric bikes, and electric scooters. Users are categorized as either
members (subscribers) or casual riders (pay-per-use). The dataset
provides ride counts by day, month, ride duration, and rideable type,
enabling a detailed examination of usage patterns. This study aims to:

-   Identify peak usage days and months.

-   Compare member and casual rider behaviors.

-   Analyze ride duration distributions.

-   Assess the popularity of rideable types.

-   Highlight seasonal trends and operational opportunities.

## **Methodology**

The dataset, originally in Excel format, was analyzed to extract key
metrics. The data includes:

-   **Ride Counts by Day**: Total rides by day of the week, split by
    > user type.

-   **Rideable Type Usage**: Ride counts for classic bikes, electric
    > bikes, and electric scooters, segmented by user type.

-   **Ride Duration**: Rides categorized into four duration bins (less
    > than 10 minutes, 10 to 30 minutes, 30 to 60 minutes, over 60
    > minutes).

-   **Monthly Trends**: Ride counts by month, day, and user type for
    > classic and electric bikes, with limited data for electric
    > scooters (primarily September).

Data was aggregated and visualized to identify trends. Key assumptions:

-   The dataset represents a full year of operations.

-   Missing duration data for some rideable types (e.g., electric
    > scooters outside September) was excluded from duration analysis.

-   Ride counts are accurate and reflect actual usage.

## **Analysis and Findings**

### **1. Ride Counts by Day of the Week**

The dataset shows a total of 5,906,269 rides, with members accounting
for 63.3% (3,741,315) and casual users 36.7% (2,164,954). Ride
distribution by day reveals distinct patterns:

  ------------------------------------------------------------------------
  **Day**      **Casual        **Member Rides** **Total       **% of
               Rides**                          Rides**       Total**
  ------------ --------------- ---------------- ------------- ------------
  Monday       251,548         528,457          780,005       13.2%

  Tuesday      231,970         568,412          800,382       13.5%

  Wednesday    271,948         618,053          890,001       15.1%

  Thursday     268,310         581,290          849,600       14.4%

  Friday       321,033         538,201          859,234       14.5%

  Saturday     448,859         487,682          936,541       15.9%

  Sunday       371,286         419,220          790,506       13.4%
  ------------------------------------------------------------------------

**Key Observations**:

-   **Peak Day**: Saturday has the highest ride count (936,541), driven
    > by casual riders (448,859), suggesting recreational use dominates
    > weekends.

-   **Member Usage**: Members ride most on Wednesdays (618,053),
    > indicating commuting patterns during midweek.

-   **Casual vs. Member**: Casual riders peak on Saturdays (20.7% of
    > their total rides), while members have more consistent usage, with
    > a slight peak midweek.

**Interesting Fact**: Despite members outnumbering casual riders
overall, casual riders contribute nearly half (47.9%) of Saturday rides,
highlighting their preference for weekend leisure activities.

### **2. Rideable Type Usage**

The dataset breaks down rides by rideable type:

  ------------------------------------------------------------------------
  **Rideable       **Casual       **Member        **Total      **% of
  Type**           Rides**        Rides**         Rides**      Total**
  ---------------- -------------- --------------- ------------ -----------
  Classic Bike     982,282        1,787,410       2,769,692    46.9%

  Electric Bike    1,097,457      1,894,783       2,992,240    50.7%

  Electric Scooter 85,215         59,122          144,337      2.4%
  ------------------------------------------------------------------------

**Key Observations**:

-   **Electric Bikes Dominate**: Electric bikes account for 50.7% of
    > rides, with members (63.3% of electric bike rides) showing a
    > slight preference over casual riders.

-   **Classic Bikes**: Classic bikes are popular among members (64.5% of
    > classic bike rides), possibly due to cost savings or fitness
    > preferences.

-   **Electric Scooters**: Scooters have the lowest usage (2.4%), with
    > limited data (mostly September), suggesting they may be a newer or
    > less promoted option.

**Insight**: The high adoption of electric bikes suggests users value
convenience and speed, particularly for longer or urban commutes.

### **3. Ride Duration Analysis**

Ride durations are categorized into four bins, with detailed data for
classic and electric bikes across all months and limited data for
electric scooters (September only). A sample of ride counts for classic
bikes (member, 10 to 30 minutes) by month illustrates seasonal trends:

  --------------------------------------------------------------------------------------------------------------
  **Month**   **Sunday**   **Monday**   **Tuesday**   **Wednesday**   **Thursday**   **Friday**   **Saturday**
  ----------- ------------ ------------ ------------- --------------- -------------- ------------ --------------
  1           1,469        3,345        3,322         4,570           3,622          2,052        1,658

  2           3,831        5,405        6,846         5,980           7,683          4,831        3,088

  3           5,051        5,820        6,063         5,766           4,834          4,435        6,182

  4           6,211        8,781        9,748         5,729           5,787          5,210        7,103

  5           8,206        8,495        9,334         15,217          11,914         12,170       11,135

  6           13,042       10,593       11,371        13,119          12,243         10,534       11,439

  7           8,500        13,096       14,262        15,979          11,975         11,335       11,911

  8           10,163       9,720        10,486        12,384          13,249         12,486       13,591

  9           9,551        12,443       10,607        12,360          11,723         9,399        9,550

  10          7,304        7,838        11,359        12,270          10,920         8,248        8,351

  11          4,446        5,160        5,584         5,198           4,296          6,190        5,105

  12          3,071        3,305        3,567         4,534           4,614          4,539        3,920
  --------------------------------------------------------------------------------------------------------------

**Key Observations**:

-   **Short Rides Dominate**: Across all rideable types, rides under 10
    > minutes are the most common, suggesting users primarily use the
    > service for quick trips (e.g., commuting or errands).

-   **Casual Riders**: Casual riders have a higher proportion of longer
    > rides (30 to 60 minutes and over 60 minutes), particularly on
    > weekends, indicating recreational use.

-   **Members**: Members favor shorter rides (less than 10 minutes and
    > 10 to 30 minutes), consistent with commuting patterns.

-   **Electric Scooters**: In September, scooters show a similar pattern
    > to bikes, with most rides under 10 minutes, but casual riders have
    > more 30 to 60-minute rides.

**Insight**: The prevalence of short rides suggests docking stations
should be strategically placed in high-traffic urban areas to facilitate
quick trips.

### **4. Seasonal Trends**

Ride counts peak in summer months (June to August) and decline in winter
(December to February):

-   **Peak Month**: August sees the highest ride counts, particularly
    > for casual riders (e.g., 18,384 classic bike rides on Saturdays,
    > 10 to 30 minutes).

-   **Low Season**: January and February have the lowest ride counts,
    > with members maintaining more consistent usage than casual riders.

-   **Shoulder Seasons**: Spring (March to May) and fall (September to
    > November) show moderate usage, with a noticeable uptick in May and
    > September.

**Interesting Fact**: Casual riders' usage spikes dramatically in
summer, with Sunday rides in September (11,705 classic bike rides, 10 to
30 minutes) nearly tripling January levels (372 rides). This suggests
weather significantly influences casual rider behavior.

## **Visualizations**

The following visualizations were generated to illustrate key findings:

1.  **Bar Chart: Rides by Day of the Week\
    > **

    -   Shows Saturday as the peak day, with casual riders driving
        > weekend spikes.

    -   Members have higher midweek usage (Tuesday to Thursday).

2.  **Pie Chart: Rideable Type Distribution\
    > **

    -   Electric bikes (50.7%) lead, followed by classic bikes (46.9%)
        > and scooters (2.4%).

    -   Highlights member preference for classic bikes and casual rider
        > preference for electric bikes.

3.  **Line Chart: Monthly Ride Trends\
    > **

    -   Displays seasonal peaks in summer (June to August) and lows in
        > winter (December to February).

    -   Casual riders show sharper seasonal fluctuations than members.

4.  **Stacked Bar Chart: Ride Duration by User Type\
    > **

    -   Short rides (less than 10 minutes) dominate for both user types.

    -   Casual riders have a higher share of longer rides (over 30
        > minutes).

## **Discussion**

The analysis reveals distinct user behaviors:

-   **Members**: Likely commuters, with consistent midweek usage,
    > preference for shorter rides, and slight preference for classic
    > bikes. Their usage is less sensitive to seasonal changes.

-   **Casual Riders**: Primarily recreational users, with weekend peaks,
    > longer ride durations, and a preference for electric bikes. Their
    > usage drops significantly in colder months.

-   **Rideable Types**: Electric bikes are the most popular, likely due
    > to ease of use and speed. Classic bikes remain competitive among
    > members, possibly due to lower costs or fitness benefits. Electric
    > scooters, with limited data, show potential for short urban trips.

**Operational Implications**:

-   **Fleet Management**: Increase electric bike availability during
    > summer and weekends to meet casual rider demand. Ensure classic
    > bike availability midweek for members.

-   **Station Placement**: Prioritize docking stations in urban centers
    > for short trips, with additional stations in recreational areas
    > (e.g., parks) for weekend casual riders.

-   **Marketing**: Target casual riders with summer promotions and
    > electric bike incentives. Offer member discounts in winter to
    > maintain usage.

-   **Seasonal Adjustments**: Scale down fleet size in winter, focusing
    > on member needs, and ramp up in summer for casual riders.

## **Conclusion**

The bike share program serves a diverse user base, with members driving
consistent commuting usage and casual riders fueling recreational peaks.
Electric bikes are the most popular rideable type, particularly among
casual riders, while classic bikes remain relevant for members. Seasonal
trends highlight the need for flexible fleet management and targeted
marketing to maximize ridership. By aligning operations with these
insights---prioritizing electric bikes in summer, optimizing station
locations, and tailoring promotions---the program can enhance user
satisfaction and operational efficiency.

## **Recommendations**

1.  **Fleet Optimization**: Increase electric bike availability in
    > summer and weekends; maintain classic bike supply for midweek
    > commuting.

2.  **Station Strategy**: Expand docking stations in urban hubs for
    > short trips and recreational areas for casual riders.

3.  **Marketing Campaigns**:

    -   Summer promotions for casual riders, emphasizing electric bikes.

    -   Winter incentives for members to sustain usage.

4.  **Data Expansion**: Collect full-year data for electric scooters to
    > assess their potential and refine usage patterns.

5.  **Maintenance Scheduling**: Schedule maintenance in winter to
    > minimize disruption during peak summer months.
