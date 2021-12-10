
![Hotel Cancellation image](https://github.com/Karan-Pruthi/HotelCancellationPrediction/blob/main/images/header.png?raw=true)


# Hotel Booking Cancellation Analysis

This project is to find out the characteristic of customers who cancelled and finding a pattern in their cancelled booking by doing an exploratory data analysis

## Problem Statement
A study conducted by D-Edge Hospitality Solutions found that guests have become accustomed to free cancellation policies that have been made popular. Global average of cancellations had reached almost 40% cancellation rate in 2018-19 before Covid pandemic, this increasing trend year on year produces a very negative impact on hotel revenue and distribution management strategies. This increase in booking cancellation makes it harder for hotels to accurately forecast, leading to non-optimized occupancy and revenue loss and opportunity cost (unsold room due to cancellation).
In reality, ‘Risk Free Reservations’ have the potential to damage a hotel’s brand integrity, increase their dependency on third-party partners and ultimately hurt their bottom line in the long run.
In order to solve this problem, here we will use a real life hotel booking dataset to create a customer segmentation analysis in order to gain insights about the customers (and hopefully reasons why they cancel their reservation)
This can create a surplus value for hotels and OTAs and hence they can take action to prevent these cancellations.
## Context
Have you ever wondered when the best time of year to book a hotel room is? Or the optimal length of stay in order to get the best daily rate? What if you wanted to predict whether or not a hotel was likely to receive a disproportionately high number of special requests?
## Dataset
The dataset is from [Hotel Booking Demand Datasets](https://www.kaggle.com/jessemostipak/hotel-booking-demand) availabe on Kaggle.. This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things. All personally identifying information has been removed from the data. 

• hotel_bookings.csv - the data set contains 119390 records which has 32 different features.
The data is originally from the article [Hotel Booking Demand Datasets](https://www.sciencedirect.com/science/article/pii/S2352340918315191), written by Nuno Antonio, Ana Almeida, and Luis Nunes for Data in Brief, Volume 22, February 2019.

## Data Dictionary
Feature | Type | Description |
--- | --- | --- |
is_canceled | int | Value indicating if the booking was canceled (1) or not (0). |
Hotel | object | (H1 = Resort Hotel or H2 = City Hotel) |
lead_time | int | Number of days that elapsed between the entering date of the booking into the Property Management System and the arrival date. Calculated by subtracting the entering date from the arrival date. |
arrival_date_year | int | Year of arrival date |
arrival_date_month | object | Month of arrival date |
arrival_date_week_number | int | Week number of year for arrival date |
arrival_date_day_of_month | int | Day of arrival date |
stays_in_weekend_nights | int | Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel |
stays_in_week_nights | int | Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel |
adults | int | Number of adults |
children | float | Number of children |
babies | int | Number of babies |
meal | object | Type of meal booked. Categories are presented in standard hospitality meal packages: Undefined/SC – no meal package; BB – Bed & Breakfast; HB – Half board (breakfast and one other meal – usually dinner); FB – Full board (breakfast, lunch and dinner) |
country | object | Country of Origin |
market_segment | object | Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators” |
distribution_channel | object | Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators” |
is_repeated_guest | int | Value indicating if the booking name was from a repeated guest (1) or not (0) |
previous_cancellations | int | Number of previous bookings that were cancelled by the customer prior to the current booking |
previous_bookings_not_canceled | int | Number of previous bookings not cancelled by the customer prior to the current booking |
reserved_room_type | object | Code of room type reserved. Code is presented instead of designation for anonymity reasons. |
assigned_room_type | object | Code for the type of room assigned to the booking. Sometimes the assigned room type differs from the reserved room type due to hotel operation reasons (e.g. overbooking) or by customer request. Code is presented instead of designation for anonymity reasons |
booking_changes | int | Number of changes/amendments made to the booking from the moment the booking was entered on the PMS until the moment of check-in or cancellation |
deposit_type | object | Indication on if the customer made a deposit to guarantee the booking. This variable can assume three categories: No Deposit – no deposit was made; Non Refund – a deposit was made in the value of the total stay cost; Refundable – a deposit was made with a value under the total cost of stay |
agent | float | ID of the travel agency that made the booking |
company | float | ID of the company/entity that made the booking or responsible for paying the booking. ID is presented instead of designation for anonymity reasons |
days_in_waiting_list | int | Number of days the booking was in the waiting list before it was confirmed to the customer |
customer_type | object | Type of booking, assuming one of four categories: Contract - when the booking has an allotment or other type of contract associated to it; Group – when the booking is associated to a group; Transient – when the booking is not part of a group or contract, and is not associated to other transient booking; Transient-party – when the booking is transient, but is associated to at least other transient booking |
ADR | float | Average Daily Rate as defined by dividing the sum of all lodging transactions by the total number of staying nights |
required_car_parking_spaces | int | Number of car parking spaces required by the customer |
total_of_special_requests | int | Number of special requests made by the customer (e.g. twin bed or high floor) |
reservation_status | object | Reservation last status, assuming one of three categories: Canceled – booking was canceled by the customer; Check-Out – customer has checked in but already departed; No-Show – customer did not check-in and did inform the hotel of the reason why |
reservation_status_date | object | Date at which the last status was set. This variable can be used in conjunction with the ReservationStatus to understand when was the booking canceled or when did the customer checked-out of the hotel |


## Exploratory Data Analysis

- Check for Missing Values
- Check for Duplicate Data
- Numerical Varibales
- Distribution of Numerical Variables
- Categorical Features
- Cardinality of Categorical Features
- Checking if there are any Outliers
- Realtionship between Dependent and Independent feature
- Univariate and Multivariate Analysis
- Data Visualization
- Insights based on EDA

## Business Questions

- How many repeated customers cancel their bookings?
- Which Market segment contribute to more cancellations?
- Which are the most busy months in terms of non-cancelled bookings?
- Which month has the highest number of cancelations?
- How much do the guests pay for a room per night?
- How does the price per night vary over the year?
- How many days people stay in each hotel with respect to  market segment?
- How long do people stay at the hotels?
- Where do most of the guests come from?
## Libraries Used

- Pandas
- Numpy
- Matplotlib
- Seaborn
- Plotly
##  References

- [Global Cancellation Rate of Hotel Reservations Reaches 40% on Average](https://hospitalitytech.com/global-cancellation-rate-hotel-reservations-reaches-40-average)
- [Real Cost of Free Cancellations](https://triptease.com/blog/the-real-cost-of-free-cancellations/)
