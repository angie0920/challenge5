# Portfolio Simulations- Challenge 5 Submission
The enclosed program queries two crypto currencies and two coventional financial assets using requests libraries and alpaca APIs. The values of these assets are combined with certain assumptions to generate a financial portfolio. This portfolio is then measured against criteria for an emergency fund. The second part of this challenge takes the conventional financial instrument portion of the total portfolio and simulates the cumulative returns over a thirty and then ten year time period.
--

## Technologies
This challenge uses alpaca apis and the request libraries to query current and historical data. The other technology differentiator is the simulation functionality - the user enters a few parameters that are then passed into a python simulator script pulled into the main coding .ipynb file.

--

## Installation Guide
Before running program: 
1) alpaca keys need to be saved to an env file.
2) Import these libraries, dependencies, and commands:
import os
import requests
import json
import pandas as pd
from dotenv import load_dotenv
import alpaca_trade_api as tradeapi
from MCForecastTools import MCSimulation

%matplotlib inline
--

## Usage

Cryptocurrencies are queried using the requests library and organized with json function. Stock and bond information is queried using the user's alpaca api key and alpaca api secret key.

Saved images show the thirty and ten year simulation results - one line plot and one histogram for each.

Summary statistics for 30 year simulation:

count           500.000000
mean             15.274573
std              12.776972
min               1.076885
25%               6.768043
50%              11.756483
75%              19.624943
max             104.403783
95% CI Lower      2.669718
95% CI Upper     49.210933

--

Summary statistics for 10 year simulation:

Count           500.000000
mean              2.940110
std               1.822864
min               0.590603
25%               1.644542
50%               2.556856
75%               3.693515
max              19.436482
95% CI Lower      0.828828
95% CI Upper      7.555668

--

## Contributors
Angela Richter is the sole contributor to this program

--

## Licenses

This program and related items in this repository is intended for learning purposes only.