# Allergen-Friendly-Foods Repository 

View the GitBook Here:  https://anabel-moreno-mendez-group.gitbook.io/allergen-friendly-foods-repository-documentation/

# Collection Policy

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


# Metadata Application Profile
Please refer to the Metadata Application Profile data dictionary. 
-NOTE-
This repository follows the AGRIS Metadata Application Profile from the UN’s FOA Agricultural Metadata Element Set (AgMES). It is otherwise known by its full title:  “The AGRIS Application Profile for the International Information System on Agricultural Sciences and Technology : Guidelines on Best Practices for Information Object Description.” AGRIS’ Best Practices combine the Dublin Core base metadata schema with fields tailored to description needs of the agricultural domain. We chose this set because our resources are all about food, particularly the ingredient/allergen content. AgMES is a widely used standard also about food production, and so it fit our needs.

Based on our user personas, one of the primary concerns is creator identity and trustworthiness. The stakes for incorrect information are high, and locating and verifying the author’s credentials is essential. Our chosen fields reflect those user needs. As our repository is not based on academic journal articles, we were able to eliminate metadata fields referring to journal citation.

In some instances, the AgMES profile needed to be supplemented with the more general fields represented in the Dublin Core. These choices are recommended by AGRIS, which contains a mixture of general Dublin Core fields and specifying AgMES fields.
To further investigate AgMES, you can follow this link: https://www.fao.org/3/ae909e/ae909e05.htm#P461_23843

-CONTROLLED VOCABULARIES-
Several fields require controlled vocabularies, which are listed in the metadata schema. These choices are all based on recommendations from AgMES, and provide greater standardization and searchability. This reasoning is also responsible for any indicated bounds on form, also listed in the schema. Depositors without the expertise to encode need not worry about doing so as our curators will review any submissions and transform the data accordingly.
     

-ENCODING-
Encoding should be done in XML. XML offers greater variety of data structures, security, and interoperability, even though it can be more complex to write.



# Transformation and Quality

1.DATA TRANSFER
Raw data may be uploaded to the Allergen-Friendly Foods Repository by submitting a pull request in the Github platform. This request will be reviewed by the repository managers who will perform initial authenticity checks and data quality assurance prior to approval. Users transferring data into the repository agree that the data will remain openly accessible, exploitable, editable, and shareable by anyone for any purpose. 


1.1 NAMING CONVENTIONS
The Naming Convention for deposited files follows the following format: SourceName_DocTitle_Allergen-focus_Semantic.Versioning.Here.csv
Semantic versioning explanation:
Versions will be tracked in a #.#.# format, starting with 1.0.0. When data is normalized, +1 to the third #. If data is updated to fix mistakes or add analysis, +1 to the second #. If new data is collected/produced from the original source, +1 to the first # and reset the following numbers to 0.


1.2 PROTECTIONS
Repository managers will rely on the built-in GitHub malware detector to prevent malicious viruses from being deposited. They will then manually review submitted data and cross-checking source data for accuracy.
No Personal Identifiable Information (PII) or unauthorized proprietary information will be collected or published within the depository. We ask that sensitive information be removed prior to submission of data. Any PII found in the submitted data will be removed prior to commitment of the pull request. Severe or repeat offenses may serve as grounds for rejection of current and/or future submission requests from the same user. 
“Unauthorized proprietary information” is defined as proprietary information, trade secrets, and any other confidential information that is unavailable to the general public through any other means. PII uses the standard definition. Users submitting data agree to release, indemnify, defend, and forever discharge repository owners from all liability, claims, demands, damages, costs, expenses, and causes of action due to death, injury, loss, or damage that result from failure to abide by these terms of use. 


1.3 IDENTIFIERS 
Repository reviewers will ensure a Github permalink is created for each unique data file that is committed to the repository prior to the data normalization process.In the event that PII is present in the original file, the PII will be removed and then the permalink will be created, with a comment noting the change.
Original documentation is kept to ensure appropriate data provenance, or to make sure everything is available for review. A separate file with an evolving identifier will be created for normalized data. Changes to this file will be automatically tracked by GitHub, however, repository managers will ensure that semantic versioning is applied to the title of the document with each new iteration. 


1.4 METADATA / ADDITIONAL DOCUMENTATION CREATION
Item-level metadata documentation will be created and tracked in a master sheet by the repository administrators upon review of the submitted items. Metadata not explicitly stated or provided may be inferred from the contents of submissions or found through further research, where possible. 
We request that the users submitting data review the metadata application profile and provide requested metadata where possible. Users possessing the technical expertise to do so are asked to adhere to “Tidy Data” principles and to provide data in preferred file formats (see 2.1 FILE FORMATS). When new documentation is created, the original file ought to be submitted with the new documentation, along with a brief data provenance statement. 


2.TRANSFORMATION
2.1  FILE FORMATS
Preferred file formats for data submissions include: CSV, XML, Markdowns, and JSON documents.  Please note PDFs and images may be converted using Tabula prior to submission.  Other file formats may be submitted for consideration. Original source documents should be submitted along with any new files when data conversions, transformations, or translations have been applied to originals prior to submission. 


