# Final-Project : Recommender Sytem for Travel Destination Idea
<img src="home.jpg" width=700 height=432>
This project was made as a final project in my Data Science course in Purwadhika.

1. Background: <br>
  The project was initially inspired by my own wish to have such recommendation system to find a place which is suitable with my preferences. I want to make sure that my next destination offers activities that I enjoy on my previous holiday, for example. <br>
  I found that there are 2 out of 3 millenials are also interested in such service, according to SiteMinder (source: https://www.siteminder.com/r/trends-advice/hotel-travel-industry-trends/millennials-travel-20-interesting-stats-millennial-hotel-guests/), beside the budget consideration. <br>
  Since millenials are important target market to travel industry, that 82% millenials travelled last year compared to 75% of all other generations according to Condor Ferries's statistics (https://www.condorferries.co.uk/millennials-travel-statistics-trends), I consider that this service could be a huge help to companies in travel industry, or could also be useful for government to improve the tourism industry.
  
2. Dataset: <br>
  I retrieved the dataset by scrapping information from Trip Advisor.co.id, which encompasses data of travel destinations in Indonesia, the activities known in respective destinations, travel spots / vendors available, as well as hotel and flight information. <br>
  The final cleaned data has 320 travel destination data and its information, as well as around 27,000 travel spot and its information. <br>
  Travel spot in this respect is the specific places in the travel destionation. For example, in Jakarta (travel destination), there are spots such as Ancol, Ragunan zoo, or some shopping malls like Grand Indonesia, Central Park, etc (spots).

3.  Model: <br>
  I made a content-based recommender system with the activities their each offers as the features. I used cosine similarity as the final method for similarity metrics, although I also tried using Jaccard similarity and Speaerman correlation. <br>
  However, since recommender system needs online evaluation in order to know which method is better in achieving the goal, I decided to use cosine similarity for this project.
  In reality, if using cosine similarity seems to not have good enough result, we can try using other methods (such as Jaccard similarity or Spearman correlations, or others).

In the recommender system, the user is requested to input their preferences as shown below.
<img src="user_input.jpg"> 
<br>In the example, the user is planning to go with his/her friends, and s/he likes outdoor activities, nature, is adventurous, an adrenaline junkies, and likes to attend special events. We will see how this recommender system works and what the recommended place would be.
<img src="recom.jpg"> 
<br> The recommendation system resulted 6 top recommended places to go, which are some places in Bali (Karangasem, Legian, Blahbatuh, and Mengwi), Flores, and also Tuban (East Java). It also shows some recommended spots of each places, the approximate hotel and flight price from Jakarta. 

<br><br> css template from: https://www.free-css.com/free-css-templates/page256/tournest (with some modification)
