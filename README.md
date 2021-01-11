# Project 03: Company Fleet Selection Using Weighted Scoring
> This project explores an analysis using the weighted scoring method on selecting one of the four vehicles as part of the company fleet: 2019 Ford Escape, 2019 Honda CR-V, 2019 Hyundai Santa Fe, and 2019 Toyota RAV4. The requirements for the vehicles are based on safety features, maintenance cost, price point, insurance, fuel economy, and resale value. In order to present this analysis to management on car selection, a data visualization tool, Tableau, is used to present my decision.


testing part 3 and 3
adfahdufa
adgnjajkdgf
adgfadg


Table of Contents
---
1. [General Information](#general-information)
2. [Summary](#summary)
3. [Tech Stack](#tech-stack)
4. [Code Examples](#code-examples)

<a name="https://github.com/sangtvo/US-Census-Bureau-Web-Scraper#general-information"/>
<a name="https://github.com/sangtvo/US-Census-Bureau-Web-Scraper#summary"/>
<a name="https://github.com/sangtvo/US-Census-Bureau-Web-Scraper#tech-stack"/>
<a name="https://github.com/sangtvo/US-Census-Bureau-Web-Scraper#code-examples"/>

General Information
---
The project is part of a graduate course (_Advance Data Visualization_) at Western Governor's University. The data will not be provided, but rather an explanation of insights. 

Summary
---
A web scraper is created by using Python and scraped 227 links from the [Population and Housing Unit Estimates web page](https://www.census.gov/programs-surveys/popest.html). In order to get only unique links, a for loop is created which resulted in 119 unique links.

Tech Stack
---
* Microsoft Excel
* Tableau

Weighted Scoring Model
---

Make | Criteria | Rating & Weighting Range | Weighted Value Range | Rating | Weight | Weighted Value | Weighted Rating
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
2019 Ford Escape | Safety Features | 1-10 | 1-100 | 8 | 10 | 80 | 8.14
2019 Ford Escape |	Maintenance Cost|	1-10|	1-100|	7	|5|	35|	8.14
2019 Ford Escape|	Price Point|	1-10|	1-100|	10	|7	|70|	8.14
2019 Ford Escape|	Insurance|	1-10|	1-100|	8	|10	|80|	8.14
2019 Ford Escape|	Fuel Economy|	1-10|	1-100	|7	|10	|70	|8.14
2019 Ford Escape|	Resale Value|	1-10|	1-100|	9|	8|	72	|8.14
2019 Honda CR-V|	Safety Features|	1-10|	1-100|	8|	10	|80|	8.8
2019 Honda CR-V	|Maintenance Cost|	1-10|	1-100	|9	|5	|45	|8.8
2019 Honda CR-V	|Price Point|	1-10|	1-100|	9|	7|	63	|8.8
2019 Honda CR-V	|Insurance|	1-10|	1-100	|9	|10	|90	|8.8
2019 Honda CR-V	|Fuel Economy|	1-10|	1-100	|9	|10	|90|	8.8
2019 Honda CR-V	|Resale Value|	1-10|	1-100	|9|	8	|72|	8.8
2019 Hyundai Santa Fe|	Safety Features|	1-10|	1-100|	8	|10	|80	|8.06
2019 Hyundai Santa Fe	|Maintenance Cost|	1-10|	1-100|	9|	5	|45	|8.06
2019 Hyundai Santa Fe|	Price Point|	1-10|	1-100	|8	|7	|56	|8.06
2019 Hyundai Santa Fe|	Insurance|	1-10|	1-100	|7	|10	|70	|8.06
2019 Hyundai Santa Fe|	Fuel Economy|	1-10|	1-100	|8|	10	|80	|8.06
2019 Hyundai Santa Fe|	Resale Value	|1-10|	1-100|	9	|8|	72	|8.06
2019 Toyota RAV4|	Safety Features|	1-10	|1-100	|8	|10	|80	|8.26
2019 Toyota RAV4|	Maintenance Cost	|1-10	|1-100|	7	|5	|35	|8.26
2019 Toyota RAV4|	Price Point	|1-10	|1-100|	8|	7|	56	|8.26
2019 Toyota RAV4|	Insurance	|1-10	|1-100|	7	|10	|70	|8.26
2019 Toyota RAV4|	Fuel Economy	|1-10|	1-100|	10	|10	|100|	8.26
2019 Toyota RAV4|	Resale Value	|1-10	|1-100	|9	|8	|72	|8.26

The ratings are collected from [JD Power](https://www.jdpower.com/) and the weight is based on the company's requirements and I. The company's criteria are safety features, maintenance cost, and price point while my criteria are insurance, fuel economy, and resale value. In the above table above, it is a weighted scoring table with the combined six criterias. The weighted value is Rating x Weighting. The Weighted Rating is the sum of the weighted value over sum of weight per vehicle. 

Dashboard
---
![Dashboard](https://github.com/sangtvo/Company-Fleet-Selection-Using-Weighted-Scoring/blob/main/images/Dashboard.PNG?raw=true)

Data Analysis & Visualization
---
![VBar](https://github.com/sangtvo/Company-Fleet-Selection-Using-Weighted-Scoring/blob/main/images/Combined_Bar.png?raw=true)

For the company’s criteria which are safety features, maintenance cost, and price point, one can notice that maintenance cost and price point for the 2019 Honda CR-V are higher than at least 2 other vehicles. While the price point is ranked second compared to the 2019 Ford Escape, we can dig deeper into pricing and will notice that we can get a better deal at our local dealership. After collecting MSRP data (not shown) for new vehicles and finding local dealerships in the South Bay, the better value and discount for our money is the 2019 Honda CR-V which is $2,706.00 (MSRP $25,570 – fair purchase price $22,864) compared to $1,850 (MSRP $25,200 - $23,350) for the 2019 Ford Escape. Additionally, the 2019 Honda CR-V has the highest weighted value of 8.55 (not shown) for the first three features and therefore wins in this group.

As for my criteria which are insurance, fuel economy, and resale value, the 2019 Honda CR-V also ranks first in this criteria group. The 2019 Honda CR-V has 2 consistent features that have a value of 90 and are higher than at least 2 other vehicles. Since insurance has the highest score of 90, I collected insurance cost (not shown) for 5 years for all four vehicles and prorated the cost yearly. The yearly insurance cost for the 2019 Honda CR-V is $923 which is lower than all the other vehicles and we can safely assume why the 2019 Honda CR-V has the highest weighted value for insurance cost. I have also looked into the loss of value in terms of resale value because its weighted value is 72 across the board. The loss of value for the 2019 Honda CR-V for 5 years is prorated to $2,890 ($14,454 / 5 years) per year, which is the lowest out of all the other vehicles. This shows that even though all cars have the same weighted value, the company will get a better value for holding it for at least 5 years because we are not losing as much value compared to others and if anything, have better resale value. Overall, the 2019 Honda CR-V is ranked first in this group with a weighted value 9 on a scale from 1 to 10.

Solution
---
When combining all six features on a dashboard, we will see that 2019 Honda CR-V is the best choice for the company's fleet with a total weighted value of 8.8 on a scale from 1 to 10. This outcome makes sense because the 2019 Honda CR-V ranked higher in the company’s criteria and my criteria as well. Personally, I can agree with the results as I also was an owner of a 2002 Honda CR-V with over 200,000+ mileage and still running after 18 years. Since the company is interested in purchasing a 2019 Honda CR-V, it will have better technology and older car issues may already have been addressed, and therefore, it will last long and have better value for the company.  

Key Takeaways
---
* 2019 Honda CR-V has the highest weighted value than all the other vehicles with the company's criteria (8.55) and my criteria (9) with an overall combined weighted rating of 8.80.
* Insurance, fuel economy, and safety features are the most important requirements when choosing a vehicle (weight of 10). 
* 2019 Hyundai Santa Fe scored the lowest and least likely to be picked. 
* The lowest rated criteria is maintenance cost due to the company's weighted requirement of 5, meaning that the company is indifferent with maintenance costs and willing to pay more or less for necessary car repairs. 
* The best car for fuel efficiency is the 2019 Toyota RAV4 which received a perfect score of 100. 

