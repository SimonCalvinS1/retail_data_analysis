## Retail Data Analytics

## Project Status: Ongoing

### A data analytics project in Python analysing Indian retail data and creating meaningful business insights.

## Changes done to the dataset:
### Change 1:
- What I noticed: The columns (first record / header of each row) were not in snake case (Python's recommeded naming and coding convention).
- What I had to do: I formatted the columns to snake case using Python strip(), lower() and replace() methods

### Change 2:
- What I noticed: The uncleaned xlsx file contained 'Unknown City' value for a few records
- What I had to do: I assigned the city based on the state and region corresponding in the same record.

### Change 3:
- What I noticed: A few values in the 'sales_method' column with values like 'App', 'Wholesale', etc. contained semicolons at the end of a few of them (e.g. 'App;')
- What I had to do: I used the rstrip method to remove them.

### Change 4: 
- What I noticed: The xlsx file showed a mismatch where cities (e.g, Bangalore) were mapped to incorrect states and regions (e.g, Haryana, North) for almost all the records.
- What I had to do: I prioritised the "State" and "Region" column as the primary geographical units because states and regions are linked to each other (e.g. Haryana and North), while the "City" value (for the same record -> "Bengaluru").
- What I did later: I implemented a custom mapping function to reconstruct the City relationship using dictionaries and stored the cleaned data in a new xlsx file.
- What happened later: Improved data accuracy to 100%, eliminating "Geographical Hallucinations" in the dataset.

## Tech Stack: 
- Python
- VS Code (Jupyter Lab extension)
- Git and GitHub

## Dataset Link:
- [Kaggle Link](https://www.kaggle.com/datasets/vaibhav2549bhardwaj/retail-dataset)

## Python Modules (as of now):
- Pandas (with OpenPyXL)
- Matplotlib (pyplot and ticker)
- Seaborn
- NumPy
