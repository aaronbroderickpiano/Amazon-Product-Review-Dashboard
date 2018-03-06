# Amazon-Product-Review-Dashboard

The finished dashboard is here.

Impact Analysis
https://plot.ly/dashboard/aaronbroderickpiano:34/view?share_key=jNG1qLEKJqP71Vdn3u6tqi


x_axis = The number of upvotes a review received.  Denoted as HelpfulnessNumerator in the original data set.

y_axis = Product review score.  5 is the best.  

Diameter of the circle = Reviewer expertise.  Calculated by counting the total number of reviews by that reviewer in the dataset.  A big circle means reviewer has written many reviews.  

Slider =  Length of time from the first review.  Calculated by determining the number of days the review was written from the first review written about the product.  Divided into 10 buckets.

Hover = Summary of the review.  Tf_idf and then using the pagerank algorithm for the most representative sentence.  



Subject Clustering
https://plot.ly/dashboard/aaronbroderickpiano:35/view?share_key=Pi2A7ops21jC6TlLSjYqXT


1. Parse for nouns using spaCy

2. Tf_idf

2. Calculate gap statistic.  Get recommended number of clusters. 

3. Calculate LSA based on n clusters from gap statistic.  

4. Plot words by LSA score and cluster

Orignal dataset aquired here https://snap.stanford.edu/data/web-FineFoods.html
