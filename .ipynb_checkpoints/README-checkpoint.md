# Module 12: NoSQL Challenge - Eat Safe, Love Ratings Data Evaluation

## Project Overview

This project analyzes UK Food Standards Agency ratings data to support the "Eat Safe, Love" magazine in selecting establishments for future articles. The project involves setting up a MongoDB database, updating it with new data, and performing exploratory analysis to identify potential story angles.

## Data and Database

- **Data Source:** UK Food Standards Agency ratings data
- **Database:** MongoDB
- **Database Name:** `uk_food`
- **Collection Name:** `establishments`

## Project Structure

The project is divided into three main parts:

### Part 1: Database Setup

1. Import data into the MongoDB database.
2. Verify database and collection existence using `mongo.list_database_names()` and `db.list_collection_names()`.
3. Display a sample document using `find_one()`.
4. Assign variables to the collection and database for efficient querying.

### Part 2: Database Updates

1. Add a new restaurant ("Penang Flavours") if it doesn't exist.
2. Update the `BusinessTypeID` for the new restaurant.
3. Remove all establishments under the Dover Local Authority.
4. Convert data types for `latitude`, `longitude`, and `RatingValue` to numerical format.
5. Verify data type conversions.

### Part 3: Exploratory Analysis

1. Identify establishments with a hygiene score of 20.
2. Find London establishments with a `RatingValue` of 4 or higher.
3. Determine the top 5 establishments near "Penang Flavours" with a `RatingValue` of 5, sorted by the lowest hygiene score.
4. Calculate the number of establishments with a hygiene score of 0 per Local Authority area, sorted descendingly.

![Output Image](Output.png)

## Conclusion

The analysis provides valuable insights for the "Eat Safe, Love" magazine, highlighting establishments with excellent hygiene and those requiring improvement. This data-driven approach informs article selection and content.

## Bonus

- Deeper analysis of specific Local Authority areas.
- Correlation between hygiene score and other factors (e.g., business type, location).
- Visualization of data for better understanding and communication of findings.

## Hints

- **Data Cleaning:** Ensure data quality and consistency before analysis.
- **Performance Optimization:** Consider indexing for efficient querying, especially with large datasets.
- **Error Handling:** Implement error handling mechanisms for robust code.
- **Data Privacy:** Adhere to data protection regulations when handling personal information.

