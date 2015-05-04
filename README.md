# a3-nanand-kaul10

# Team Members

1. Aditya Kaul kaul10@uw.edu
2. Nandita Anand nanand@uw.edu

# English Premier League - Team Performance Analysis for Season 2014 - 2015
Data Domain - Barclays English Premier League is a professional football premier league for men's association football clubs. There are a total of 20 clubs associated with this division. Each team plays a total of 38 matches including 19 home fixtures and 19 away fixtures. Each year the EPL season runs from August to May. 
Since the EPL season is currently in progress and very much in news, it got us interested and we thought of analysing the EPL data for the ongoing season. We decided to analyse the performance statistics of each team with regards to the number of matches they won, number of matches lost, number of goals scored, and number of goals conceded which would help us compare the teams with a higher points tally and the number of goals they scored. Also, it would help us understand which teams were in the relegation zone due to poor performance and higher number of goals conceded. Another important question we wanted to answer was whether a team scoring high number of goals was among the top contenders or not.

Data Set - For the purpose of this visualization we took the EPL statistics data from http://www.statto.com/football/stats/england/premier-league/2014-2015/table. It gives a tabular representation of the statistics which makes it a little hard for a casual observer to comprehend how different teams are performing individually and also with respect to others. This was also one of the motivations for us to work with this dataset and make it visually appealing and effective.

Data Cleaning - As the original data was in a tabular form, we couldn't use it directly in our code. Thus, we converted this data to the JSON format so that we could readily use/import it in our D3 code and create effective and interactive visualizations. 
<Name of JSON data file - EplData.JSON>

Interaction Techniques and Reasons - We attempted to incorporate the following interaction techniques in our visualization 
1. Mouse Hover
  - We ensured that when the user would hover over the visualization, the bar over which the mouse pointer was present would turn into a different color in order to make viewing of the particular statistic easier for the user. 
  - We also introduced a transition time of 0.3 seconds to ensure smooth transitioning from one bar to another and minimize the abrupt change in color.
  - In order to refer to the value of the bars, we introduced labels at the tip of the bars which would become visible to user on hovering the mouse over the respective bar.
2. Sorting via Mouse Click
  - As an important part of our question was to figure out the top contenders for the title and the teams facing relegation, we incorporated sorting feature so that a user could sort the data/bars in either ascending or descending order and easily decipher which teams belonged to the aforementioned catergories.
  - On the 1st click within the visualization layout, the bars would get sorted in descending order.
  - On the 2nd click within the visualization layout, the bars would get sorted in ascending order.
3. Selection via Buttons
  - In order to visualize and analyse specific statistics for each team such as goals scored, goals conceded, matches won, total points et cetera, we included buttons in our visualization. We ensured that the button labels were self-explanatory and on clicking a specific button, its corresponding statistic would be displayed.
  - We introduced a delay of 1500 ms so that the transitioning of the bars from one window to another became smooth and visually appealing.

The Final Visualization - We have implemented a multi-view interactive visualization for the EPL Season 2014-2015 teams performance statistics. Users can explore different performance statisics by clicking on respective buttons in the visualization window. Within a particular statistic plot or window, users can sort the data in ascending or descending order to analyse it from varied perspectives. Users can also get the actual value of a statistic for a particular team by hovering over the corresponding bar which would not only display the value but also change the color of the bar.

# Running Instructions

Access our visualization at http://cse512-15s.github.io/a3-nanand-kaul10/ or download this repository and run python -m SimpleHTTPServer 8888 and access this from http://localhost:8888/.

# Story Board

In order to create this interactive visualization we toyed with a couple of distinct visualization approaches. Below are our storyboards and corresponding description -

![StoryBoard1](https://github.com/CSE512-15S/a3-nanand-kaul10/blob/master/story_1.jpg?raw=true)

![StoryBoard2](https://github.com/CSE512-15S/a3-nanand-kaul10/blob/master/story_2.jpg?raw=true)



# Changes between Storyboard and the Final Implementation

A paragraph explaining changes between the storyboard and the final implementation.

# Development Process

Include:

Breakdown of how the work was split among the group members.
A commentary on the development process, including answers to the following questions:
Roughly how much time did you spend developing your application?
What aspects took the most time?
Challenges
