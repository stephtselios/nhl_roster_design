# Examination of efficient NHL roster design
## 1) import data frames
## 2) categorize data frames based on their similarity
### a) takeaways and giveaways
### b) goals, shots, missed shots (miss) and blocked shots (block)
### c) faceoffs, hits, penalty
## 3) merge data frames
### | merge takeaway and giveaway csv since columns are identical
### --------------------------------------------------------------------------------
### | merge goal and shot csv files
### | merge missed shots (miss) to the above merged data frame of goal and shot
### | merge blocked shots (block) to the above merged data frame of goal, shot, miss
### ---------------------------------------------------------------------------------------------------
### | merge faceoff and hit csv files
### | merge penalty to the aboved merged data frame of faceoffs and hits
### ---------------------------------------------------------------------------------------------------------------
## 4) merge merged data frames between each other
### | merge (a) (takeaway and giveaway) to (b) (goal, shot, miss, block)
### ---------------------------------------------------------------------------------------------------------
### | merge (c) (faceoff, hit, penalty) to the above merged file of (a) and (b)
### -----------------------------------------------------------------------------------------------------------------
## 5) merge detail play to all on-ice events (a), (b) and (c)
## 6) merge the above merged file to play by play (dm) csv file
## 7) merge detail scoring to play by play file to add 3 columns: goal number, assist player 1 and assist player 2
## 8) remove irrelevant observations: man-advantage scenarios and stoppage of play
## 9) keep only the first two games of the season for analysis
## 10) store final data frame¶
In [ ]:
