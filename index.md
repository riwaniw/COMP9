---
# Do not edit the text between these lines!
layout: default
---

# Analysis for Continous Improvement:

<!-- This is a comment. Below, you'll see code for inserting an image. To make this image appear, update <custom-path>. To add an image, save it inside the imgs folder of this repository. -->
<img src="https://riwaniw.github.io/COMP9/static/imgs/logo.png" alt="Image of Comp110 rainbow logo. "  width="500"/>

## Summary of Analysis:

First, I used the .csv Reader so that python can use all of the data from the survey. Then we used the columnar function so all of our data is in a dict based on columns. Next we used select to trim the data to only what we thought we needed to use. We use the columns prior_exp, pre_lecture_videos, understanding, and difficulty to later be able to compare if people with less prior experience or who are finding the course more challenging would prefer pre-lecture videos. 

Then we created a heatmap of values of preferring pre-lecture videos based on difficulty and understanding. What this does is looks at the number of students who assigned each score to both columns, darker squares mean more students selected that combination of rankings.

<img src="{{ '/static/imgs/heatmap1.png' | relative_url }}" 
     alt="Difficulty Heatmap" width="500" />

<img src="{{ '/static/imgs/heatmap2.png' | relative_url }}" 
     alt="Understanding Heatmap" width="500" />

Next, we created a bar-graph/histogram based on prior experience and rankings of preference for pre-lecture videos. To make this data even clearer we created a box plot to see where most of the data lies for each group based on experience level.

<img src="<COMP9>/static/imgs/bargraph1" alt="Prior Experience Bar Graph"  width="500"/>
<img src="<COMP9>/static/imgs/boxplot" alt="Prior Experience BoxPlot"  width="500"/>

Finally, after doing these comparisons of different groups I realized I wanted a look at overall whether students wanted pre-lecture videos so I created a bar graph of just these counts.

<img src="<COMP9>/static/imgs/bargraph2" alt="Pre Lecture Videos Bargraph"  width="500"/>

## Conclusions: 

One of the first things that my analysis displays is that a majority of respondants had a fairly high preference level for pre-lecture videos being available. The first hint I got that this might be true was from my run of the counts function on my selected data, where 388/534 students selected a preference greater than or equal to 5. This is visually displayed by my bar graph of just the variable pre-lecture videos which shows a skew towards the higher end of rankings for pre-lecture video preference.

Besides this overall preference for pre-lecture videos I wanted to see what subcategories of students were major stakeholders by plotting difficulty, understanding, and prior experience measures against pre-lecture video rankings. 

The box plot is one of the strongest visual representations for the prior_exp - pre-lecture videos comparison, and it reveals that students with None-Less than one month of prior experience were more likely to have a preference for pre-lecture videos, while students with more experience had less of a preference and more variability in their rankings. 

The two heatmaps that I first graphed were representations of understanding and difficulty plotted with pre-lecture video rankings, displaying concentrations or frequencies of results. 

There were large clusters around a difficulty ranking of 4-5 and a pre-lecture video ranking of 6-7 which does display that students with a mid-to-high ranking of difficulty had a mid-to-high preference of pre-lecture videos being available, but the graph also just displays that skew towards preferring the video no matter what as we have already seen.

The understanding graph is less conclusive, with mostly the takeaway that even students with a mid-to-high understanding level in the course had a mid-to-high preference for pre-lecture videos. 

Overall, even though the data doesn't necessarily show a strong relationship between difficulty and understanding rankings and video preference, it does show that most students would prefer pre-lecture videos be available, especially those with less prior experience. 

The actionable reccomendation from this would naturally be to create optional, short, pre-lecture videos that students could watch to get a preview of the information before coming to class. Some of the costs to initiating this change would largely be on the instruction team, ie. the professors/TAs that would need to take the time to create these videos. This could potentially draw these stakeholders time from other important parts of the course. 

Further exploration of this idea could come from future-leading questions that ask specifically if students think the videos would help their learning, as well as specifications about video length and content coverage. Another step could also be a look into how much time it would take to initiate this addition to the course and who would be willing to do it. 