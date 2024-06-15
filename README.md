# A-Forecasting-DSS-for-Burger-Bounty-using-R
![burgervan](https://github.com/Kritika97Gaikwad/R-Shiny-Projects/assets/151272622/dd35bc56-fd74-4198-bc91-c5673003ec47)

## Data Structure

- **Visits Sheet:** Contains data related to customer visits.
- **Prices Sheet:** Stores the selling prices for each burger type.
- **Sales Sheet:** Captures the quantity sold for each burger type.


# Burger Bounty Shiny Dashboard

This Shiny app serves as a dashboard for summarizing and updating monthly sales data for a fictional burger business. The app allows users to input data related to customer visits, sales quantities, and pricing. The data is then visualized in an Excel file using the "shinydashboard" package in R.

## Features

- **Customer Order Entry Form:** Collects user information, date of data collection, town visited, time spent, weather conditions, and event/weekend status.

- **Sales Data Entry:** Allows the user to input the quantity sold for each type of burger.

- **Pricing Data Entry:** Lets the user set the selling price for each burger type.

- **Update Button:** Triggers the update of the Excel file with the entered data.

## Getting Started

### Prerequisites

- R installed on your machine
- Shiny package installed (`install.packages("shiny")`)
- Shinydashboard package installed (`install.packages("shinydashboard")`)
- Readxl package installed (`install.packages("readxl")`)
- install.packages("openxlsx")


### Running the App

1. Open RStudio or your preferred R environment.
2. Open the `app.R` file.
3. Run the Shiny app.

## Usage

1. Fill in the customer order entry form with the required information.
2. Enter the quantity sold for each burger type.
3. Set the selling price for each burger type.
4. Click the "Update" button to update the Excel file with the entered data.

### Generate Regression Models:

Download 3.Forcasting/Forcasting_using_linear_regression.R and open Forcasting_using_linear_regression.R in R or RStudio.
Run the script to generate six linear multiple regression models for each type of burger.
The script reads data from data/BurgerBounty.xlsx and outputs the regression models.

### Regression Models
Six linear multiple regression models are created, one for each type of burger. Each model predicts sales (number of burgers) based on the following seven independent variables:
- Burger price
- Visited town
- Time spent at the location
- Average precipitation
- Average temperature
- Whether there was an event
- Whether it was a weekend

### 4. Shiny App Design
The Shiny app provides location recommendations based on user inputs and the regression models. The user interface includes:

Four inputs for variables common to all locations:
- Hours to be spent at the location
- Average precipitation
- Average temperature
- Whether the visit will be on a weekend day
- Seven inputs for each location to specify whether there will be an event at that location
- Six inputs for the planned price per burger for each burger type
- A button titled "Recommendations"


## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.


## Acknowledgments

- Thanks to the Shiny and Shinydashboard communities for providing powerful tools for interactive data visualization in R.
