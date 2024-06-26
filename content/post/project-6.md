---
date: 2022-08-08
description: "Property investing lead generator and investment analysis tool."
featured_image: "/images/dwmap2.png"
tags: ["Python", "R", "Shiny", "ETL"]
title: "Project 6: AU Property App"
---
- Sourcing deals for rental property investing can be a challenging 
process. Not only does extensive searching need to be done but deal 
analysis must be thorough in order to determine whether a 
property can be cash flow positive. This app serves as a tool which queries a 
real estate listing site and loads data into a data warehouse. 
Thereafter, the data is served along with user-defined master data in 
order to present useful functionalities for investors such as summary 
market statistics, a geocoded plot of property locations, lead 
generator, and investment deal calculator. I used a realestate.com.au
Python [wrapper](https://github.com/tomquirk/realestate-com-au-api) 
designed by GitHub user Tom Quirk to assist with the source ETL 
process.
- High-level design and data flow:
{{< figure src="/images/project-6-0.png" title="" >}} 

- **Dashboard**:  
View Australian property market stats as according to 
listings on realestate.com.au and drill-down by state.
{{< figure src="/images/project-6-1.png" title="" >}} 

- **Map**:  
View current listings in data warehouse fact table. 
Hover over a listing to view the precise address.
{{< figure src="/images/project-6-2.png" title="" >}} 

- **Leads**:  
Based on user-defined master data, e.g. downpayment 
percent, loan interest rate, and desired ROI, current 
fact data is displayed with a calculated column of 
whether the property would make sense as deal based on 
your numbers ('Buy' or 'Pass').
{{< figure src="/images/project-6-3.png" title="" >}} 

- **Calculator**:  
Quickly try out different scenarios based on your 
investment strategy. Take screenshots of your results.
{{< figure src="/images/project-6-4.png" title="" >}} 

- Down the line, I plan to expand this project to 
add more functionality and package it for public use.

Versions used:

- Python 3.10.4
- R 4.2.0

View the project on **Github**:  
[David-dmh/dw-rei](https://github.com/David-dmh/dw-rei)
