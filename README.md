## Retail Data Analytics

## Project Status: Ongoing

### A data analytics project in Python analysing Indian retail data and creating meaningful business insights.

## Changes done to the dataset:
### Change 1: 
- What I noticed: The xlsx file showed a mismatch where cities (e.g, Bangalore) were mapped to incorrect states and regions (e.g, Haryana, North) for almost all the records.
- What I had to do: I prioritised the "State" and "Region" column as the primary geographical units because states and regions are linked to each other (e.g. Haryana and North), while the "City" value (for the same record -> "Bengaluru").
- What I did later: I implemented a custom mapping function to reconstruct the City relationship using dictionaries and stored the cleaned data in a new xlsx file.
- What happened later: Improved data accuracy to 100%, eliminating "Geographical Hallucinations" in the dataset.

## Tech Stack: 
- Python
- VS Code (Jupyter Lab extension)
- Git and GitHub

## Python Modules (as of now):
- Pandas (with OpenPyXL)
