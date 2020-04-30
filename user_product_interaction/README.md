# Understanding user and product interaction

Amazon’s employee travel provider has asked you to review how users interact with their online travel website.
They store their data in JSON files. Each row in these files lists all the different cities that have been searched for by a user within the same session (as well as some other info about the user). 

## Business Questions

1- There was a bug in the code and one country didn't get logged. Can you guess which country? How?<br>
2- For each city, find the most likely city to be also searched for within the same session.<br>
3- Travel sites are browsed by two kinds of users. Users who are actually planning a trip and users who just dream about a   vacation. The first group obviously has a much higher purchasing intent. Users planning a trip often search for cities close to each other, while users who search for cities far away from each other are often just dreaming about a vacation (or a great work trip!). Based on this idea, come up with an algorithm that clusters sessions into two groups: high intent and low intent.<br>

## Data Details

The data provided is in JSON format and include fields that can be summarised as below:

Fields:<br>
*session_id*: session id. <br> 
*unix_timestamp*: unix timestamp of session start time <br> 
*cities*: the unique cities which were searched within the same session <br> 
*user*: <br> 
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *user_id*: the id of the user <br> 
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *joining_date*: when the user created the account<br> 
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; *country*: where the user is based <br>
