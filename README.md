# Coursera_Capstone
Capstone project

# Introduction
In this project we will try to find an optimal location for a restaurant. Specifically, this report will be targeted to stakeholders interested in opening an restaurant and school in New York, Unite States.Since there are lots of restaurants in New York we will try to detect locations that are not already crowded with restaurants. We choose some candidate location in Queens New York city. We want to get the cluster information about the Center Queens, so that we can analyze the cluster. Secondly, it is important that analyze the distribution of the restaurant type in each cluster. We will use our data science powers to generate a few most promising neighborhoods based on this criteria. Advantages of each area will then be clearly expressed and get the cluster character, so that best possible final location and restaurant type can be chosen by stakeholders.So, we want to explore the center candidate location that belongs to the restaurant type.

# Data
Based on definition of our problem, factors that will influence our decision are:
number of existing restaurants in the neighborhood (any type of restaurant) number of and distance to Italian restaurants in the neighborhood, if any distance of neighborhood from city center
number of school in the neighborhood (any type of school)
We decided to use regularly spaced grid of locations, centered around city center, to define our neighborhoods. This is our data flow:
Get the Queens geometry information
Calculate candidate geometry information, under the conditions, like ~6 km from Queens center, and each are has 600 meters each circle apart
Get the detailed information in each circle by using Foursquare API
