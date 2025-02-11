# Wine Recommender, A Virtual Sommelier

## The Project

I wanted a way to find new wines, or a new wine variety, based on a bottle I already know I enjoy. I used 50,000 wine reviews from Wine Enthusiast Magazine to find features about a preferred wine to recommend something new. My recommender examines a wine review and uses two separate models to examine the description, and then finds similar features of a different wine and makes a recommendation. This is a content-based recommender because I am recommending a product with similar features the user already enjoys. I examined these two different models and determined which model is giving the best recommendation. 

## The Data
My dataset consists of wine reviews from Wine Enthusiast Magazine that were scrapped by zackthoutt. Here is a link to the page where the dataset is: https://www.kaggle.com/zynicide/wine-reviews. I used 50,000 wine reviews which consist of over 500 different varieties of wine. I examine the wine descriptions, which characterize the wine's smells, flavors, and structure. I am looking for keywords that are unique to each bottle of wine to make a recommendation for a new bottle with similar keywords and characteristics. 

### This is an example of a wine review.

![](images/wine_review.png)

### The average wine review is 200-250 characters long.

![](images/char_count.png)

### Of my 50,000 wine reviews, 95% come from these ten countries with the majority being from the United States and the top 5 rounded out with European countries.

![](images/top_ten_countries.png)


## The Recommender Models

### TF IDF Recommender

This model focuses on the importance of individual words and not just words that appear often. I want to focus on unique or rare words because they are going to be more important and indicative of the wine's characteristics. I chose a 2013 Cabernet Sauvignon as my input, and I examined the recommended wines and their descriptions to find matching keywords. This model recommended a wine with some similarity between the input wine.

![](images/tfidf_results.png)

### LDA Recommender

I used the same 2013 Cabernet Sauvignon for my input. This model focuses on topic modeling and finding themes of a document. Topics will be based on the words used in the wine description and these topics will be used to recommend a new wine with matching topics. 

Topic examples: 

Topic 1: Full, Fruits, Texture, Rich, Crisp, Fresh, Citrus, Apple, Spice, Light

Topic 1 has features like crisp, citrus, and apple which are commonly associated with white wines.

Topic 2: Black, Cherry, Spice, Berry, Note, Opens, Pepper, Plum, Oak, Full

Topic 2 has different red fruits like cherry and plum and differnt flavors like spice and pepper. These characterisctics are often found in red wines.

The LDA model has done a better job of recommending a wine because there are more matching characteristics of the wines.

![](images/lda_results.png)



## Going Forward


In the future, I want to add to this project by adding another way to recommend a wine. I want a user to be able to enter in their own description, and then have a wine recommended from their own custom input. The model works now by having a user select a bottle of wine from the dataset and then having a wine recommended. Allowing a user to customize their own input allows more freedom for the consumer. Adding a price feature is needed as well because wines can vary in price, so this is also beneficial for the consumer. 


