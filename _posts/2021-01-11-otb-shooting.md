---
layout: post
title: A statiscial data analysis to find the best shooters from Outside the box
subtitle: 
image: /img/soccer-ball-variant.png
tags: [Visualizations, Data Analytics, Analytics, Football Analysis]
---

While watching a game of football, we all love to see a shot from outside the box with the commentator screaming at the top of his lungs, especially if the shot is going to be from one of the best shooters. At the same time, seeing your player take a shot from outside the box can be frustrating if your team is chasing the game in the last few minutes. This analysis tries to find out which players are best in shooting from outside the box and which players are not.

*Maybe somebody out there has already done this type of research and already has the answer to the question. If so, I would love to talk to that person to see how my thought process matches with theirs and would love to get suggestions on how I can build further on this analysis. I would like to thank understat.com for providing the data for this analysis. Players actively playing in Europe's top 5 leagues are only considered for this analysis.*

Before we delve deeper into this analysis, the following visualisation (Figure 1) shows all shots taken from outside the box through open play, since 2014, by players who are actively playing in Europe’s top 5 leagues.


<figure>
  <img
  src="/img/otb_shooting/otb_plot.png"
  alt="shots-from_outside-the-box-all-years">
  <figcaption>
  	<b>
  		<i>Figure 1 - Open Play shots from outside the box since 2014</i>
  	</b>
  </figcaption>
</figure>


That’s 54335 shots from outside the box from open play - roughly 40% of the overall open play shots have come from outside the box in Europe’s top 5 leagues since the 2014/15 season.

In terms of % of shots from different areas on the pitch outside the box, the following visualization (Figure 2) shows the % of shots from each zone. Please note that these zones were decided by me for the purpose of this analysis. Unsurprisingly, the area just immediately outside the box has seen the most shots. The zones behind this, centrally, come second.

![percent_otb_shots](/img/otb_shooting/zone_plot.png)
***Figure 2 - Shooting zones outside the box since 2014***

**Shooting Volume**

Some players are comfortable shooting from outside of the box and some players are just not. Also, whether a player decides to shoot from outside the box depends on the game state but mostly players take a call based on their instincts and ability. The volume of shots a player takes from outside the box answers the question of how comfortable that player feels  shooting from outside the box. The following table (Figure 3) shows the ‘Top 10 players’ for Average number of shots per 90 minutes from Outside the box since 2014/15.

Lorenzo Insigne ranks number one in ‘Europe’s big 5 leagues’ for average number of shots per 90 minutes in open play since 2014/15. Other familiar names in the top 10 include Philippe Coutinho(1.72), Cristiano Ronaldo(1.46), Hakan Calhangolu(1.45). No player from the Premier League is in the top 10. The only premier league players in the top 25 are Kevin De Bruyne(1.34), Paul Pogba(1.33), Harry Kane(1.15), Ross Barkley(1.14), Jonjo Shelvey(1.13). Lionel Messi ranks number one if you consider shots from every situation.

![table_freq](/img/otb_shooting/tableFreq.png)
***Figure 3 - Shooting Volume (Top 10) from Outside the box since 2014***

There are also players who are not comfortable taking the shots from outside the box or players who don’t have a lot of opportunities to take shots from outside the box. These players are mostly forwards/strikers as they are often located inside the box because of their role. The following table (Figure 4) shows the players who rank bottom 25 for ‘Average number of shots per 90 minutes from outside the box’.

Jamie Vardy, Diego Costa, Mauro Icardi, Timo Werner who are all well known to be at the right place at the right time inside the box rank below average for volume of shots from outside the box and rightfully so. Most of these players regularly play in the front three in their teams.
Couple of surprising names in the list include Georginio Wijnaldum and David Silva who in spite of playing a little bit deep rank bottom for Average no. of shots per 90 minutes from outside the box.

![table_non_freq](/img/otb_shooting/tableNonFreq.png)
***Figure 4 - Shooting Volume (Bottom 25) from Outside the box***

**Percentage of shots from outside the box***

Another way to measure a player’s volume of shots from outside the box is what percentage of a player’s shots come from outside the box. The following table (Figure 5) shows the top 10 sorted by ‘Percentage of shots from outside the box’.

