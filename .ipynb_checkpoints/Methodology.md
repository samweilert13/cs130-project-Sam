# Methodology

## Data Sources
- I downloaded my data for my data analysis from Kaggle.com. I downloaded Rishab Jadhav's "NFL Passing Statistics (2001-2023)" passing_cleaned.csv to begin analyzing data over the last 20 years of football history. I also used profootballreference.com on my
article to find career passing statistics.
## Data Preperation/cleaning
- To first prep my data, I called it through the passing_cleaned.csv file and stripped and split the data to make it readable for my code. This was key as many of the following steps would've been near impossible without a clearly legible code to draw from. 
- You can also see in my testing that I messed around with the data several times to see what I could draw from it. I unfortunately deleted the code earlier on in my process but an original plan I had was creating an average yards per game played statistic but I found that the method I decided to end with was much better.
- Another way I prepared my data for analyzation was by importing pandas, numpy, and matplotlib.pyplot to better draw data from my code
- To make the data I was drawing from only related to starters, I eliminated a good chunk of the names from the entire passing_cleaned.csv by required that to be analyzed, a player must have at least 1000 passing yards and 14 starts. I did this every year by entering the code: passing_stats2001 = passing_stats.loc[(passing_stats.Yds > 1000) & (passing_stats.GS >= 14) & (passing_stats.Year == 2001)]
## Assumptions
- One way that helped me make sure the data I was using was consistent to real world NFL data was by comparing Jadhav's findings to profootballreference.com's. 
- Throughout my process I assumed that his data was always right
## Limitations
- Luckily I found the limitations to the data right near the very end when I was encountering problems with the Buffalo Bills data. For some reason, the data was returning Josh Allen as the starter in the year 2007, a time when Josh was only 11 years old. I did some digging and somehow the data for 2007 was a mirror copy of 2023 data. I have no idea how that happened but I deleted any data in my file that came with the year 2007 because of that
- Besides the very strange 2007 debacle however, my data was in very pristine condition to be analyzed 
