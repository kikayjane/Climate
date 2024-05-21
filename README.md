# Climate
This project aims to analyze long-term trends (warming ocean temperatures, more frequent or intense storms, etc) of seven major ocean basins: the Arctic, North Atlantic, South Atlantic, Indian, North Pacific, South Pacific, and Southern Oceans by utilizing 80 years of data comprising of daily sea surface temperature, wave height, and wind speed.

## Requirements
Colab

## Data
This notebook utilizes data queried from the ERA5 Reanalysis Product produced by the European Center for Medium-Range Weather Forecasting (ECMWF), widely regarded as the best forecasting center in the world.

All the data for each ocean basins are located in the "data" folder in the repository.

## Analysis
To forecast future trends, the following steps were taken:
1. Load the data then review their contents
2. Rename columns and convert the 'date' column to datetime format
3. Plot the time series and generate summary statistics
4. Apply seasonal decomposition to isolate trend, seasonal, and residual components, and visualize them
5. Fit an autoregressive (AR) model to the residual component and forecast future temperatures
6. Forecast sea surface temperature for the next 10 years and plot the forecasted and historical data
7. Calculate and visualize the overall correlation matrix between temperature, wind speed, and wave height
8. Segment data into season and visualize correlation matrices for each season
9. Split data into training and test sets, forecast the test period, calculate the MSE and visualize results
10. Interpret results to produce conclusions.

The file "climate_analysis.ipnyb" contains the coding that performs the analysis and forecasting, also linked in the repository.

## Author
Rica Jane Bayani-Dahilig (me)

## License
MIT License

Copyright (c) 2024 Rica Bayani-Dahilig

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
