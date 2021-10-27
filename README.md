# Exploring UFO Sighting Data
## Overview

> In this project we are using HTML, CSS, and different Javascript libraries to analyze UFO sightings with data that we are provided. We will use D3.js to allow us to transfer the array of js objects into a table on our index.html page. Our main goal is to add the appropriate filters on the HTML page that correspond to the characteristics of each sighting (city, country, state, date, shape). Using these filters we want an updated table that will correctly 
filter the data based on the user's inputs to be returned. 
---

## Results
After working through the code we were able to create a working website that correctly filtered the data.
Here is a walkthrough on how to use the filters when searching:

1. You will be brought to the main "UFO Sightings" page which will include the complete dataset in the table.
![](https://github.com/mooshak21/UFOs/blob/main/static/images/mainPageNoFilter.png)

2. The page will already have the format for the input values. Once you put in a value that is contained in the dataset, the filtered table will be returned. In this case, I searched for the sightings in **City**: el cajon and **State**: ca. Note that the state field will require the two character code for the state.
![](https://github.com/mooshak21/UFOs/blob/main/static/images/filterCityState.png)

3. You can do the same with the other filters sing the format to get the desired results.
---

## Summary
### Drawbacks of design
1. One drawback of the design we chose is the fact that there is no button to submit the results. Instead we are receiving live updates to the table data. While this can be seen as a good thing, I think it would be better to return the new filtered table once we clicked a submit button. While we are searching and the user input doesn't match any of the table data, the table is blank until the user input matches a value in the table (seen in image below). It would be more beneficial for the user to be able to see some of the table while they are searching in my opinion. 
![](https://github.com/mooshak21/UFOs/blob/main/static/images/drawback.png)
![](https://github.com/mooshak21/UFOs/blob/main/static/images/drawback2.png)

### Recommendations
1. I feel like some examples values should be included for some of the input fields. For example, if someone comes to the page for the first time and has no idea what they are doing, they might not know what to input into the "shape" field. Including some specific options in a key or legend would be helpful. Additionally, adding the date range that the sightings span from would be helpful beacuse in our dataset it only includes around 13 days of observations. 

2. Another recommedation applies to this dataset specifically. Since all of the observations are within the US, there is no real need to have an input field for country. It isn't too big of a deal but if it is not necessary then we shouldn't have to include it. If this was a dynamic sataset that was getting constant changes then I could see its benefit.

3. Expanding on the point above, if there was a live dataset that was getting changes, we could incorporate flask/mongo to do something similar to last project. We would be able to retrieve live data and update the table with all of the changes and make the application more dynamic. This is less of a recommendation and more a cool way to expand on this topic to add more of the skills we have learned. 