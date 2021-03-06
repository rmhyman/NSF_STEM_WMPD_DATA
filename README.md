# Summary
The National Science Foundation Data on Women, Minorities, and People with Disabilites STEM Data is released annually.  This data visualization initial focus is to illustrate the graduation rate of those ethnicities that are under-represented in the Techonology sector.  We can see an increase the graduation rate amongst African-Americans/Hispanics in Mathematics/Statistics, Electrical Engineering, and Computer Science.  Below the graphic are degree fields that the user can explore at their own leisure.   

# Design
My Data Wrangling process can be found in the Ipython notebook (**Data Wrangling STEM data.ipynb**).  My Exploratory Data Analysis can be found in the R markdown file (**nsf_degrees.Rmd**).  I initially wanted to create a SunBurst visualization, but was having a difficult time trying to generate a good hiearchy. The SunBurst visualization would have allowed me to present all of the data in a consolidated space. I then decided to produce Mini Donuts instead. This could give me some experience of working with arcs.  I wanted to generate a martini-glass style of visualization so my initial author-driven was to show the data for the Bachelor's Degree for the three fields that are heavily sought after in the Tech Industry (Math/Stats, Electrical Eng. and Computer Science).  After the animation, I invite the user to view the data where they can toggle the year of the data as well as the degree type(Associate's, Bachelor's, Masters).  I was happy with the visualization, but there were a lot of donuts since I binded the donuts to the various areas of study so that visualization was very tall. Also it was tough to get the absolute graduation count for each ethnicity.  This is where **d3-tip** came in handy because it was easier to adopt then the *d3-mouse* function.  You can view the data visualization at [here](http://bl.ocks.org/rmhyman/1b09cba5086f5f540bbb8465e6f0166e).  After getting feedback, I thought that it would be better to group the visualization to illustrate the data over time, rather to break it down by areas of study.  So i switched my design to an stacked area chart based on the feedback.  I thought that I should use some other Data Visualization Theory so in my animation, I use color as pre-attentive attribute so that the focus could be on the under-represented ethnicities. The initial shows the graduation rate of the same three areas of study, but this time the animation focus was on the American Indian, Hispanic, and African American graduation rates. I had a tough time binding the areas of study to the buttons since some of the areas are not applicable to the Associate Degree type. To mitigate this, I decided to color those areas differently than the other buttons.  Thus only buttons that are red are applicable for the Associate Degree, but all of the buttons work for the Bachelor and Masters Degree type. You can see that visualization on this [gist](http://bl.ocks.org/rmhyman/raw/3435445362fea7b9d91d8943cbc20141).

After I received some feedback on that, I felt like I was not conveying my story in the best manner.  The attention that I wanted the user to focus on was not being captured.  So I decided to gather more data.  I scraped the internet for released *Equal Employment Opportunity*(EEO) reports released by tech companies.  I started my first Open Data repository from this activity and you can read more about that on my [OpenEEO](https://github.com/rmhyman/openeeo) repository. I wasn't able to acheive a way to perform transitions on my stacked bar chart, so I chose data that I have from 2014.  I chose EEO data from 2014 because I was able to find more EEO reports from tech companies that year and it was close to the years that I plotted from my NSF data.  You can view the EEO data from [2013](http://bl.ocks.org/rmhyman/raw/3197f5e86381f02db7f2f3a62c19f87b/) and [2015](http://bl.ocks.org/rmhyman/raw/1dd78f5db15d238f099f183d6585ca5d/). I also removed other majors that were not the central focus of my story.  I decided to focus on Computer Science, Electrical Engineering, and Mathematics since a large portion of people employed in the Engineering sector for these companies tend to come from these backgrounds.  After some enhancements in CSS and incorporating the Bootstrap framework, my final visualization was generated [here](http://bl.ocks.org/rmhyman/raw/50b5cd66b8f04d95cd05843789a02105).
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
