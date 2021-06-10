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


## Conclusions and Recommendations

We are able to identify some of the more popular bands and is able to assign them with a longer lifepsan as compare to others.
When sorted by longest lifespan or latest disband date we get interesting groups which reflect the trend of a certain generation of Kpop music group.
We have shown that we are able to predict the lifespan of a music group to an extend. However the RMSE is considered high still thus more data collection will be required to lower the score. Preferbly having more detailed dates of their disbandments (in terms of months instead of years) would help to improve the results.
We also highlighted that show that active music groups are starting to plateau. Thus it might be an indicator that its not a good time to introduce more group to the industry and also identified the features that helps extend the lifespan of music groups.


