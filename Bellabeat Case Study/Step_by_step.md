## Step by step
These are the steps of how I approached the Bellabeat case study, which are the steps taught by Google Data Analytics Course. 

## 1. Ask
Define what the project would look like and what would qualify as a successful result

Guilding questions from case study:
* What is the problem you are trying to solve?
  * What are some trends in smart device usage?
* How can your insights drive business decisions?
  * How could these trends apply to Bellabeat customers?
  * How could these trends help influence Bellabeat marketing strategy?

## 2. Prepare 
Download the data from 'https://www.kaggle.com/datasets/arashnic/fitbit'

Guilding questions from case study:
* Where is your data stored?
  * Google Cloud Platform
* How is the data organized? Is it in long or wide format?
  * It is organised by their title, for instance, if they are related to daily data, the file title will start with daily. 
* Are there issues with bias or credibility in this data? Does your data ROCCC?
  * It was not downloaded from Bellabeat.   
* How are you addressing licensing, privacy, security, and accessibility?

* How did you verify the data’s integrity?

* How does it help you answer your question?

* Are there any problems with the data?
  * Google Cloud Platform is taking long time on joining them. 

## 3. Process 

Guiding quesions from case study:
* What tools are you choosing and why?
* Have you ensured your data’s integrity?
* What steps have you taken to ensure that your data is clean?
* How can you verify that your data is clean and ready to analyze?
* Have you documented your cleaning process so you can review and share those results?

```sql
SELECT  
hi.Id,hi.activityhour,hi.totalintensity, hc.calories
FROM 
`ferrous-destiny-344108.Fitabase_Data.hourly_intensities` hi
JOIN
`ferrous-destiny-344108.Fitabase_Data.hourly_calories` hc
ON 
hi.id = hc.id

```

```SQL
SELECT  
hci.id, hci.activityhour, hci.calories, hci.totalintensity, hs.steptotal
FROM
 `ferrous-destiny-344108.Fitabase_Data.hourly_c_i` hci
JOIN
`ferrous-destiny-344108.Fitabase_Data.hourly_steps` hs
ON
hci.id = hs.id
```

## 4. Analyze 


## 5. Share 


## 6. Act
