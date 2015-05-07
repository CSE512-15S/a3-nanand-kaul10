# a3-nanand-kaul10

# Team Members

1. Aditya Kaul kaul10@uw.edu
2. Nandita Anand nanand@uw.edu

# English Premier League - Team Performance Analysis for Season 2014 - 2015
**Data Domain** - Barclays English Premier League is a professional football premier league for men's association football clubs. There are a total of 20 clubs associated with this division. Each team plays a total of 38 matches including 19 home fixtures and 19 away fixtures. Each year the EPL season runs from August to May. 
Since the EPL season is currently in progress and very much in news, it got us interested and we thought of analysing the EPL data for the ongoing season. We decided to analyse the performance statistics of each team with regards to the number of matches they won, number of matches lost, number of goals scored, and number of goals conceded which would help us compare the teams with a higher points tally and the number of goals they scored. Also, it would help us understand which teams were in the relegation zone due to poor performance and higher number of goals conceded. Another important question we wanted to answer was whether a team scoring high number of goals was among the top contenders or not.

**Data Set** - For the purpose of this visualization we took the EPL statistics data from http://www.statto.com/football/stats/england/premier-league/2014-2015/table. It gives a tabular representation of the statistics which makes it a little hard for a casual observer to comprehend how different teams are performing individually and also with respect to others. This was also one of the motivations for us to work with this dataset and make it visually appealing and effective.

**Data Cleaning** - Since our data was in tabular format we preferred using a csv file to import all our data in order to carry out the visualization effectively. 

**Interaction Techniques and Reasons** - We attempted to incorporate the following interaction techniques in our visualization

1. **Mouse Hover**
  - We ensured that when the user would hover over the visualization, the bar over which the mouse pointer was present would turn into a different color in order to make viewing of the particular statistic easier for the user. 
  - We also introduced a transition time to ensure smooth transitioning from one bar to another and minimize the abrupt change in color.
  - In order to refer to the value of the bars, we introduced tooltip at the tip of the bars which would become visible to user on hovering the mouse over the respective bar.

2. **Selection via Buttons**
  - In order to visualize and analyse specific statistics for each team such as goals scored, goals conceded, matches won, total points et cetera, we included buttons in our visualization. We ensured that the button labels were self-explanatory and on clicking a specific button, its corresponding statistic would be displayed.
  - We introduced a delay of 1500 ms so that the transitioning of the bars from one window to another became smooth and visually appealing.

**The Final Visualization** - We have implemented a multi-view interactive visualization for the EPL Season 2014-2015 teams performance statistics. Users can explore different performance statisics by clicking on respective buttons in the visualization window. Users can also get the actual value of a statistic for a particular team by hovering over the corresponding bar which would not only display the value but also change the color of the bar.

# Running Instructions

Download this repository and run python -m SimpleHTTPServer 8888 and access this from http://localhost:8888/.

# Story Board

In order to create this interactive visualization we toyed with a couple of distinct visualization approaches. Below are our storyboards and corresponding description -

![StoryBoard1](https://github.com/CSE512-15S/a3-nanand-kaul10/blob/master/story_1.jpg?raw=true)

Initially we thought of taking the EPL data for all of the 20 teams and creating an interactive line chart visualization for the same. We thought of plotting the team details on the Y axis and the EPL statistics on the X axis. Depending on what statistic a user chose from a given list, the line charts would change and show relevant data.

However, owing to technical limitations we decided to modify our visualization design.

![StoryBoard2](https://github.com/CSE512-15S/a3-nanand-kaul10/blob/master/story_2.jpg?raw=true)

We also explored our dataset using bubble charts. Our idea was to plot interactive bubble charts showing each of the 20 teams' statistics such as matches won, matches lost, goals scored et cetera. In order to make our visualization more informative, we thought of including both multiple views for each of the statistic and interactivity on the click/selection of a bubble by a user. 

![StoryBoard3](https://github.com/CSE512-15S/a3-nanand-kaul10/blob/master/story_3.jpg?raw=true)

After much brainstorming, we decided to go with the above design for our visualization. We decided to use D3 to make interactive bar plots for our data based on different statisics. As can be seen from the design, we included buttons to allow users to explore individual statistics and also attempted to include features such as dynamic tool tip and sorting.

# Changes between Storyboard and the Final Implementation

Our storyboard guided our implementation. Having said that, we did change the placement of buttons on our visualization. We also modified some of the button labels from what we had thought earlier. Another addition to our actual implementation was, including time delays between button clicks and changing the color of the selected bar in a chosen bar chart. 

Note - 
1. We had planned to include sorting feature for bars on mouse-click. However, we couldn't implement the same. 
2. We also modified our older visualization (submitted on May 4, 2015) and were able to implement tool-tip for bars in this current visualization. This solved our earlier problem of not being able to distinguish which bar represented which club in the visualization. The tooltip now contains all the relevant information for each club and for each statistic. It also contains an image of the club logo for those interested. These are the additional features that we have added.

# Development Process

- As both of us didn't have significant prior experience in HTML, CSS, and JavaScript, we begun work on this assignment together by learning the basics of these technologies. We also devoted significant amount of time studying the nuances of D3.js. 
- Then, we brainstormed and came up with our respective interest areas and found some relevant datasets. We analysed the datasets to determine what kind of visualizations we could make. 
- After shortlisting our dataset, we cleaned and formatted the data so that we could use it in our code for visualization.
- Following cleaning, we began coding for one statistic only. We collaborated while coding since both of us were new to this technology and needed each other's help in resolving issues that came up.
- Once we had coded for one statitic, we enhanced the code to cover other statistics of interest to us. We also worked on labelling, formatting and colors of our visualization.

**Work Breakdown**

We roughly divided the work as follows -

**Aditya Kaul**
- Dataset exploration
- Interactive bar plot implementation
- Ascending and descending sort

**Nandita Anand**
- Dataset preparation
- Implemeting multi-view visualization using buttons
- Colors and layout

**Together**
- Data analysis
- Brainstorming and design
- Implementation and integration
- Writeup

**Effort Expended**

Below is the approximate time we spent per person on building the interactive visualization -
- Exploring online available datasets: 4 - 5 hours
- Data cleaning and data preparation: 4 - 5 hours
- Brainstorming and designing: 15 - 20 hours
- Coding (including re-work): 15 - 20 hours
- Learning HTML, CSS, JavaScript, D3: 40 -50 hours

**Challenging and Time Consuming Aspects**

- Learning D3
- Brainstorming and designing
- Data preparation in the correct format
- Implementing interaction features such as tool-tip

**Limitation**
- We would have liked to sort the bars in ascending or descending order in order to compare the teams at the top of the league or at the bottom, however due to technical limitations we could not implement the same.

**Reference**
- We used 'Interactive Data Visualization for the Web' by Scott Murray as reference for our code.
