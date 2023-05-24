# Hotel_Summer_Data_Analysis

## Objective of this project

Get insights from the year 2016 under resort hotel during summer period (July and August)
Deduce factors contributing to high cancellation rate
Provide recommendations/possible Solutions

## About the Dataset
The dataset contains 119391 columns and 17 rows (Booking ID, Hotel, Booking Date, Arrival Date, , Lead Time, Nights, Guests, Distribution Channel, Customer Type, Country, Deposit Type, Avg Daily Rate, Status, Status Update, Cancelled (0/1), Revenue, Revenue Loss).

## About the Project
This project was carried out using Mainly PowerBi, because the data was clean, the project involved creation of visualization and generation of insight, various measures were created in order to enhance the analytics process.
 
## Measures Used
% Cancelled = 
    DIVIDE([Total Cancelled], [Total # of Transaction], 0)
    
Average_ADR = 
    AVERAGE(Data[Avg Daily Rate])

Total # of Transaction = COUNTROWS(Data)

Total Cancelled Booking = 
    CALCULATE([Total # of Transaction], Data[Cancelled (0/1)] = 0)
    
Total Revenue Made = SUM(Data[Revenue])

Total Revenue Lost = SUM(Data[Revenue Loss])

Since this project is focused on July and August of 2016, the filter pane is used to filter the visuals based on these criteria

![Screenshot 2023-05-24 064015](https://github.com/RaphDeAnalyst/Hotel_Summer_Data_Analysis/assets/76891015/14018d0f-106a-4b74-be35-67682c0cdb2f)

The full report can be found in the [Project Report] (



## Conclusion
1. It was discovered from the analysis that the main contributor to the high cancellatuon rate was high average rate during the summer period
2. Bookings with lead time of 0 to 30 days has higher average lead time and are a contributing factor to the cancellation rate

## Recommendation
- The average daily rate should be reviewed and if possible reduced especially for summer (July and August) bookings with lead time between 0 to 30 days, this will decrease the likelihood of cancellation.
- Although July and August brought in more revenue than other months and had lower number of cancelled booking compared to most months, the revenue lost was the highest, overbooking during the summer will ensure lost of revenue does not affect the generation of revenue during this period.
- Other marketing strategies like target advertising, organization of seasonal events and activities, creation of promotional packages can also be implemented

