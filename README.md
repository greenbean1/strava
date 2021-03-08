# Strava
This project visualizes [Beau's strava data][1] in a [Dash App][2] designed to answer some questions

## How Does This Work?
1. First we hit the [Strava API][3], grabbing activity data
2. Then we put that activity data into a [Google Sheet via API][4] (first - one time then periodically)
3. Next we use Pandas to format several dataframes convenient for our viz - Is this necessary?
4. Lastly we had Dash point to those dataframes for a sweet viz

## Motivation
- Technical Learning
    - Great opportunity to practice getting data from a modern API - Strava
    - Given we use Google Sheets so much personally & professionally, learning to use its API makes a lot of sense
    - Dash adds another powerful data visualization tool to the toolkit & is an introduction to making web apps
    
- This project incentivizes use of Strava which means more exercise which means better health! 

## Tactical Details

### General Approach
- Use branches and PRs with code reviews before merging with main

### Division of Labor & Milestones
#### Brian
Read Strava data from Gsheets and put into Dash
1. Learn Gsheets API authentication & Hello World reading data
2. Read Beau's faked Strava from GSheets
3. Learn Dash & Hello World (most basic viz)
4. Determine Gsheets -> Dash pipeline (ex: intermediate Pandas required?)
5. Read from Gsheets into Dash & Basic Dash app
6. Iterate on Dash visualizations
#### Beau
Pull Strava Data & put it into GSheets
1. Learn Strava API activity data format to put in fake data into GSheet
2. Learn about Strava API authentication & Hello World
3. Get JSON Strava API activity data
4. Learn GSheets API authentication & Hello World
5. Write Strava JSON data into Gsheets
#### Last Milestone: Schedule refreshes OR give Dash users the option refreshing of data from Strava to Gsheets to Dash

## Misc

### Things Learned
- So much

### Credits
Thank you [Nathan Hoover][5] for your guidance on this project.

[1]: https://www.strava.com/athletes/22694485
[2]: https://dash.plotly.com/
[3]: https://developers.strava.com/
[4]: https://developers.google.com/sheets/api
[5]: https://github.com/nhoover