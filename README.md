# Capstone 3 Ideas

What could I do for capstone 3? I thought of a few ideas, some old, some new, and wrote them down here.

# Idea #1: Caption Generator

So initially I didn't want to do a caption generator (as an extension of my capstone 2) because I was afraid that I wouldn't know how to tie the computer vision element into it. 

But, after seeing Kyle's capstone, I thought "hey I could do a similar project, build my own captioner, and if I can get the computer vision to tie into it, that would be great, but otherwise I still have a captioner that I built myself."

So yeah, my favorite capstone idea at the moment is to train a caption generator. I would a few things, perhaps including training my own from large datasets, transfer learning based on the YouTuber that Kyle transfer learned from, and adding my own voice to the model. 

I would do a combination of the above approaches, and then try to change the program to learn from the screen. 

I would use openCV and tesseract to easily create a list of words on the screen at the moment, and then I would try to use those words to change the probabilities of the words being the words on the screens.  

While I might not get this last part to work, I think that I could give it a lot of effort and learn a lot and still have something to show for it (a caption generator) even if I don't get the last part to work.  

## #2: Time Series Forecasting For Inventory / Supply Chain

Nico told me that he never did enough time series forecasting, and told me about Maria's project before we even talked about it in class.  He said it was difficult and super useful, and I believe that I would learn a lot by doing this project.  

### Possible Datasets:

- [https://www.kaggle.com/vijayuv/onlineretail?select=OnlineRetail.csv](https://www.kaggle.com/vijayuv/onlineretail?select=OnlineRetail.csv)
    - This includes 500,000 rows of sales data from an online retail store, each row containing data on what was purchased, a unique customer ID, how many they purchased, when they purchased, and the price of purchase.
    - From this I think I could do customer segmentation and time series forecasting using a variety of methods. I could use an LSTM, WaveNet, ARIMA, and other simpler practices to predict sales

- [https://www.kaggle.com/manjeetsingh/retaildataset](https://www.kaggle.com/manjeetsingh/retaildataset)
    - This dataset has much more information than the last, but doesn't have info about specific customers. Is this Maria's dataset? It doesn't say Walmart but it sure looks like it.
    - It has better features, such as when holidays are, the unemployment rate, the CPI, and fuel price.  The sales data is 2-3 years of data from 45 different stores
    - If this were the stock market, trying to predict it would be stupid because if you can predict it, people are already putting their money into it before you. But, with store sales, if you can predict your sales volume, this doesn't influence the future and you can just be better prepared by warehousing inventory better and saving more money.  If you can predict sales volume beautifully, you can keep less safety stock on hand, and your warehousing costs go down. Also you don't need to have capital tied up in unneeded inventory.  This is how you can save money in a supply chain.
    - Perhaps I can compare sales forecasting with forecasting the stock market and talk about chaotic theory.

    ## Idea #3: Cologne Recommender

    If I scraped the website [Fragrantica.com](http://fragrantica.com) similar to how [this guy](http://cs229.stanford.edu/proj2016spr/report/024.pdf) did, I could create a recommender system of fragrances.  Now, I wouldn't have any user data to use (no user-user similarity) but if I scraped this, there is a lot of great data that I could use to recommend similar fragrances.  I would need to scrape the website really well though, somehow finding a way to go to the URL's of every fragrance posting... not sure how to find this directory on the site. Web crawler? I think so? 

    I would make a Flask app recommending people new fragrances based on fragrances that they enjoy, and I would give them leveraging in weighting what factors they deem important to the recommendations I provide.