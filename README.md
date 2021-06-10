# KpopGroupReview

## Problem statement

Working in one of the major music entertainment company in korea, our company has multiple music group of various performance under our care. The competition in this industry is very tough. Every music group have to ensure they are constantly able to bring about new music to contiune to capture their audience or to capture new ones to remain in the industry. Once they are unable to do so other group will take this oppertunity to overtake them. The role of the music entertainment company is not only to help promote the exsiting music group but to also recuit trainees and prepare them for their debut should there be signs of the music group on the verge of disbandment. However this is a long process, as new trainees often have to go through many years of training before they are even considered when a new group is slated to be form. Thus a way to identify the remainding time before a group would be disbanded would help save the company time and resources spent on the trainees. Thus we are tasked to come up with a model to predict the expected lifespan for a music group before it would be disbanded, identify current and future music group trend.

## Dataset
**Datasets:**
<details>
  <summary>Click here to show Datasets!</summary>

  |Dataset|Description|Source|
  |---|---|---|
  |KpopTrend2004To2021.csv|shows the trending value of keyword "KPOP" from 2004 to 2021|www.googletrend|
  |MusicGroup.csv|details of all the music groups from 1990 to 2021|https://kpop.fandom.com/|
  
</details>

**Data Dictionary:** Explains the features found in the datasets
<details>
  <summary>Click here to show Data Dictionary!</summary>
  
  |Feature|Type|Dataset|Description|
  |:---|:---|:---|:---|
  |**group_name**|*object*|MusicGroups.csv|Name of the KPOP group|
  |**company**|*object*|MusicGroups.csv|Name of the Company KPOP group is under|
  |**group_type**|*object*|MusicGroups.csv|Male or Female group|
  |**debut_year**|*int*|MusicGroups.csv|Year they officially debut|
  |**disband_year**|*int*|MusicGroups.csv|Year they offically disband|
  |**current_status**|*object*|MusicGroups.csv|Active or Disband|
  |**social_account**|*int*|MusicGroups.csv|Number of social media accounts|
  |**inactive_members**|*int*|MusicGroups.csv|Number of inactive members|
  |**current_members**|*int*|MusicGroups.csv|Current number of members|
  |**original_members_remainding**|*int*|MusicGroups.csv|Number of original members still with the group|
  |**initial_members**|*int*|MusicGroups.csv|Inital number of members|
  |**member_changes**|*int*|MusicGroups.csv|Number of member changes|
  |**subunits**|*int*|MusicGroups.csv|Number of sub-units|
  |**albums**|*int*|MusicGroups.csv|Number of album released|
  |**mini_albums**|*int*|MusicGroups.csv|Number of mini album released|
  |**other_albums**|*int*|MusicGroups.csv|Number of other types of album released|
  |**singles**|*int*|MusicGroups.csv|Number of single released|
  |**digital_singles**|*int*|MusicGroups.csv|Number of digital single released|
  |**other_singles**|*int*|MusicGroups.csv|Number of other type of single released|
  |**foreign_albums**|*int*|MusicGroups.csv|Number of album released in a foreign language|
  |**foreign_mini_albums**|*int*|MusicGroups.csv|Number of mini album released  in a foreign language|
  |**foreign_other_album**|*int*|MusicGroups.csv|Number of other types of album released in a foreign language|
  |**foreign_singles**|*int*|MusicGroups.csv|Number of single released in a foreign language|
  |**foreign_digital_singles**|*int*|MusicGroups.csv|Number of digital single released in a foreign language|
  |**foreign_other_singles**|*int*|MusicGroups.csv|Number of other type of single released in a foreign language|
  |**others**|*int*|MusicGroups.csv|Other kind od releases|
  |**last_production_year**|*int*|MusicGroups.csv|The year of the last released activity|
  |**total_releases**|*int*|MusicGroups.csv|Total number of releases regarless of type|
  
</details> 

## Executive summary

** Work In Progress **

## Conclusions and Recommendations

** Work in Progress **


## TO DO LIST 

    1) Problem Statement
        1.1) Determine Baseline

    2) Data gathering 
        2.1) Initial Collection done.
        2.2) Could find more features after everything is done?

    3) Cleaning
        3.1) Varify input values (Years are within range)
        3.2) Handle null values (for groups that are still active)
        3.3) Standard cleaning (lower cases, remove spaces)
        3.4) Seperate Actives and Disband groups
        3.5) Train/Test on Disband portion, Select a subset from Active group to predict on.

    4) EDA
        4.1) Distribution of Activities
        4.2) Distribution of Local/Foreign Activities
        4.3) Average Activities across their lifespans (could be a feature)
        4.4) Any difference between Male groups and Female groups? (yes,no? will the ols shows the same?)
        4.5) Years to disband since last activities (cannot be a feature but interesting to know)
        4.6) Something on the Companies? (the big three? do they perform better than other companies? use median lifespan as a performace indicator )

    5) Modeling
      5.1) Choosing regression methods

    6) Evaluation

    8) Summary and Review
