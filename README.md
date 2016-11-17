# Data Analyst Nanodegree Project 6

Chosen Data Set: baseball_data.csv 

## Summary

The visualisation below presents an analysis of how the performance of baseball players can vary according to certain inherent physical characteristics.
As shown in the final chart, batting averages appear to decrease with height, while home runs appear relatively steady in the middle range of heights from 71-76 inches.
Players at 77 inches and above seem to have lower batting and home run averages. Home runs for players below 70 inches show some variation, but without a clear pattern.
Right-handed players also seem to have consistently lower batting and home run averages than their left-handed counterparts across comparable ranges of height.

## Design

My initial mockups investigated how the two performance indicators varied according to height and weight respectively, in separate bubble charts, created in excel for easy sketching. During exploratory data analysis, I also experimented using multiple lines to denote batting average and home runs for each chart. However, I felt this confusing and thus did not seek feedback on them, instead, only seeking feedback on the bubble charts.

###### Initial Design: 
![Initial Visualisation](/Initial Visualisation.png)

After receiving some feedback (see Feedback section below), I decided to do away with the weight chart, as it did not provide additional insight over the height chart.
Additionally, I decided to plot handedness using different colours, in order to see if any other interesting insights could be found from that. The blue, yellow and green color scheme was chosen as green, a mixture of the other two colors, adequately represents both.
Lastly, feedback on the lack of clarity regarding labels and titles was taken into consideration in creating the final design.

###### Post Feedback Design: 
![First Submitted Visualisation](/First Submitted Visualisation.png)

After submitting the design above, I received feedback that the scaling for my bubbles was inaccurately performed on radius, and the necessary correction was made, thus resulting in the revised visualisation seen below.

###### Post Submission Design:

![Revised Visualisation](/Revised Visualisation.png)

## Feedback

This section details three instances of feedback that I received on the visualisation sketch made in excel, and how those instances of feedback translated into the visualisation that I made for the first submission. Also, I included the feedback from the previous udacity reviewer and the changes made after receiving feedback on the first submission.

#### Monty

###### Feedback Given:

"Labels can be clearer. I lack background in baseball and can't really tell if the y-axis is batting average or something else."

###### Follow Up Action:

From this feedback, I made it a point to include clear labels of axes, and included a chart title to describe the chart.

#### Claire 

###### Feedback Given:

"There seems to be a downward trend in batting average as both height and weight increase. May want to investigate height more... seems like there's more complexity there."

###### Follow Up Action:

This insight led me to abandon the weight chart from the sketch to the first submission, as both height and weight are able to display the same downward trend.

#### Kevin 

###### Feedback Given:

"At first, the x-axis seemed like it displayed home runs. Also, it seems surprising that batting average decreases with size. Are there any other factors that might affect performance?"

###### Follow Up Action:

The first point made here overlaps with previous feedback on the need for axis labels. The last suggestion led me to investigate handedness as another variable to include in the visualisation, which I did, using color, as detailed in the design section above.

#### Udacity Reviewer

###### Feedback Given:

"After a further investigation, however, it looks like bubble sizes have not been properly scaled... (referencing a specific datapoint) The above bubble encodes 246 home runs, while the bottom one encodes 67. Ideally, the above bubble should be able to contain four of the bottom bubbles, but that does not seem to be the case."

###### Follow Up Action:

setTimeout was used in order to scale the visualisation properly, representing home run data as area instead of radius as it previously had been. This change is reflected in the latest "Revised Visualisation" file.

## Resources

###### http://techslides.com/over-1000-d3-js-examples-and-demos
###### http://stackoverflow.com/questions/25416063/title-for-charts-and-axes-in-dimple-js-charts
###### http://dimplejs.org/advanced_examples_viewer.html?id=advanced_custom_styling
