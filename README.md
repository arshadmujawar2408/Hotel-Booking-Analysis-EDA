# EDA for Hotel-Booking-Analysis
The project contains the real world data record of hotel bookings of a city and a resort hotel containing details like bookings, cancellations, guest details etc. from 2015 to 2017. In this project we are going to analyze Hotel Booking Data in order to find out valuable insights and give suggestions to increase revenue of hotels.

**Programming Language** : Python

**Libraries used** : Pandas, Numpy, Matplotlib, Seaborn

**Notebook** : Google Colab

**Dataset Source** : Provided by Almabetter themself.

## Objective
We are provided with a hotel bookings dataset.

The main purpose of this study is to perform EDA on the given dataset and draw useful conclusions about the trends in hotel bookings and how factors that control hotel bookings influence each other.

## Dataset 
We are given a hotel bookings dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features.
```
- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.
```

- Total number of rows in data: 119390
- Total number of columns: 32

## Data Cleaning and Manipulation

### (1) Handling null values
Null values in columns `company` and `agent` were dropped.

### (2) Removing Duplicate rows
All duplicate rows were dropped.

### (3) Identify Continuous and Categorical Variables
The dataset consists of 12 continuous variables and 18 categorical variables. 

### (3) Converting columns to appropriate naming conventionsdata types

## Data Preparation
#

 1) Combine the categories of children and babies into a single category called "kids."
 2) Calculate the total number of bookings by adding the counts of kids and adults.
 3) Convert the data types of the following columns to string: ArrivingYear, ArrivingMonth, ArrivingDate, Canceled, and RepeatGuest.
 4) Convert the arrival date column to the datetime data type for accurate date and time calculations and analysis.


## Exploratory Data Analysis

Performed EDA and tried answering the following questions:

```
 Q1) Which hotel has more no of bookings and What is the  percentage of bookings in each hotel ?
 Q2) Hotel Wise Bookings based on Month and year also What is the trend of bookings within a month ?
 Q3) Which meal type is the  most preffered meal of customers ?
 Q4) Which room type is in most demand and which room type generates the  highest average daily rate?
 Q5) How long do people stay at the hotels?
 Q6) What is preferred stay length in each hotel based on weekday nights and weekend nights ?
 Q7) Which Booking is preffered with the deposite type?
 Q8) Cancellation rates in both the hotels also arival year and  lead time?
 Q9) What is the Average daily rate month wise also which are the most busy months??
 Q10) What is the Average daily rate with respect to per person?
 Q11) Which types of customers mostly make bookings?
```

Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
   - Bar Plot.
   - Count Plot
   - Pie Chart.
   - Line Plot.
   - Heatmap.
   - Box Plot
             
## Analysis:

Performed analysis and made following conclusions:
```
1} Cancellations: Approximately 27% of the bookings, amounting to 23,987 bookings, were canceled.
2} Bookings by Country: The majority of bookings, around 31%, were made from Portugal, followed by Great Britain with 12% and France with 10%.
3} Occupancy by Month: August is the busiest month with 12.91% of the bookings, while January is the least occupied month with only 5.33% of the bookings.
4} Booking Channels: Around 59% of the bookings were made through Online Travel Agents (OTAs), approximately 15% through Offline Travel Agents, and less than 13% were direct bookings without involving any other agents.
5} Bookings by Year: In terms of the distribution of bookings over the years, 48% were made in 2016, 36% in 2017, and 15% in 2015, indicating an increasing trend in bookings year by year.
6} Meal Preferences: The most ordered meal option was Bed & Breakfast (BB), accounting for approximately 77.7% of the bookings. This was followed by bookings without any meal package specified (SC), Half Board (HB), Undefined, and Full Board (FB).
7} Customer Type: The majority of customers, around 82%, belonged to the Transient customer type, indicating a higher proportion of individual and short-stay guests.
8} Check-Out and Cancellation Rates: Approximately 72% of the visitors checked out as planned, while 26% of the bookings were canceled.
```
## Conclusion

```
1} Majority of the hotels booked are city hotel. Definitely need to spend the most targeting fund on those hotel.
2} We also realise that the high rate of cancellations can be due high no deposit policies.
3} We should also target months between May to Aug. Those are peak months due to the summer period.
4} Majority of the guests are from Western Europe. We should spend a significant amount of our budget on those area.
5} Given that we do not have repeated guests, we should target our advertisement on guests to increase returning guests.	
6} Bed and Breakfast (BB) is the most preferred meal package, indicating the potential to introduce offers and promotions for other meal packages like Full Board (FB) to increase revenue.
7) The distribution channel TA/TO (Travel Agents/Tour Operators) accounts for 80% of bookings, highlighting the importance of collaborating with these channels for marketing and promotions.
And many more conclusions.
```
## Challenges
```
(1) Lot of null values were present in the dataset.
(2) Data type of some Data was in wrong format.
(3) Lot of duplicate data.
(4) Which visualization techniques to use was a challenge?
