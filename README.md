# Summary
The National Science Foundation Data on Women, Minorities, and People with Disabilites STEM Data is released annually.  This data visualization initial focus is to illustrate the graduation rate of those ethnicities that are under-represented in the Techonology sector.  We can see an increase the graduation rate amongst African-Americans/Hispanics in Mathematics/Statistics, Electrical Engineering, and Computer Science.  Below the graphic are degree fields that the user can explore at their own leisure.   

# Design
My Data Wrangling process can be found in the Ipython notebook (**Data Wrangling STEM data.ipynb**).  My Exploratory Data Analysis can be found in the R markdown file (**nsf_degrees.Rmd**).  You can view the data visualization at [here](http://bl.ocks.org/rmhyman/1b09cba5086f5f540bbb8465e6f0166e)
# Feedback
*Feedback 1*:
Ransford, I really like what you've done in terms of the data! I noticed the changes in degrees achieved by minorities, and it's good to know that blacks have achieved around 50% increase in Associates Degrees between 2002 and 2012, while whites have also gained a good percentage increase around 31%.

I would say that the main takeaway is that there is a really great improvement in degree achievements among minority groups, and continued improvement among the majority group. However, almost every field of study suffers from a relative lack of minority representation.

The visualization simply states the facts but not the reason which would probably require a different visualization.

Great job, thanks for the valuable information!!

*Feedback 2*:
Great work! Particularly the animation which really catches eye. Here're some ideas for you to consider:

Pie charts are not normally the top choice for visualizing numerical variables since it's hard for our eyes to distinguish between different areas. Although I have to say in this case, animation has made the comparison easier. Also, ring chart does seem to be different than pie chart. Alternatively, you can consider using an area chart like this3 with the x-axis being time, y-axis being percentage.
Displaying all the different job fields in the meantime can be a bit overwhelming for the reader, also makes it hard to switch between fields. Using one field as default and give an option to choose on the side can probably help.

*Feedback 3*:
On a technical note, on the default chart that appears before you click on any of the boxes, the Asian/Pacific Islander, White,  and Other groups are all showing up as grey in the chart, but have different colors in the legend. 

As far as my perception of the visualization, it was not obvious to me at first that I needed to click on the boxes of the majors to show the data for that major... I just thought it was another visualization that I didn't understand. So, a little bit of clarification could help (or better yet, change the design in some way that makes the viewer drawn to do what they need to do to see the different views without explicitly telling them what to do).

Also, I didn't read any of the links in the description, but one thing I was wondering about the data is if the numbers had been normalized to the proportions of the different ethnicities in the general population. For example, if only 5% of the general population is Asian/Pacific Islander, then having 5% of STEM graduates being Asian isn't an under-representation. However, if 50% of the population is Asian and only 5% of graduates are Asian, then there's definitely a discrepancy.

Anyway, good job overall! I think it's a very interesting visualization.


# Resources

[d3-tip](https://github.com/Caged/d3-tip)

[Stacked Area Chart example](https://bl.ocks.org/mbostock/3885211)

[Video explaining how to implement stack area charts](https://www.youtube.com/watch?v=5H7PSAqZ0Co)
