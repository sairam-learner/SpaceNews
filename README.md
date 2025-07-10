SpaceNews - Android Application

Developer: M. Sai Ram
Roll No: 2211CS010379
Email: 2211cs010379@mallareddyuniversirty.ac.in

Project Overview

SpaceNews is a mobile application developed using Android (Java) that displays the latest news related to space missions, satellites, and space exploration. It uses the public API provided by Spaceflight News API to fetch real-time articles and display them dynamically in a user-friendly list format.

Features

Fetches live space news from https://api.spaceflightnewsapi.net/v4/articles/

Displays news articles with:

Image

Title

Tapping an article opens the full article in the browser.

Efficient and smooth UI using RecyclerView.

Image loading handled by Glide library for optimized performance.

XML Layout Files

activity_main.xml: Contains a TextView for the heading and a RecyclerView to display the news list.

item_news.xml: Custom layout for each news item with an ImageView and TextView.

Java Components

MainActivity.java: Initializes the RecyclerView, fetches news data using OkHttp, parses JSON, and updates the UI.

NewsAdapter.java: RecyclerView adapter to bind the news data with UI elements. Also handles click events to open news in browser.

NewsArticle.java: A simple model class to hold data fields: title, imageUrl, and articleUrl.

Libraries Used

OkHttp – For making network API calls.

Glide – For efficient image loading and caching.

How It Works

On app launch, a network request is made to the API.

JSON data is parsed and converted into a list of NewsArticle objects.

The RecyclerView is populated using NewsAdapter.

Clicking on an item opens the corresponding article in a web browser.

Sample UI

Main screen: List of articles with titles and thumbnails.

User Interaction: Tap to view full article in the browser.

Notes

Internet permission is required in the AndroidManifest to fetch live data.

Make sure to handle slow network conditions gracefully in production.
