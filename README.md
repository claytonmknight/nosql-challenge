# nosql-challenge
 nosql-challenge
## UK Food Hygiene Ratings Database

This repository contains scripts and instructions for setting up a MongoDB database named `uk_food` and importing the UK Food Hygiene Ratings dataset into a collection named `establishments`. Additionally, it includes Jupyter Notebook files for conducting exploratory analysis on the dataset using Python and MongoDB.

### NoSQL_setup_starter.ipynb
#### Eat Safe, Love
##### Part 1: Database and Jupyter Notebook Set Up
- **Importing Data**: Import the data provided in the `establishments.json` file from your Terminal. Name the database `uk_food` and the collection `establishments`.
- **Database and Collection Setup**: Initialize a MongoDB client, create the `uk_food` database, and confirm its creation. Then, assign the `establishments` collection to a variable and review its content.

##### Part 2: Update the Database
1. **Add New Restaurant**: Add a new restaurant named "Penang Flavours" to the database. This halal restaurant is located in Greenwich and has not yet been rated.
2. **Find BusinessTypeID**: Find the `BusinessTypeID` for the "Restaurant/Cafe/Canteen" business type and return only the `BusinessTypeID` and `BusinessType` fields.
3. **Update New Restaurant**: Update the new restaurant "Penang Flavours" with the correct `BusinessTypeID`.
4. **Remove Establishments from Dover**: Check the number of documents containing the Dover Local Authority, remove any establishments within the Dover Local Authority from the database, and confirm deletion.
5. **Convert Data Types**: Convert string data types to decimal numbers for latitude and longitude fields and convert the `RatingValue` field to integer numbers.

### NoSQL_analysis_starter.ipynb
#### Eat Safe, Love
##### Part 3: Exploratory Analysis
1. **Identify Establishments with Hygiene Score of 20**: Find establishments with a hygiene score of 20 and display the number of documents and the first document in the results.
2. **Find Highly Rated Establishments in London**: Identify establishments in London with a `RatingValue` greater than or equal to 4 and display the number of documents and the first document in the results.
3. **Top 5 Establishments with RatingValue 5**: Find the top 5 establishments with a `RatingValue` of 5, sorted by the lowest hygiene score, nearest to the new restaurant added, "Penang Flavours".
4. **Establishments with Hygiene Score of 0**: Determine the number of establishments in each Local Authority area that have a hygiene score of 0 and display the results in a DataFrame.

Each analysis task includes instructions for setting up queries, executing them against the MongoDB database, and displaying the results using Pandas DataFrames.

Note: In NoSQL_setup_starter.ipynb, redundant command "# review the collections in our new database" was removed.