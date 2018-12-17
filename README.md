# MSDS696
Final project for Regis MSDS696 - Denver Bike Map and Text Analysis
Meng Luo

## 1. Project discription

### a. High level description of the project: what question or problem are you addressing?
The project is trying to create an interactive map for cyclists around Metro Denver area to show them the available bike trails, lanes, as long as some nearby community news and events. 

### b. What type of data science task is it? 
Data collection, visualization and text analytics.

### c. Brief description of data.
The first part of the project is the map itself. The geo data is available to the public provided by DRCOG and organizations such as Bike Denver. The data sets are relatively small. 

The second part is the recent or upcoming events for the nearby area. It is scraped from Bike Denver and Bicycle Colorado for Decemeber, January and Feburary.

(Originally, I was planning to find available data/APIs from Strava, MeetUp and Reddit. I either never received permissions or the API is too advance for me.)

### d. How do you analyze the data? What machine learning methods do you use?
Data analytics main applies to the 2nd part of the project. I was able to collect tweets based on certain keywords, and then apply lemmatization and Sentiment Intersity Analysis (SIA) upon them and create masked word cloud to show the most common words.
 
## 2. Main achievements and problems 
### a. Main achievements
- Used new techniques not covered in the course: GeoJSON, folium, geopandas, masked word cloud.
- Practiced on obtain new data sets and how to clean/transform a new data set.
- Successfully created a html file for the interactive map with layers to show event popups with details.
- Successfully analyzed the tweets collects for Denver and other cities.
### b. Main problems
- The original GeoJSON file is too large to load in real time. I had to shrink it.
- Cleaning datasets consumed the majority of the project time. 
- Right before submitting the project, the Twitter API is locked and I couldn't show the text anlytics results to compare different cities.

### c. What have I learnt from this project
- Available data is far from usable data. Never make plans based on when we obtain the data. It needs to be cleaned, transformed, loaded first. 
- Data collecting and preparation did take 80% of a data scientist's time.
- Text analytics is quite fun with very interesting results. (I see people are talking more about giving bike as a gift rather than icy hazards on the road and the tweets are getting much more positive in the holiday season) However, I need to make the results more visually attractive.

## 3. Conclusions

The proejct shows Denver's bike lanes and events as an html page [https://milite.github.io/MSDS/index.html]. We also conduct text anlytics against twitter on Denver bikes and cycling. 

It seems not that hard to load GeoJSON files with the folium package in Python and present them as .html files. Text analytics is useful when it comes to tweets to gather people's opinions. However, the most important thing I learnt from this project is that, it is no joke data collecting and preparation is the hardest part of being data scientist. Now I am more skillfull and ready to tackle these issues.


## References

Bicycle Colorado Event Calendar.(2018, Decemeber).*Bicycle Colorado*.Retrieved from https://www.bicyclecolorado.org/events/

Bicycle Facility Inventory Dataet.(2018).*Denver Regional Council of Governments*.Retrieved from https://data.drcog.org/dataset/bicycle-facility-inventory

Bike Denver Events page.(2018, December).*Bike Denver*.Retrieved from https://bikedenver.org/events/

Course materials from MSDS680,682,and 696.(2018).*Regis University*.