![otb_percent](/img/otb_shooting/otb_percent.png)
***Figure 5 - % of player’s total shots (Top 10) from outside the box***

A common thing among some of the players listed in Figure 5 is that those players play in a deeper role and are mostly stationed outside the box almost all the time.  Andros Townsend, known for his excellent curlers from outside the box has attempted roughly 64% of the shots from outside the box since 2014/15.

When we consider the opposite of this (i.e.) players who attempt a fewer percentage of their shots from outside the box (Figure 6), we get almost the same list of players as in Figure 4 because these are players who are almost always stationed inside the box.

![otb_percent_less](/img/otb_shooting/otb_percent_less.png)
***Figure 6 - % of player’s total shots (Bottom 10) from outside the box***

In Figure 3, we saw who were the players with the most shots per 90 from outside the box in Europe’s top 5 leagues since 2014/15. What % of their shots do these players attempt from outside the box? The following table ( Figure 7) has the answer to that question.

![otb_percent_custom](/img/otb_shooting/otb_percent_custom.png)
***Figure 7 - % of total shots ( for frequent shooters) from outside the box***

Radja Nainggolan, Philippe Coutinho, Hakan Calhanoglu, Josip Ilicic are all very comfortable taking shots from outside the box. They attempt more than 50% of their shots from outside the box.

**Shooting Frequency Rate (SFR)**

We looked at Volume - which was an indicator of how comfortable a player feels shooting from outside the box. Volume also indicated the frequency in a way - if a player has more shots per 90 minutes - one could refer to him as a ‘Frequent Shooter from outside the box’. A more direct indicator of the frequency metric is the Shooting Frequency Rate ( SFR ). SFR indicates how often the player is willing to take a shot from outside the box based on the minutes he has been on the pitch.

![sfr](/img/otb_shooting/sfr_best.png)
***Figure 8 - Shooting Frequency rate (Top 10)***

Figure 3 indicated that Philippe Coutinho ranks 2nd for avg. no. of shots per 90 minutes from outside the box. That is largely because Coutinho attempts a shot from outside the box every 49 minutes and is the best in Europe’s top 5 leagues for that metric. Paul Pogba, Kevin De Bruyne, Jonjo Shelvey - among players actively playing the premier league - rank in the top 20 for SFR.

**Quality of Shots**

Volume and SFR don’t reflect how good the players are shooting from outside the box. A metric that answers that question is the Expected Goal value. First, we will try to find out what is the average xG of shots from outside the box for players listed in Figure 3 as they are the ones who often shoot from outside the box.

![quality_custom](/img/otb_shooting/quality_custom.png)
***Figure 9 - Quality of shots from outside the box***

Thauvin and Ilicic have the best xG. An Expected Goal value of 0.04 is considered pretty average from a general perspective but to think Thauvin and Ilicic shoot from outside the box with an average xG value of 0.04 is quite impressive. Lorenzo Insigne has attempted the most open play shots from outside the box. His average xG value stands at 0.03.

Players like Coutinho, Ronaldo and Ilicic pass the eye test as good shooters from outside the box. The analysis backs that fact. Some surprising names (at least for me) for the best shooters from outside the box include Florian Thauvin, Hakan Calhanoglu. 

To finish off this analysis, here is a visualisation (Figure 10) showing the shot zones from outside the box for Coutinho, Insigne, Ronaldo, and Ilcic.

![custom_zone_plot](/img/otb_shooting/custom_zone_plot.png)
***Figure 10 - Shooting Zones from outside the box***

***Note:*** *All the data used in this analysis was obtained from understat.com. Shots only beyond half line were considered. Please reach out to me via twitter [(@VenkyReddevil)](https://twitter.com/VenkyReddevil) in case you have any suggestions or if you find any mistakes in this and my apologies if you do find any mistakes.*

***How am planning to improve this research in the future?***
T*his article now is more generic and a lot of importance has not been given to the end product and conversion from each zone outside the box. To find the exact ‘Shooting Strength Zone’ of each player is the next step in this research.*

Follow me on twitter if you like my work - [@VenkyReddevil](https://twitter.com/VenkyReddevil). Email me at venkatanarayanan22@gmail.com if you have any queries or suggestions about my work





