# Allergen-Friendly-Foods Repository Collection Policy

The Allergen-Friendly Food Repository is happy to take submissions to support the goals of our users. The more data we have, the safer you can eat!  If you would like to submit a data source or dataset to this repository, please work through the steps listed below. 

1. Think about the context.
This repository collects data about allergen presence and absence in food. Our level of specificity is individual items, not brands, so we cannot accept datasets indicating general allergen sensitivity over whole brands. 
Our data is focused on the top nine food allergies, which account for 90% of all food allergies:  milk, eggs, fish, shellfish, tree nuts, peanuts, sesame, gluten, and soybeans. As possible, we are also interested in collecting data about foods that are kosher, halal, vegan, vegetarian, and organic. We will accept data about any of these allergen/food needs as long as the other criteria in this collection policy are met. 
    Answer these questions:
    Is my data specific enough?
    Is my data about one of the allergens listed in 1b?

2. Think about the format.
-We cannot accept proprietary formats, or formats encrypted with password protection. File size should be reasonable. Machine- and human-readable CSV or XML spreadsheets are our preferred formats for data submissions (JSON and Markdown are acceptable). Metadata is important because it helps us organize the data and offer proper attribution. 

    If you have the technical knowledge, please make sure that your data: 
    a. Is in a machine-readable format. If you need to convert a PDF to a CSV file, Tabula is a helpful tool. 
    b. Adheres to the principles of tidy data, such as:
      -Avoids special characters such as commas in numerical values (ex: 1000✓ vs 1,000 ✗ or 99.9✓ vs 99.9% ✗).
      -Variables are columns and observations are rows.
      -Each cell contains only one value.
    c. Adheres to the format indicated in the Transformation and Quality documentation in this repository. Repository curators will review all submissions for accuracy and completeness.

    *If submitter performs data conversion, transformation, or translation, include the original source documents along with any new files.
    If you do not have the technical skills to assure that your data is 1) in the correct file format and 2) normalized according to tidy data and repository principles, you may submit other formats, and our data curators will evaluate and normalize the data as necessary.*

3. Think about metadata.
We need certain kinds of information about the creator and source of the submitted data to maintain our desired levels of accountability and data quality.  Please see our metadata profile for more information. 

4. Think about data integrity.
Checksums are lines of characters that check data for errors. We use these to ensure continuing data quality.  Repository managers will use gtkhash on a minimum yearly basis to check for data integrity. 

5. Preservation Policy
Certain actions must be undertaken to support the ongoing preservation of files in our repository. Our curators will take on the following actions:
a. Assigning permanent, persistent, unique identifiers
b. Assigning and maintaining preservation metadata
c. Regular assessment of need for transformation based on file format
d. Virus and file corruption checks


6. Ingestion and Curation
Once submitted, curators will assign a permanent, unique identifier to your dataset. This will be entered into the dataset’s metadata under “identifier.”
Curators will evaluate the license for public accessibility and the data dictionary for completeness, as relevant. 
Based on file format and transformation status at the time of submission, curators will perform any necessary data cleaning, adhering to the principles of tidy data. Curators will also assess the preservation needs and status of the file(s) and will undertake any necessary preservation actions.
Our curators will contact you if and when the submitted dataset is ready for publication.


