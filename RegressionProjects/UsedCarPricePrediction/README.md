<center><span style="font-family: TimesNewRoman; font-size:1.4em;color:blue;"><b>  LinearRegression:  Predict Price for Used Car in India</b></span></center><br>
<center><img src=https://images.unsplash.com/photo-1506883968894-6e7738ccfc05?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80 width="400" height="300"></center>
<p size=1 ><i>image source:Meriç Dağlı on Unsplash</i></p>
<br>

## Context
    
<p style = "font-size : 15px ; color: black;font-family:TimesNewRoman">
There is a huge demand for used cars in the Indian Market today. As sales of new cars have slowed down in the recent past, the pre-owned car market has continued to grow over the past years and is larger than the new car market now. Cars4U is a budding tech start-up that aims to find footholes in this market.
In 2018-19, while new car sales were recorded at 3.6 million units, around 4 million second-hand cars were bought and sold. There is a slowdown in new car sales and that could mean that the demand is shifting towards the pre-owned market. In fact, some car sellers replace their old cars with pre-owned cars instead of buying new ones. Unlike new cars, where price and supply are fairly deterministic and managed by OEMs (Original Equipment Manufacturer / except for dealership level discounts which come into play only in the last stage of the customer journey), used cars are very different beasts with huge uncertainty in both pricing and supply. Keeping this in mind, the pricing scheme of these used cars becomes important in order to grow in the market. We have to come up with a pricing model that can effectively predict the price of used cars and can help the business in devising profitable strategies using differential pricing.</p>


<p style = "font-size : 20px ; color: black;font-family:TimesNewRoman">
    <b>Table of Contents</b>
</p><br>
<p style = "font-size : 15px ; color: black;font-family:TimesNewRoman">
    
- [Data Set](#Data-Set)

-  [Problem](#Problem)

- [Libraries](#Libraries)

- [Read and Understand Data](#Read-and-Understand-data)

- [Data Preprocessing](#Data-Preprocessing)
    
- [Basic EDA](#EDA)    
    
- [Handling Missing Value](#Handling-missing-values)
    
- [Exploratory Data Analysis](#Exploratory-Data-Analysis) 
    
- [Insights based on EDA](#Insights-based-on-EDA)
  
- [Model Building](#Model-Building)
    
- [Test Assumptions](#Test-Assumptions) 
    
- [Recommendation](#Recommendation)

<br>

## Data Set
    
<br>
<p style = "font-size : 15px ; color: black;font-family:TimesNewRoman">
    
1. S.No. : Serial Number<br>
    
2. Name : Name of the car which includes Brand name and Model name<br>
    
3. Location : The location in which the car is being sold or is available for purchase Cities<b<br>r>
    
4. Year : Manufacturing year of the car<br>
    
5. Kilometers_driven : The total kilometers driven in the car by the previous owner(s) in KM.<br>
    
6. Fuel_Type : The type of fuel used by the car. (Petrol, Diesel, Electric, CNG, LPG)<br>
    
7. Transmission : The type of transmission used by the car. (Automatic / Manual)<br>
    
8. Owner : Type of ownership<br>
    
9. Mileage : The standard mileage offered by the car company in kmpl or km/kg<br>
    
10. Engine : The displacement volume of the engine in CC.<br>
    
11. Power : The maximum power of the engine in bhp.<br>
    
12. Seats : The number of seats in the car.<br>
    
13. New_Price : The price of a new car of the same model in INR Lakhs.(1 Lakh = 100, 000)<br>
    
14. Price : The price of the used car in INR Lakhs (1 Lakh = 100, 000)<br>
</p>  

## Problem
<p style = "font-size : 15px ; color: black;font-family:TimesNewRoman">

- Does various predicating factors effect the price of the used car .?<br>
- What all  independent variables effect the pricing of used cars?<br>
- Does name of a car have any effect on  pricing of car.?<br>
- How does type of Transmission  effect  pricing?<br>
- Does Location in which the car being sold has any effect on the price?<br>
- Does kilometers_Driven,Year of manufacturing  have negative correlation with  price of the car?<br>
- Does Mileage ,Engine and Power have any effect on the pricing of the car?<br>
- How does number of seat ,Fuel type effect the pricing.?<br>
</p>