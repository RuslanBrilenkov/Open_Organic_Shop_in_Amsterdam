# Data Science Capstone: _Open Organic Store_

## A step-by-step Exploratory Data Analysis project 
From a business problem to my solution and implementation, using Foursquare API, Beautiful soup, Requests, Pandas, and Folium.

# Introduction & Summary
I created this project in order to complete a Capstone Project to finish the "Applied Data Science Capstone" and obtain IBM Professional Data Science Certificate. 

I came up with this business idea because it resonates with me as a promoter of a healthy lifestyle. So I would like to share it with you step-by-step.

## Motivation

Nowadays, more and more people are "going green", i.e., moving towards a healthier lifestyle - not only by increasing daily movements but also by choosing the healthier products (wild-caught, locally-produced, bio+, organic  -  you name it).

The underlying reason may be an increasing knowledge about nutrition and health, and/or increasing availability of clean sources of food. In both cases, I totally support this movement. As the number of "health-is-priority" people grows, so the number of organic stores as well. 

### I want to create some value for others, so why not try to catch up with this trend by opening a new Organic Shop!

In my view, a good business is one oriented towards values, growth, and a vision for the future. Building an organic store has the potential to bring value to our customers, make profit, and increase it in the future as more and more people will be joining this healthy movement.

*In my view, a good business is one oriented towards values, growth, and a vision for the future. Building an organic store has the potential to bring value to our customers, make profit, and increase it in the future as more and more people will be joining this healthy movement.*

**In this project, I will be exploring Amsterdam neighborhoods to find out the best place to open a new organic shop.**


This file consists of the following sections:
• ***Business Problem*** (Introducing a business idea and my approach to solving it);
• ***Data Analysis*** (Describing the relevant data and the process of its acquisition);
• ***Results and Conclusions*** (Drawing conclusions from the findings and scope for future work).



### Data Analysis
In this section, I perform the following actions:
1. obtain the data from open sources on the Internet (by web scraping);
2. create and pre-processing (cleaning) the data sets;
3. combine various data sets and visually exploring the possible answers to the problem;
3. outline possible future steps to explore this topic even deeper.

### A Business Problem
Here, I emphasize my motivation, reasonings, and open questions which I am addressing project. 

Namely, by asking myself these three questions: 
**Why** I decided to do it?

**What** I am going to do?

**How** I am planning to handle it?



## My Toolbox

These are the tools I will be using in this project:

• Pandas. If you are working with data sets, this library is a must. It has many functions for data importing, manipulation and analysis. [official page](https://pandas.pydata.org/);

• Beautiful Soup. This Python package is used for parsing HTML and XML documents. Basically, it is useful for web scraping. [official page](https://www.crummy.com/software/BeautifulSoup/);

• NumPy. If you are working with arrays, dictionaries, functions, data types, and images, you need to know NumPy. [official page](https://numpy.org/);

GeoPy. This Python package is used to locate the coordinates of addresses, cities, countries, and landmarks across the globe using third-party geocoders and other data sources. [official page](https://geopy.readthedocs.io/en/stable/);

• Tqdm (optional). This library is used to make the loops show a smart progress meter/bar. This is optional but I found it nice to track the progress of the web scraping. [documentation](https://tqdm.github.io/);

• Folium. A Python library for map rendering that makes it easy to visualize data on an interactive Leaflet map. [documentation](https://pypi.org/project/folium/0.1.5/).


# Preliminary Visualization

According to statistics, approximately 65 percent of the population is visual learners!

So, let us visualize the problem. I want to see the map of Amsterdam with its neighborhoods.

For this, we need to know the postalcodes (zip) of each neighborhood, and its corresponding latitude and longitude values.

To accomplish this task, I perform the following steps:

1. Scrape the web for postal codes using ***beautiful soup*** and ***requests***;
2. Find corresponding coordinates (latitude and longitude) with ***geopy***;
3. Combine all the data into a ***pandas*** Data Frame;
4.Visualize the neighborhoods with ***folium***.


As a result, I create a beautiful map of Amsterdam neighborhoods, shown below:

![Amsterdam neighborhoods](https://miro.medium.com/max/1400/1*6UyLdmNE26JHS3E4SLfWEw.png)

Figure above. Amsterdam neighborhood map.

# Exploring Cenus Data

My ultimate goal is to find the best, most profitable place in the Amsterdam neighborhood for opening an Organic Store. 

I assume that the profit/income is proportional to the number of people around a store. 

So, I explore the open archives from the government website to find out the density of people around Amsterdam. 

The result is shown in the following heat density map:

![heat density map of Amsterdam neighbors](https://miro.medium.com/max/1400/1*3qcKky72S-qpuIOcWNhJTA.png)

Figure above. Heat/density Map of the Amsterdam neighborhoods.


# Looking for competitors

To become a profitable shop, we need to have not only enough people around but they have to come and buy something in our shop, right?

With this idea, I look into the density of competitors around Amsterdam. 

The result is shown below:

![Organic shop competitors in Amsterdam](https://miro.medium.com/max/1400/1*ahrO-mBmCTIQtIiOTPPVhQ.png)

Figure above. Visualizing Organic Shops of Amsterdam together with the population density.

# Combining all in one visual!

In order to complete our Exploratory Data Analysis for finding the best, most profitable place in Amsterdam, I combine all of the above-mentioned information in one great leaflet map:

![All-in-one visual: popultaion density, competitors, Amsterdam neighborhoods](https://miro.medium.com/max/1400/1*h5iPtj7m9cnLPo5OpDZC-w.png)

Map of Amsterdam (above). Filled circles represent an area of 1 km around every organic shop (our competitors) with the star pins representing the competitors themselves. The red circles show the neighborhoods. Circle size is proportional to the population density in this neighborhood.

# Conclusions

Based on the above-shown figure, I can suggest that the best places to open a new Organic Shop would be the neighborhoods of:

• ***Osdorp-East, Osdorp Central North, Don Bosco*** (Western far part of Amsterdam);

• ***Kolenkit, Kolenkitbuurt North, Kolenkitbuurt South*** (Western close part of Amsterdam);

• Around ***Valkenburg*** (near Central Station).


Like anything else, opening a new shop involves certain risks. However, this preliminary conclusion is backed by publically available data. 

As the preliminary, conclusion I would recommend opening a new Organic Shop in one of the above-mentioned locations.

The further in-depth analysis on a lrager dataset is neccessary to proceed with opening a shop. However, these are the places I would start to explore at first.

Even without utilizing every neighborhood in Amsterdam, we could draw a fairly full picture of its population density and the presence of other organic shops. Using visual exploration, I analyzed the above-mentioned distributions to get the best 3 areas for opening a new organic shop.

With this, I conclude my analysis.


# Contacts


If you would like to connect, have any questions, suggestions or found any error, please contact me. Let us connect!

[LinkedIn](https://www.linkedin.com/in/ruslan-brilenkov/)

[Original article](https://medium.datadriveninvestor.com/my-data-science-project-open-organic-shop-in-amsterdam-daf3d08ae16f)
