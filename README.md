# Sentiment analysis for news
This repo use https://github.com/karpathy/arxiv-sanity-lite and get news from flask web server<br/>
News get from https://newsapi.org. using API <br/>

## Installation (python 3.9)
* 1.pip install -r requirements.txt<br/>

* Installation transformers u can use (https://github.com/pytorch/serve.git) <br/>
apt update<br/>
apt install -y default-jdk <br/>
pip install torchserve torch-model-archiver torch-workflow-archiver transformers openpyxl <br/>
python ./ts_scripts/install_dependencies.py<br/>

## Downloading news
* 2.News download from https://newsapi.org using API
* ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/news_api.jpg)
 we need run next scripts:<br/>
 python arxiv_daemon.py --num 1
 
 * run next script for compute some features:<br/>
 python compute.py
 
 ## Finally<br/>
 We run flask web server and get news sentiment analysis, 0-negative,1-neutral,2-positive:<br/>
 python serve.py 
 * ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/news_sentiment_analysis_1_1.jpg)
 * ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/news_sentiment_analysis_1_2.jpg)
 
## Metrics
* ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/metrics.jpg)

## Find best models
* ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/pictv1_1.jpg)
* ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/pictv1_3.jpg)
## Stack
* ![Image alt](https://github.com/shaimarus/news_sentiment_analysis/blob/main/stack.jpg)
