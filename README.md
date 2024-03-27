# nosql-challenge

Welcome to the NoSQL challenge! Within this assignment, I have delved into the evaluation of food hygiene ratings data provided by the UK Food Standards Agency. The primary objective of this project is to aid the editors of a food magazine, Eat Safe, Love, in analyzing the ratings data to facilitate their journalists and food critics in deciding where to focus future articles.

## Part 1: Database and Jupyter Notebook Setup

In this initial section, I've meticulously set up the NoSQL database and prepared the Jupyter Notebook for data analysis. Key steps undertaken include:

Data Import: I have seamlessly imported the data provided in the establishments.json file into a MongoDB database named uk_food, housing a collection named establishments. The import process was meticulously documented within the notebook.

Library Imports: The Jupyter Notebook was equipped with the necessary Python libraries, including PyMongo for database interaction and Pretty Print (pprint) for displaying data.

MongoDB Client: An instance of the MongoDB client was created to establish a connection to the database.

Data Validation: Verification of the successful creation of the database and the establishments collection was conducted by listing the available databases and collections. Furthermore, a sample document from the establishments collection was retrieved and displayed using find_one.

Variable Assignment: The establishments collection was assigned to a variable for further analysis.

## Part 2: Update the Database

This segment entailed making requested modifications to the database before proceeding with queries or analysis. The following changes were implemented to the establishments collection:

Addition of New Restaurant: A new halal restaurant was seamlessly added to Greenwich in accordance with the magazine's request.

BusinessTypeID Query: The BusinessTypeID for "Restaurant/Cafe/Canteen" was identified and returned alongside the BusinessType field.

Update New Restaurant: The information of the new restaurant was updated with the BusinessTypeID obtained in the previous step.

Deletion of Dover Establishments: Establishments within the Dover Local Authority were identified and removed from the database.

Data Type Conversion: Utilizing update_many, latitude and longitude were converted to decimal numbers, and RatingValue was converted to integer numbers.

## Part 3: Exploratory Analysis

In this section, an exploratory analysis of the dataset was conducted to address specific inquiries posed by Eat Safe, Love. Each question was tackled using MongoDB queries, and the results were presented systematically. The following questions were explored:

Establishments with Hygiene Score 20: Identification of establishments with a hygiene score equal to 20.

High-Rated Establishments in London: Discovery of establishments in London with a RatingValue greater than or equal to 4.

Top 5 Establishments with RatingValue 5: Determination of the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score and proximity to the new restaurant "Penang Flavours."

Local Authorities with Hygiene Score 0: Enumeration of establishments in each Local Authority area with a hygiene score of 0, sorted from highest to lowest, with the top ten local authority areas displayed.

## Conclusion:

This project exemplifies proficiency in working with NoSQL databases, conducting data analysis, and executing MongoDB queries to extract valuable insights from real-world data. It equips Eat Safe, Love with the requisite information to make informed decisions regarding future articles and restaurant recommendations, thus enhancing the exploration of food hygiene ratings. Enjoy delving into the world of food hygiene ratings!
