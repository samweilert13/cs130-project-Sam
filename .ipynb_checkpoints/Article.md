# How have Passing Stats in the NFL changed over time?

## Introduction

Since the first ever NFL game between the Dayton Triangles and Columbus Panhandles was played over 100 years ago all the way back in 1920, the league has been in a never ending cycle of evolution. Rule changes and changing coaching philosophies led to a sport that was previously a smashmouth, run it up the middle 40+ times a game sport into a more nuanced game of passing and strategy.
>Former 1960s and 70s Rams and Chargers Head Coach Sid Gillman is often credited as the father of the modern passing game, leaving behind a legendary coaching tree that is second to none

### Hypothesis
This got me wondering how much the NFLs passing game has expanded over the past 2 decades. I believe that since ther turn of the millenium we've seen even more of a shift towards the passing game, with legends such as Tom Brady, Drew Brees, and Aaron Rodgers breaking nearly ever QB record that was set before them. However, since those GOATs have either retired or regressed, the NFL has seen more of a return to the run game. My prediction is that from 2000-2020 there will be a consistent growth in total passing statistics, but once we hit post 2020, the graph will begin to lower more towards the late 2000s early 2010s numbers. 
>Of the QBs who rank top 10 in passing yards all time throughout their careers, 7 of the 10 were drafted after the 2000 season and only 10th place Dan Marino retired before then

  <img width="321" height="277" alt="Screenshot 2025-12-12 at 6 08 56 PM" src="https://github.com/user-attachments/assets/c1221985-56fa-4850-ae98-367e0680c393" />

### Data Collection
To find this data, I searched on kaggle.com for an NFL dataset and came across one by Rishab Jadhav that has all NFL passing data from the 2001-2023 seasons. Any player that attempted a pass was included so it was perfect for my research. I decided I wanted to find 4 specific trend lines to see the increase in passing data over the 22 year period, with a focus on the Bills as they are a team that has seen a massive increase in passing offense with the arrival of (soon to be father) Josh Allen.
- **Starters passing yards**
- **Starters passing TDs**
- **Buffalo Bills passing yards**
- **Buffalo Bills passing TDs**

## Starters passing yards
<img width="629" height="447" alt="Screenshot 2025-12-12 at 7 43 31 PM" src="https://github.com/user-attachments/assets/5335a3b5-eba1-437a-8eef-236f62e9a1bd" />

### Statistical metrics
- **Slope line: 3453.85 + 30.58x (x = number of years with 2002 being 1)**
- **R^2 value: 0.589 (Moderate positive relationship)**

As you can see here, my hypothesis seems right. theres a strong increase over time of the average starters passing yards, and then at a certain point in the late 2010s/2020s it plateus. From starting at around 3400 in the early 2000s to over 4200 is a very impressive jump. I calculated the statistical metrics for both league wide starters statistics using linear regression models.

## Starters passing TDs
<img width="589" height="447" alt="Screenshot 2025-12-15 at 1 42 22 PM" src="https://github.com/user-attachments/assets/07ae44ba-fade-4d1b-9ae1-276246888487" />


### Statistical metrics
- **Slope line: 21.06 +  .296x**
- **R^2 value: 0.456 (Moderate positive relationship)**

The average TDs metrics are very similar to the ones we saw above with the yards statistic, with only a slightly lower corelation. It started at only around 20 TDs to near 30, there was a pretty significant jump in how many TDs the QBs contributed to.

## Bills passing yards
<img width="597" height="446" alt="Screenshot 2025-12-12 at 8 08 21 PM" src="https://github.com/user-attachments/assets/176c2b7a-53f4-4172-bd33-8104b527fbcb" />

### Statistical metrics
- **Slope curve: 3203.76 + 42.17x + 7.19x^2**
- **R^2 value: 0.455 (Moderate positive relationship)**

When you look at the data through the lens of a specific team, the data is much more volitile. For example, the Buffalo Bills in 2002 had prime Drew Bledsoe at the realm throwing for 4359 passing yards, good for 2nd most in the league. After Bledsoe however, the Bills went into a horrific drought trying to find their next franchise QB. It was another 18 years before Josh Allen broke onto the scene to become the next Bill to throw for over the 4000 yard mark. For the statistical metrics on both stats related to the Bills, I used a quadratic regression model to explain the curvature of the graph
>Most teams probably wouldn't require a quadratic model as on average the leagues metrics went up, but the Bills extreme drought in the middle at the position called for a nonlinear measurement

## Bills passing TDs
<img width="579" height="444" alt="Screenshot 2025-12-12 at 8 27 45 PM" src="https://github.com/user-attachments/assets/1e5c4a29-744b-4a62-84a3-01a3787ed8e2" />

### Statistical metrics
- **Slope curve: 18.763 + .627x + .0661x^2**
- **R^2 value: 0.428 (Moderate positive relationship)**

The TD stats show off even more how generational Josh Allen has been for this team. There isn't even much correlation as the years go on and the team struggles to find a QB, but when Josh finally develops into a superstar in 2020, the difference is night and day. This data doesn't even include all the rushing TDs he racks up as well, it just shows how dominant of a passer the Bills have been lucky enough to find

## Conclusion
There were two major findings in this study, one being that the NFL definitely saw a surge in passing statistics through the late 2000s and 2010s, and also that Josh Allen is a god among men. I believe that if I continued to track data over time for the league wide portion of the study, I would continue to see the leveling out of stats that were present in the final 3 years of the data. The NFL now has seen an abundance of QBs that are effective with their legs as well as their arms, which translates into more rushing yards and TDs instead of their passing counterparts. Defenses also adjusted to the shift in strategy to becoming much better at stopping the pass over the last couple years with new inovations coming out every day. However, as the drastic changes from 2001-2023 show you in this article, anything is possible in the NFL.

## Links
- https://www.pro-football-reference.com/leaders/pass_yds_career.htm
- https://www.kaggle.com/datasets/rishabjadhav/nfl-passing-statistics-2001-2023?resource=download
