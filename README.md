# Project 03: Company Fleet Selection Using Weighted Scoring
> This project explores an analysis using the weighted scoring method on selecting one of the four vehicles as part of the company fleet: 2019 Ford Escape, 2019 Honda CR-V, 2019 Hyundai Santa Fe, and 2019 Toyota RAV4. The requirements for the vehicles are based on safety features, maintenance cost, price point, insurance, fuel economy, and resale value. In order to present this analysis to management on car selection, a data visualization tool, Tableau, is used to present my decision.

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

Data Preprocessing
---

Make | Criteria | Rating & Weighting Range | Weighted Value Range | Rating | Weight | Weighted Value | Weighted Rating
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
2019 Ford Escape | Safety Features | 1-10 | 1-100 | 8 | 10 | 80 | 8.14
