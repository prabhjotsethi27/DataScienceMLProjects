## Description
- This is a code to access the Twitter API once you have a Developer account with Elevated Access. 
- In case you don't get the Elevated access, then you may refer to this link -https://www.kirenz.com/post/2021-12-10-twitter-api-v2-tweepy-and-pandas-in-python/twitter-api-v2-tweepy-and-pandas-in-python/

## Steps taken to access Twitter API and search tweets for "Covid"
The steps taken to complete the task are explained below:

1.	It started with exploring the process of creating a Twitter Developer account, which took quite some time in setting up the same. 
2.	It involved creating a new Project in the Developer account and changing its access rights to "Read and Write." 
3.	The API authentication details like the API key and secret and access details like access token and secret were to be saved in a separate config file called "config.ini" so I could use it to send calls to the Twitter API. The file is saved in the root location where Python code resides.
4.	Two new Python libraries - "tweepy" and "configparser" - were required to be installed to perform this task. It is simpler to login and use the Twitter API with Tweepy, a free Python wrapper. These were installed using "pip install" in Jupyter.
5.	A new jupyter notebook file was created where the following code steps were written:
•	Importing the Python three libraries - tweepy, configparser and pandas.
•	The code was written to authenticate the Twitter API using Tweepy. The authentication credentials from the "config.ini" file were read and then passed to Tweepy's auth () method.
•	After configuring authentication, we'll use the search_tweets() function of the authentication object to retrieve tweets, loop over them, and display the content.
•	I used a filter of the "covid-19" keyword and search date as parameters to get filtered tweets and iterate over them. You can change this filter and search tweets related to any keyword.