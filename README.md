# NoSQL-Challenge
## Eat Safe, Love - Database Analysis
This repository contains code and instructions for evaluating the food hygiene ratings of various establishments in the United Kingdom. The goal is to assist the editors of the food magazine, Eat Safe, Love, in determining where to focus their future articles.

### Part 1: Database and Jupyter Notebook Set Up
To begin the analysis, follow the instructions below:

1.Import the data provided in the establishments.json file into a MongoDB database named uk_food and a collection named establishments.
2.Import the necessary libraries: PyMongo and Pretty Print (pprint).
3.Create an instance of the Mongo Client.
4.Confirm that you have successfully created the database and loaded the data by listing the databases in MongoDB and ensuring that uk_food is listed. Also, list the collections in the uk_food database and ensure that establishments is present. Retrieve and display one document from the establishments collection using the find_one method and pretty print it.

### Part 2: Update the Database
In this section, make the following modifications to the establishments collection:

1.Add a new document representing an exciting new halal restaurant called "Penang Flavours" in Greenwich, London. The restaurant has not yet been rated. Include all the required information, such as business name, type, address, postcode, and so on.
2.Find the BusinessTypeID for the business type "Restaurant/Cafe/Canteen" and return only the BusinessTypeID and BusinessType fields.
3.Update the document of the new restaurant, "Penang Flavours," with the BusinessTypeID found in the previous step.
4.Check how many documents contain the Dover Local Authority. Then, remove any establishments within the Dover Local Authority from the database.
5.Convert the latitude and longitude values stored as strings to decimal numbers using the update_many method.
6.Convert the RatingValue field from strings to integer numbers using the update_many method.

### Part 3: Exploratory Analysis
In this section, you will explore the dataset to answer specific questions posed by Eat Safe, Love:

1.Analyze the RatingValue field to determine the overall rating of establishments. Note that the field includes non-numeric values such as 'Pass', which should be treated as nulls during the analysis.
2.Consider the scores for Hygiene, Structural, and ConfidenceInManagement fields. Remember that higher values indicate worse performance in these areas.
3.By performing these exploratory analyses, you will help Eat Safe, Love find the locations they wish to visit and avoid.




