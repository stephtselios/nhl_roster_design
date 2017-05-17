# process of roster design analysis
## 1) import stored data frame.
## 2) fill in team code for all type of events (NaN values).
## 3) fill in home and visitor team code with the use of team code.
### - fill in home team code for all events prior to a goal.
### - fill in visitor team code for all events prior to a goal
## 4) goal number variable to be filled backwards for all event type prior to a goal.
## 5) goal time variable to be filled backwards for all event type prior to a goal, with the actual time of goal.
## 6) generate a variable that will calculate the time difference between events and goal.
## 7) keep only events that happened 20 seconds prior to a goal.
## 8) group events by goal number in a game.
## 9) create a column that will show the total observations for two games.
## 10) create columns for each type of event and assign values to determine the impact they have on a goal. When an event occurs a value of 1 will be assigned to the respectful event.
### - create a column that assigns a value of 1 to block events.
### - create a column that assigns a value of 1 to faceoff events.
### - create a column that assigns a value of 1 to giveaway events.
### - create a column that assigns a value of 1 to goal events.
### - create a column that assigns a value of 1 to hit events.
### - create a column that assigns a value of 1 to miss shot events.
### - create a column that assigns a value of 1 to penalty events.
### - create a column that assigns a value of 1 to shot events.
### - create a column that assigns a value of 1 to takeaway events.
## 11) display the incidence of each event in two games.
## 12) create a variable that will show the value of each event.
### the mean is used to determine the impact of each event on a goal.
## 13) determine if an event has a positive or negative impact on a team.
### - giveaway has a negative impact on a team.
### - faceoff has a positive impact on the team that won the faceoff and a negative impact on the team that lost.
### - hit has a positive impact for the team that delivered the hit and a negative impact on the team that received the hit.
### - penalty has a positive impact on the team that drew the penalty and a negative impact on the team serving. 
### - takeaway has a positive impact on the team that stole the puck and have possession.
## 14) create event value for home and visitor teams.
### - event value for home team. If an event has a positive impact on the home team, the mean will be positive. If an event has a negative impact on the home team, the mean will be negative.
### - event value for visitor team.  If an event has a positive impact on the visitor team, the mean will be positive. If an event has a negative impact on the home team, the mean will be negative.
## 15) assign the value of each event to the players that were on ice for both teams.
