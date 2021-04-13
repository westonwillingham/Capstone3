# Capstone 3 Ideas

What could I do for capstone 3? I thought of a few ideas, some old, some new, and wrote them down here.

## #1: Time Series Forecasting For Inventory / Supply Chain

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

    ## Idea #2: Cologne Recommender

    If I scraped the website [Fragrantica.com](http://fragrantica.com) similar to how [this guy](http://cs229.stanford.edu/proj2016spr/report/024.pdf) did, I could create a recommender system of fragrances.  Now, I wouldn't have any user data to use (no user-user similarity) but if I scraped this, there is a lot of great data that I could use to recommend similar fragrances.  I would need to scrape the website really well though, somehow finding a way to go to the URL's of every fragrance posting... not sure how to find this directory on the site. Web crawler? I think so? 

    I would make a Flask app recommending people new fragrances based on fragrances that they enjoy, and I would give them leveraging in weighting what factors they deem important to the recommendations I provide.  

    ## Idea #3: Caption Generator

    I would build my own caption generator (I guess similar to Kyle's capstone 3) that could perhaps be modified to use computer vision to look at words on the screen and update... the Euler-"Oil or" problem.  

    I would use the Mozilla Voice dataset, maybe a Kenlm rules based language model, and a rescoring algorithm like ctcbeamscore. I don't really know what these do off the top of my head, but I looked at a few YouTube videos of a guy building a caption generator from scratch.