2.2 APPROPRIATE DATA VALUE
Users normalizing data prior to submissions should refer to the Allergen Friendly Foods Data Dictionary for appropriate data values. A template for normalization of data is made available. 

# Potential Users

POTENTIAL USER COMMUNITY
Users of the Allergen-Friendly Food repository will range from parents wanting to know which foods their children can eat safely (seeking data) to companies looking to promote their allergen friendly foods to an audience that needs them (data depositors). Information seekers wish to find fully free resources with no strings attached. Depositors want to provide information in an easy-to-read and search place. Potential users are described below:


 **Information Seekers**
    _General public with dietary needs_,
        Individuals with multiple dietary restrictions,
        Parents of children with allergies,
        Teachers hosting a classroom party with food;
    _Health safety professionals,_
        Nutritionists assisting patients in meeting their dietary needs,
        Allergists providing food safety tips to patients,
        Government regulators conducting audits on allergen-free claims; 
    _Businesses and Entrepreneurs,_
        Consultants assessing the allergen-friendly food industry,
        Entrepreneurs exploring the possibility of starting an allergy-friendly food business,
        Influencers reaching an audience,
        Retailers looking to meet the needs of a growing customer-base,
        Both large corporations and small retailers may be interested in expanding the allergen-friendly foods available on their shelves.


**Information Depositors**
_Small businesses looking to promote their allergen-friendly products_,
    The allergen-friendly food industry is largely dominated by small businesses who may not have the marketing budget to promote their products across the country. Small businesses may choose to add their products to the allergen-friendly food repository;
_Nonprofits working to improve food labeling_,
    Many nonprofits focus on increasing awareness of different allergens or non-allergen based food needs. Including their pre-certified products in a repository increases awareness of the certification and thus potentially support and buy-in from major retailers; 
_General public with allergy concerns_,    
    Individuals who find and share information with their communities.

SAMPLE DATASET OVERVIEW:
Several sources are openly available for inclusion in this repository (after normalization). Snacksafely.com provides a catalog of foods that are free from various allergens, including: Peanuts and Treenuts, Milk (Dairy), Gluten, and Sesame. The Snack Safely guides for the allergens listed here are available for free as PDFs, but a paid subscription allows the user to have additional database features which allow for a personalized list of allergen-safe foods.
For example, the “Safe Snack Guide: Peanut and Tree Nut Free Edition” is a PDF that provides a list of foods that are peanut-free and treenut-free, meaning the information seeker can select any item on the list without being concerned about those allergens. Within the guide, you also will see the occasional “tag” indicating that a food is also free from one or multiple other allergens. This PDF can be accessed here: https://snacksafely.com/peanut-treenut-free/.
Information provided includes:
    *Manufacturer / Brand information,
    *Product food type,
    *Product name,
    *Product description,
    *Product certifications,
    *Additional Excluded Allergen information (allergen “tag”),
    *Permanent identifier /URL,
    *Last Modified Date,
    *Licensing / Copyright information


**USER STORY**
**Information Seeker, General Public**
Here, we highlight the user story of Rima Srivastav (she/her), an elementary school teacher seeking information to ensure her classroom party is safe and inclusive for all.
    Rima teaches second grade at a public school, and she wants to throw a party to celebrate the great work her students did on a recent project. Four of her students are deathly allergic to even trace amounts of peanuts and tree nuts. One student can’t eat soy and another student has celiac and can’t eat gluten. She wants to be able to find fun, tasty snacks that are free from all the allergens and restrictions that affect her students.
    Although there are various guides and lists available across the internet, she has found it difficult to find an inclusive allergen-friendly foods database that does not require a paid subscription. She wishes to have all the allergen information for various products in one place, so she can shop easily, rather than having to scour over the ingredient list on each individual snack she sees in the store. Even doing her research in advance, she has realized that it is not always easy to find which stores will carry the food items she is interested in purchasing. Rima is wondering if it is possible for her to purchase the special snacks in bulk from the manufacturer, so it can be shipped directly to her classroom. She is feeling a bit overwhelmed and this would make everything far easier. 
    Members of the general public are typically users who seek certified allergen -friendly food information for personal health reasons. They or someone they care about have one or multiple allergies and wish to safely enjoy pre-packaged foods. They don’t want to do extensive research to be able to find this information.They want an easily searchable collection that provides this information in one place.


ASSESSMENT OF NEED  
As noted, individuals are often allergic to multiple things, and it can be quite tedious to cross check multiple lists to find appropriate snack foods that satisfy all dietary restrictions. Although the guide is extensive and useful, normalizing the data before depositing it in our repository is essential. 
For Rima, this dataset includes indications on all relevant allergens (presence and absence), but the way it is organized would make it difficult for Rima to choose products based on multiple allergens at once. CTRL+F search can only really search one term at once, and she has three required allergens she needs to search for. Rima’s most-needed features are allergen filters and a free, easily accessible interface for her to use them. At this time, the guides do not provide this (for free), however, once the list is cleaned and put into an easy-to-read spreadsheet, she will be able to access it on GitHub and filter for all relevant allergens more easily. This will result in a complete list of foods that fill her needs. 
She also would love to see permanent identifiers in for the original product manufacturer site included -this will allow her to explore different purchasing options. If she cannot find quite what she is looking for, the repository will allow her to explore different datasets
