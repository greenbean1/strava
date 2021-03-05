# Strava
This project grabs [Beau's strava data](https://www.strava.com/athletes/22694485) puts it into a CSV and then
interactively visualizes it in a Dash App

## Motivation
So much

## How Does This Work?
1. First we hit the Strava API, grabbing activity data
2. Then we put that activity data into a Google Sheet
3. Next we use Pandas to format several dataframes convenient for our viz
4. Lastly we had Dash point to those dataframes for a sweet viz

## Division of Labor
### Brian
-Read Strava data from Gsheets and put into Dash
-Initially use faked data in the same format that the Strava API will give
### Beau
-Get Strava authentication & write into GSheets