## Player Allocation
- Upon completion of evaluation of overall performance for all skaters, each player will be categorized and assigned to their respectful position within the roster of their team. The fundamental statistic used to differentiate top from bottom players, is zone start percentage. There are three zones from where plays can be started: offensive, neutral and defensive. Offensive zone start percentage is calculated by the number of face-offs held in the attacking area divided by the sum of face-offs an individual player was on the ice for. Identically, defensive zone start percentage is computed by the number of face-offs taken in their own territory divided by the total face-offs each player was on the ice for. Skaters who are talented in creating opportunities and producing goals will have a greater percentage of offensive zone starts in comparison to defensive zone starts. Equivalently, players who are skilled in preventing chances and goals being conceded, will have a higher defensive zone start percentage in correlation to offensive zone starts. In other words, top six forwards and top four pairing defensemen will start much of their shifts in the zone their opponent whereas bottom six forwards and bottom pairing defensemen in their own zone.
### 1) import data frame
### 2) create offensive, neutral and defensive zone starts
- zone start variable:
- a value of 1 will be assigned if the on-ice event happened in the offensive zone. 
- a value of 0 will be assigned if the on-ice event happened in the neutral zone. 
- a value of -1 if it happened in the defensive zone of the representative team.
### 3) home and visitor zone start
- If team code of event is the same as visitor team, the visitor zone start variable will be assigned identical value to zone start. If not, it will be assigned the opposite (negative) value of zone start.
- If team code of event is the same as home team, the home team will be assigned identical value to zone start. If not, it will be assigned the opposite (negative) value of zone start.
### 4) assign zone start to players
- the value of zone start is assigned to all players that were on ice, a total of 12 players (6 per team). The overall zone start variable of each player is the total (sum) of events they participated in.
- a) overall zone start of each player from the visitor team in all (6) positions
- b) overall zone start of each player from the home team in all (6) positions
### 5) allocate players per position to forward lines and defensive pairings
- If the zone start variable of a player for a given team is the highest in that specific position, it indicates that he participated in the most offensive zone starts. These skaters will be identified as **first line forwards and top defenisive pairing.**
- If the zone start variable of a player is the second highest in that specific position, it indicates that the given skater participated in the second most offensive zone starts. These skaters will be identified as **second line forwards and second defenisive pairing.**
- If the zone start variable of a player is the third highest in that specific position, it indicates that the given skater participated in the third most offensive zone starts. These skaters will be identified as **third line forwards and bottom defenisive pairing.**
- If the zone start variable of a player is the lowest in that specific position, it indicates that the given skater participated in the least offensive zone starts. These skaters will be identified as **fourth line forwards.**
