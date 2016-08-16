# Project 6
Steven Yeh


##Summary
In this chart, I visualized the mean batting average and total home runs for each height measurement and batting handedness. The y-position of each circle represents the batting average for a given x-position height, the color represents the handedness, and the relative size of the circle represents the total number of home runs. Notice that for right and both handed batters, there is a specific height and batting average where the total HR count is much higher than its other similarly colored circles. Also notice how in general, left handed batters hit a better average and more home runs for a given height than right/both handed batters.

##Design
### Initial Design
I initially tried to represent the relationship between batting averages, handedness, and height with a bar chart. The mean batting average for each height and handedness preference on the x-axis(first height by x-axis location then handedness by bar color). A legend for handedness was placed in the top right. Hovering over a bar would provide the mean average for that specific height and handedness. In addition, I edited the data to remove batting averages of 0, reducing the datapoints from 1157 to 891 (-266). I also expanded the values in handedness: from B to Both Handed, L to Left Handed, and R to Right Handed.

### Second Design
After collecting feedback, I decided to add a fourth variable, HR to show where left, right, and both handed players performed the best in batting average and total home runs. To visualize this, I decided to switch from a bar graph to a bubble graph for its extra visual dimension (size). In addition, I added gridlines to foster a better visual separation by height. I changed the title to reflect the new variable, and the title font was changed from default Times New Roman to Georgia and was moved from the top left to top center. The y-axis was renamed from 'avg' to 'Batting Average' for cohesiveness.

### Final Design
To further improve the graphic, I reduced the margin to 25, increased the width from '1400 - margin' to '1800 - margin', and increased the height from '600 - margin' to '900 - margin'. This also stacked the bubbles vertically for each height, allowing a better comparison of different handed batters for a given height. I removed handedness from the x-axis since it was already indicated by the bubble color. The radii of the bubbles were scaled by square root of home runs hit to represent the size of home runs hit. I added thin trendlines for each handedness to better show how left handed batters have slightly higher batting averages than right and both handed batters. The bubble sizes were proportionally reduced to reduce visual cluttering. Text was added above the graphic to describe the data set, give readers a clue as to why some circles were huge, and give a disclaimer about average of averages. Abbreviations of variables were removed in favor of the full name (ex: Home Runs instead of HR). A custom tooltip was implemented with fully named variables.

##Feedback
Here are several feedback comments after showing the first version of the graphic to three individuals:


###What do you notice in the visualization?

* Some heights are missing bars, mostly on the outer ranges of height (65-66 in, 77-80 in).

* The majority of mean batting averages are within 0.01 or 0.02 to 0.250.

* Very tall right handed batters have rather low batting averages.


###What questions do you have about the data?

* It seems like only left handed batters have a lower average with increasing height, why? 

* Why is there no discernable relationship for right/both handed batters?

* How many batters are there for each height and handedness?

* Why do left handers have higher averages for a given height?
  

###What relationships do you notice?

* For left handers, batting averages generally decrease with height.

* For heights with all three batting handedness represented, left handers have a higher mean batting average.


###What do you think is the main takeaway from this visualization?

* Left handers have somewhat lower batting averages with increasing height, and right/both handed batters have no relationship with height. 

* Left handers have a higher batting average than their right/both handed batters of the same height. 


###Is there something you don’t understand in the graphic? How can it be improved?

* Seems like the lack of data for players 65-66 inches and 77-80 inches makes the graphic misleading. How many players were 79 inches versus 72 inches?

* Make the title stand out more

* Since there's other variables such as weight and HR count, maybe try to incorporate another variable to get a better picture.

##Resources

https://github.com/PMSI-AlignAlytics/dimple

http://dimplejs.org/

http://stackoverflow.com/tags/dimple.js/

Udacity Forums: DAND P6:
https://discussions.udacity.com/c/nd002-p6-data-visualization-with-d3-js/p6-make-effective-data-visualization