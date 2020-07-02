# Data-processing-and-searching
The project was built by two sub open-sources projects of Apache Foundation, POI and Lucene, to process and analyze data from twitter. In addition, we construct the demo of search engine based on these data.

## Installation
You can use the Maven to download the API of POI and Lucene or just import the relevent API from the file of Additional Library.

## DataSet
The coursework uses a subset of the dataset (file name: twitterDataset.xlsx) published at http://followthehashtag.com/. It contains 204,820 short messages (tweets) collected from Twitter (https://twitter.com), during the period of 14-16, April, 2016, from various locations in the United States. The dataset contains many different topics, e.g., weather, leisure, sports, etc.

The dataset is stored in an EXCEL file and needs to be processed from your Java program. Each record (row) contains information about a tweet. The columns are explains as follows. 
•	Tweet Id – the ID of a tweet  
•	Date – the date on which a tweet is published  
•	Hour – the time when a tweet is published  
•	User Name – name of a user  
•	Nickname – nickname of a user  
•	Tweet content – the actual message  
•	Favs – number of users who like the tweet  
•	RTs – number of users who re-tweet the tweet (republish)  
•	Latitude – latitude of the location where a tweet is published  
•	Longitude – longitude of the location where a tweet is published  
•	Followers – number of followers of a user (the values are the same for the same user)  

## Data Processing, Analysis 
You need to write code to extract data from the dataset(EXCEL) and then perform some simple data analysis.
```
Requirements:
•	T3-1: load data in the program.
•	T3-2: print top 10 tweets. Tweets should be ranked based on the sum of: (1) number of users who like the tweet (Favs), and (2) number of users who re-tweet the tweet (RTs). Relevant information, such as when, and by whom it is published, should also be shown.
•	T3-3: print top 10 users. Users should be ranked based on the number of followers that they have
```
## Content Search
Effective tweet searching is an important functionality for users, especially when there are millions of tweets published in each single day. The search process takes a user’s input keyword as a query and then retrieves relevant tweets. Two simple searching strategies are considered.

1.	Text matching – The idea is to find tweets based on matching the user’s keyword (only one word) with all the tweets. A tweet is regarded as relevant if the keyword appears in it. This is a basic feature of the application.

2.	Full text search – This is considered as an advanced feature of the application. To simplify the problem, you do NOT need to study the techniques in the field of Information Retrieval. According to the research reported in [1], the full text search functionality on Twitter is based on a modified version of the Apache Lucene API. However, the actual full text search on Twitter is extremely complicated. This coursework only attempts to build a much simpler full text search engine based on the original Lucene API, only for limited amount of Twitter data. Lucene can be downloaded at: https://lucene.apache.org/core/. A tutorial is available here: https://lucene.apache.org/core/7_7_1/demo/overview-summary.html. 
```
•	T3-4: tweet search based on string matching.
•	T3-5: tweet search based on full text searching using Lucene.
```

## Usage
T3-2: It prints the top 10 popular tweets based on the Favs and RTs.  
![image](https://media.giphy.com/media/l3sL4wNSk35zpIraSk/giphy.gif)

T3-3: It prints the top 10 popular users based on the Fans.  
![image](https://media.giphy.com/media/gFJoPWsLzWtXIoN3V3/giphy.gif)

T3-4: It prints search information based on string matching.  
![image](https://media.giphy.com/media/ggEngsaoMfoE00Z5qt/giphy.gif)

T3-5: It prints search information based on full text searching using Lucene.  
![image](https://media.giphy.com/media/PhBjLu0eQIkjYZ2QbH/giphy.gif)


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

