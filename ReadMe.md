# Wine Recommender, A Virtual Sommelier

## The Project

I wanted a way to find new wines, or a new wine variety, based on a bottle I already know I enjoy. I used 50,000 wine reviews from Wine Enthusiast Magazine to find features about a preferred wine to recommend something new. My recommender examines a wine review and uses two separate models to examine the description, and then finds similar features of a different wine and makes a recommendation. This is a content-based recommender because I am recommending a product with similar features the user already enjoys. I examined these two different models and determined which model is giving the best recommendation. 

## The Data
My dataset consists of wine reviews from Wine Enthusiast Magazine that were scrapped by zackthoutt. Here is a link to the page where the dataset is: https://www.kaggle.com/zynicide/wine-reviews. I used 50,000 wine reviews which consist of over 500 different varieties of wine. I examine the wine descriptions, which charaterize the wine's smells, flavors, and structure. I am looking for keywords that are unique to each bottle of wine to make a recommendation for a new bottle with similar keywords and characteristics. 


## The Recommender Models

### TF IDF Recommender

This model focuses on the importance of individual words and not just words that appear often. I want to focus on unique or rare words because they are going to be more important and indicative of the wine's characteristics. I chose a 2013 Cabernet Sauvingnon as my input, and I examined the recommended wines and their descriptions to find matching keywords. This model recommedned a wine with some similarity between the input wine.

![tfidf_results.png]

### LDA Recommender

This model focuses on topic modeling and finding themes of a document. Topics will be based on the words used in the wine description and these topics will be used to recommend a new wine with matching topics. 

Topic examples: 

Topic 1: Full, Fruits, Texture, Rich, Crisp, Fresh, Citrus, Apple, Spice, Light

Topic 1 has features like crisp, citrus, and apple which are commonly associated with white wines.

Topic 2: Black, Cherry, Spice, Berry, Note, Opens, Pepper, Plum, Oak, Full

Topic 2 has different red fruits like cherry and plum and differnt flavors like spice and pepper. These characterisctics are often found in red wines.



## Going Forward





