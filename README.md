# Final-Project-Statistical-Modelling-with-Python

## Project/Goals

(fill in your description and goals here)

This project tested the application of python-based libraries in exploratory data analysis and statistical modelling. This was with the aim to utilizing .JSON files sourced from specific websites (citybikes and foursquare) with the aid of API keys. The project was in four phases viz.: successfully extract information from citybikes in a named city (I selected Paris); successfully call information on citybikes website by using foursquare; successfully join the parsed dataframes from the fist two activities; and  store the dataframes in a SQLite database and successfully model the dataframe.

## Process

### (your step 1)

First, I generated information about citybikes in Paris, being my city of choice, then I produced a dataframe which contained information on the location, station name (later renamed name\_x in the combined dataframe), empty\_slots and free\_bikes, of city bikes in Paris. This process did not involve the use of API key. After parsing the information into a dataframe, it was converted into a .csv file for use in a different text editor.

A similar process was used to retrieve information on places of interest, such as bar, restaurant, cafe, gym, pharmacy, etc, in Paris. This was done in foursquare website with known endpoint and API key. After GET-ting the JSON dictionaries, it was parsed into a dataframe which was converted into .csv file for use in a different text editor. 

### (your step 2)

Once the two dataframes had been retrieved, they were merged using cross-joining and named. Further exploratory data analysis were then conducted on the merged dataframe. 

## Results

(fill in what you found about the comparative quality of API coverage in your chosen area and the results of your model.)

The results of the linear regression analysis revealed that the predictor variables were not enough to predict the availability of bikes in the stations in Paris. Although empty\_slots and free\_bikes were both target variables, only empty\_slots showed a significant relationship with free\_bikes. Furthermore, the classification model was not a great one because the predictor variables could not impartially predict bike availability. For instance, the model showed high bias for low availability of bikes in Paris. When category counts were included in the model, they showed a little negative to negligible impact on the building of the model. Distance did not have any impact on the model prediction.

## Challenges

(discuss challenges you faced in the project)

My kernel crashed in Jupyter lab on several occasions, which slowed my work down. Furthermore, I could not access Yelp and as such I was unable to carry out a comparative test between the results retrieved from there and foursquare. Additionally, my logistic regression model refused to work for some reasons even after casting the objects to integer, as such, I resorted to the use of classification method. I will have to remove my API key before pushing my project to GIT, since I was unable to get it saved to a system environment. I was unable to call it with the OS library, so I had to manually input it in the code. If I had a little bit of time, I would have gotten it sorted. Finally, despite saving some of my codes which worked before the crashing of my kernels in jupyter lab, these codes refused to work after loading my libraries. The workaround was unsuccessful and I was delayed by at least 7 hours while trying to find a solution.

## Future Goals

(what would you do if you had more time?)

Unfortunately, there was little time allotted for the completion of this project, coupled with the technical issues and difficulties I experienced. These made it impossible for me to fully do an indepth EDA on the combined dataframe. I have learnt a few things on this project and still learning as we go on. 

