# Course 03 - Prepare Data For Exploration
# Module 1
## Data exploration
### Data collection considerations
- How the data will be colected
  Decide if you will collect the data using your own resources or receive (and possibly purchase it) from another party. Data that you collect yourself is called first-party data.
- Data sources
  - First-party data: data collected by an individual or group using their own resources. Tipically the preferred method because you know exactly where it came from.
  - Second-party data: data collected by a group directly from its audience and then sold. his data didn't start with you, but it's still reliable because it came from a source that has experience with traffic analysis.
  - Third-party data: data collected from outside sources who did not collect it directly. This data might have come from a number of different sources before you investigated it. It might not be as reliable, but that doesn't mean it can't be useful. You'll just want to make sure you check it for accuracy, bias, and credibility. 
- Decide what data to use
  Datasets can show a lot of interesting information. But be sure to choose data that can actually help solve your problem question. For example, if you are analyzing trends over time, make sure you use time series data — in other words, data that includes dates.
- How much data to collect
  - Population: all possible data values in a dataset. If you're analyzing data about car traffic in a city, your population would be all the cars in that area. But collecting data from the entire population can be pretty challenging. That's why a sample can be useful. 
  - Sample: part of a population that is representative of the population. You might collect a data sample about one spot in the city and analyze the traffic there, or you might pull a random sample from all existing data in the population. How you choose your sample will depend on your project. 

  If you are collecting your own data, make reasonable decisions about sample size. A random sample from existing data might be fine for some projects. Other projects might need more strategic data collection to focus on certain criteria. Each project has its own needs. 
- Select the right data type

- Determine the time frame for data collection
  If you are collecting your own data, decide how long you will need to collect it, especially if you are tracking trends over a long period of time. If you need an immediate answer, you might not have time to collect new data. In this case, you would need to use historical data that already exists. 

  ![alt text](image.png)

### Data formats
- Quantitative data:
  - Discrete data: data that is counted and has a limited number of values. Example is a movie's budget and box office. They can be counted and have a limited number of values. For example, the amount of money a movie makes can only be represented with exactly two digits after the decimal to represent cents. There can't be anything between one and two cents. Discrete data isn't limited to dollar amounts. Examples of other discrete data are stars and points. When partial measurements (half-stars or quarter-points) aren't allowed, the data is discrete. If you don't accept anything other than full stars or points, the data is considered discrete.
  - Continuous data: data that can be measured using a timer, and its value can be shown as a decimal with several places. Examples are movie run time (110.0563 minutes)
- Qualitative data:
  - Nominal data: a type of qualitative data that's categorized without a set order. In other words, this data doesn't have a sequence. Examples are questions like "Have you watched Star Wars?". Answers could be "Yes", "No", "Not sure". These choices don't have a particular order.
  - Ordinal data: a type of qualitative data with a set order or scale. If you asked a group of people to rank a movie from 1 to 5, some might rank it as a 2, others a 4, and so on. These rankings are in order of how much each person liked the movie.
- Internal data: data that lives within a company's own systems. For example, if a movie studio had compiled all of the data in the spreadsheet using only their own collection methods, then it would be their internal data
- External data: data that lives and is generated outside of an organization. External data becomes particularly valuable when your analysis depends on as many sources as possible. A great thing about this data is that it's structured.
- Structured data: data that's organized in a certain format, such as rows and columns. Spreadsheets and relational databases are two examples of software that can store data in a structured way. 
- Unstructured data: data that is not organized in any easily identifiable manner. Audio and video files are examples of unstructured data because there's no clear way to identify or organize their content. Unstructured data might have internal structure, but the data doesn't fit neatly in rows and columns like structured data.


### Primary versus secondary data
| Data format classification | Definition                                      | Examples                                                    |
|---------------------------|-------------------------------------------------|-------------------------------------------------------------|
| Primary data              | Collected by a researcher from first-hand sources | Data from an interview you conducted - Data from a survey returned from 20 participants - Data from questionnaires you got back from a group of workers |
| Secondary data            | Gathered by other people or from other research  | Data you bought from a local data analytics firm’s customer profiles - Demographic data collected by a university - Census data gathered by the federal government |

### Internal versus external data
| Data format classification | Definition                                      | Examples                                                    |
|---------------------------|-------------------------------------------------|-------------------------------------------------------------|
| Internal data              | Data that is stored inside a company’s own systems | Wages of employees across different business units tracked by HR - Sales data by store location - Product inventory levels across distribution centers |
| External data            | Data that is stored outside of a company or organization  | National average wages for the various positions throughout your organization - Credit reports for customers of an auto dealership |

### Continuous versus discrete data
| Data format classification | Definition                                      | Examples                                                    |
|---------------------------|-------------------------------------------------|-------------------------------------------------------------|
| Continuous data           | Data that is measured and can have almost any numeric value | Height of kids in third grade classes (52.5 inches, 65.7 inches), Runtime markers in a video, Temperature |
| Discrete data             | Data that is counted and has a limited number of values | Number of people who visit a hospital on a daily basis (10, 20, 200), Maximum capacity allowed in a room, Tickets sold in the current month |

### Qualitative versus quantitative data
| Data format classification | Definition                                      | Examples                                                    |
|---------------------------|-------------------------------------------------|-------------------------------------------------------------|
| Qualitative               | A subjective and explanatory measure of a quality or characteristic | Favorite exercise activity - Brand with best customer service - Fashion preferences of young adults |
| Quantitative              | A specific and objective measure, such as a number, quantity, or range | Percentage of board certified doctors who are women - Population size of elephants in Africa - Distance from Earth to Mars at a particular time |

### Nominal versus ordinal data
| Data format classification | Definition                                      | Examples                                                    |
|---------------------------|-------------------------------------------------|-------------------------------------------------------------|
| Nominal                   | A type of qualitative data that is categorized without a set order | First time customer, returning customer, regular customer - New job applicant, existing applicant, internal applicant - New listing, reduced price listing, foreclosure |
| Ordinal                   | A type of qualitative data with a set order or scale | Movie ratings (number of stars: 1 star, 2 stars, 3 stars) - Ranked-choice voting selections (1st, 2nd, 3rd) - Satisfaction level measured in a survey (satisfied, neutral, dissatisfied) |

### Structured versus unstructured data
| Data format classification | Definition                                      | Examples                                                    |
|---------------------------|-------------------------------------------------|-------------------------------------------------------------|
| Structured data           | Data organized in a certain format, like rows and columns | Expense reports, Tax returns, Store inventory |
| Unstructured data         | Data that cannot be stored as columns and rows in a relational database | Social media posts, Emails, Videos |

Structured data works nicely within a <strong>data model</strong>, which is a model that is used for organizing data elements and how they relate to one another. <strong>Data elements</strong> are pieces of information, such as people's names, account numbers, and addresses. Data models help to keep data consistent and provide a map of how data is organized. 

### The effects of different structures
Data is everywhere and it can be stored in lots of ways. Two general categories of data are: 
- Structured data: Organized in a certain format, such as rows and columns.
- Unstructured data: Not organized in any easy-to-identify way.
For example, when you rate your favorite restaurant online, you're creating structured data. But when you use Google Earth to check out a satellite image of a restaurant location, you're using unstructured data. 



### The fairness issue

The lack of structure makes unstructured data difficult to search, manage, and analyze. But recent advancements in artificial intelligence and machine learning algorithms are beginning to change that. Now, the new challenge facing data scientists is making sure these tools are inclusive and unbiased. Otherwise, certain elements of a dataset will be more heavily weighted and/or represented than others. And as you're learning, an unfair dataset does not accurately represent the population, causing skewed outcomes, low accuracy levels, and unreliable analysis.

## Data modeling levels and techniques
This reading introduces you to data modeling and different types of data models. Data models help keep data consistent and enable people to map out how data is organized.
### What is data modeling?
Data modeling is the process of creating diagrams that visually represent how data is organized and structured.  These visual representations are called data models. You can think of data modeling as a blueprint of a house. At any point, there might be electricians, carpenters, and plumbers using that blueprint. Each one of these builders has a different relationship to the blueprint, but they all need it to understand the overall structure of the house. Data models are similar; different users might have different data needs, but the data model gives them an understanding of the structure as a whole. 

### Levels of data modeling

Each level of data modeling has a different level of detail. 

![alt text](image-1.png)

- Conceptual data modeling gives a high-level view of the data structure, such as how data interacts across an organization. For example, a conceptual data model may be used to define the business requirements for a new database. A conceptual data model doesn't contain technical details. 
- Logical data modeling focuses on the technical details of a database such as relationships, attributes, and entities. For example, a logical data model defines how individual records are uniquely identified in a database. But it doesn't spell out actual names of database tables. That's the job of a physical data model.
- Physical data modeling depicts how a database operates. A physical data model defines all entities and attributes used; for example, it includes table names, column names, and data types for the database.

### Data-modeling techniques

There are a lot of approaches when it comes to developing data models, but two common methods are the Entity Relationship Diagram (ERD) and the Unified Modeling Language (UML) diagram. ERDs are a visual way to understand the relationship between entities in the data model. UML diagrams are very detailed diagrams that describe the structure of a system by showing the system's entities, attributes, operations, and their relationships. As a junior data analyst, you will need to understand that there are different data modeling techniques, but in practice, you will probably be using your organization’s existing technique. 

### Data analysis and data modeling

Data modeling can help you explore the high-level details of your data and how it is related across the organization’s information systems. Data modeling sometimes requires data analysis to understand how the data is put together; that way, you know how to map the data. And finally, data models make it easier for everyone in your organization to understand and collaborate with you on your data. 

## Explore data types, fields and values
### Data type

A specific kind of data attribute that tells what kind of value the data is. In other words, a data type tells you what kind of data you're working with. Data types can be different depending on the query language you're using. For example, SQL allows for different data types depending on which database you're using. A data type in a spreadsheet can be one of three things: a number, a text or string, or a Boolean.

## Wide and long data
- With wide data, every data subject has a single row with multiple columns to hold the values of various attributes of the subject. In a wide format, data is spread across columns, with each observation in a single row. This is common for cross-sectional analysis.

| ID | Name  | Score_2023 | Score_2024 | Score_2025 |
|----|-------|------------|------------|------------|
| 1  | Alice | 85         | 90         | 88         |
| 2  | Bob   | 78         | 82         | 85         |
| 3  | Carol | 92         | 94         | 91         |

Key characteristics:
  1. Each year (2023, 2024, 2025) is in a separate column.
  1. Fewer rows, more columns.
  1. Easier for reading but harder for some types of analysis.

- Long data is data in which each row is one time point per subject, so each subject will have data in multiple rows. In a long format, data is stacked with repeated observations across rows for different time points.

| ID | Name  | Year | Score |
|----|-------|------|-------|
| 1  | Alice | 2023 | 85    |
| 1  | Alice | 2024 | 90    |
| 1  | Alice | 2025 | 88    |
| 2  | Bob   | 2023 | 78    |
| 2  | Bob   | 2024 | 82    |
| 2  | Bob   | 2025 | 85    |
| 3  | Carol | 2023 | 92    |
| 3  | Carol | 2024 | 94    |
| 3  | Carol | 2025 | 91    |

Key characteristics:

1. Each year appears as a separate row.
1. More rows, fewer columns.
1. Easier for statistical analysis and visualization (e.g., time-series analysis).

## Transforming data
Data transformation is the process of changing the data’s format, structure, or values. Data transformation usually involves:

- Adding, copying, or replicating data 
- Deleting fields or records 
- Standardizing the names of variables
- Renaming, moving, or combining columns in a database
- Joining one set of data with another
- Saving a file in a different format. For example, saving a spreadsheet as a comma separated values (.csv) file.

### Why transform data?
Goals for data transformation might be: 

- Data organization: better organized data is easier to use
- Data compatibility: different applications or systems can then use the same data
- Data migration: data with matching formats can be moved from one system to another
- Data merging: data with the same organization can be merged together
- Data enhancement: data can be displayed with more detailed fields 
- Data comparison: apples-to-apples comparisons of the data can then be made 

### Data transformation example: data merging
Mario is a plumber who owns a plumbing company. After years in the business, he buys another plumbing company. Mario wants to merge the customer information from his newly acquired company with his own, but the other company uses a different database. So, Mario needs to make the data compatible. To do this, he has to transform the format of the acquired company’s data. Then, he must remove duplicate rows for customers they had in common.

### Data transformation example: data organization (long to wide)
To make it easier to create charts, you may also need to transform long data to wide data. Consider the following example of transforming stock prices (collected as long data) to wide data. 

Long data is data where each row contains a single data point for a particular item. In the long data example below, individual stock prices (data points) have been collected for Apple (AAPL), Amazon (AMZN), and Google (GOOGL) (particular items) on the given dates.

![alt text](image-2.png)

Wide data is data where each row contains multiple data points for the particular items identified in the columns. 

![alt text](image-3.png)

With data transformed to wide data, you can create a chart comparing how each company's stock changed over the same period of time.  

You might notice that all the data included in the long format is also in the wide format. But wide data is easier to read and understand. That is why data analysts typically transform long data to wide data more often than they transform wide data to long data. The following table summarizes when each format is preferred:

| Wide data is preferred when  | Long data is preferred when |
| ---------------------------- | --------------------------- |
| Creating tables and charts with a few variables about each subject | Storing a lot of variables about each subject. For example, 60 years worth of interest rates for each bank |
| Comparing straightforward line graphs | Performing advanced statistical analysis or graphing |

## Terms and definitions for Course 3, Module 1
Agenda: A list of scheduled appointments

Audio file: Digitized audio storage usually in an MP3, AAC, or other compressed format

Boolean data: A data type with only two possible values, usually true or false

Continuous data: Data that is measured and can have almost any numeric value

Cookie: A small file stored on a computer that contains information about its users

Data element: A piece of information in a dataset 

Data model: A tool for organizing data elements and how they relate to one another

Digital photo: An electronic or computer-based image usually in BMP or JPG format

Discrete data: Data that is counted and has a limited number of values

External data: Data that lives, and is generated, outside of an organization

Field: A single piece of information from a row or column of a spreadsheet; in a data table, typically a column in the table

First-party data: Data collected by an individual or group using their own resources

Long data: A dataset in which each row is one time point per subject, so each subject has data in multiple rows

Nominal data: A type of qualitative data that is categorized without a set order

Ordinal data: Qualitative data with a set order or scale

Ownership: The aspect of data ethics that presumes individuals own the raw data they provide and have primary control over its usage, processing, and sharing 

Pixel: In digital imaging, a small area of illumination on a display screen that, when combined with other adjacent areas, forms a digital image 

Population: In data analytics, all possible data values in a dataset

Record: A collection of related data in a data table, usually synonymous with row

Sample: In data analytics, a segment of a population that is representative of the entire population

Second-party data: Data collected by a group directly from its audience and then sold 

Social media: Websites and applications through which users create and share content or participate in social networking

String data type: A sequence of characters and punctuation that contains textual information (Refer to Text data type)

Structured data: Data organized in a certain format such as rows and columns

Text data type: A sequence of characters and punctuation that contains textual information (also called string data type)

United States Census Bureau: An agency in the U.S. Department of Commerce that serves as the nation’s leading provider of quality data about its people and economy

Unstructured data: Data that is not organized in any easily identifiable manner

Video file: A collection of images, audio files, and other data usually encoded in a compressed format such as MP4, MV4, MOV, AVI, or FLV

Wide data: A dataset in which every data subject has a single row with multiple columns to hold the values of various attributes of the subject



# Module 2 - Unbiased and objective data
## Unbiased and objective data
Bias: a preference in favor of or against a person, group of people, or thing. It can be conscious or subconscious. The good news is once we know and accept that we have bias, we can start to recognize our own patterns of thinking and learn how to manage it

Data bias: a type of error that systematically skews results in a certain direction.

- Sampling bias: when a sample isn't representative of the population as a whole. You can avoid this by making sure the sample is chosen at random, so that all parts of the population have an equal chance of being included. Unbiased sampling results in a sample that's representative of the population being measured. Another great way to discover if you're working with unbiased data is to bring the results to life with visualizations.

- Observer bias: sometimes referred to as experimenter bias or research bias. Basically, it's the tendency for different people to observe things differently. One time observer bias might happen is during manual blood pressure readings. Because the pressure meter is so sensitive, health care workers often get pretty different results. Usually, they'll just round up to the nearest whole number to compensate for the margin of error. But if doctors consistently round up, or down the blood pressure readings on their patients, health conditions may be missed, and any studies involving their patients wouldn't have precise, and accurate data.

- Interpretation bias: the tendency to always interpret ambiguous situations in a positive, or negative way. Let's say you're having lunch with a colleague, when you get a voicemail from your boss, asking you to call her back. You put the phone down in a huff, certain that she's angry, and you're on the hot seat for something. But when you play the message for your friend, he doesn't hear anger at all, he actually thinks she sounds calm and straightforward. Interpretation bias, can lead to two people seeing or hearing the exact same thing, and interpreting it in a variety of different ways, because they have different backgrounds, and experiences. Your history with your boss made you interpret the call one way, while your friend interpreted it in another way, because they're strangers. Add these interpretations to a data analysis, and you can get bias results.

- Confirmation bias: the tendency to search for, or interpret information in a way that confirms preexisting beliefs. Someone might be so eager to confirm a gut feeling, that they only notice things that support it, ignoring all other signals. This happens all the time in everyday life. We might get our news from a certain website because the writers share our beliefs, or we socialize with people because we know that they hold similar views.

## Achieve data credibility
- ROCCC: Process to identify good data sources.

| Criteria | Definition |
|----------|------------|
| Reliable | Accurate, complete and unbiased information that's been vetted and proven fit for use. |
| Original | To make sure you're dealing with good data, be sure to validate it with the original source. |
| Comprehensive | The best data sources contain all critical information needed to answer the question or find the solution. |
| Current | The usefulness of data decreases as time passes. The best data sources are current and relevant to the task at hand. |
| Cited | Citing makes the information you're providing more credible. When you're choosing a data source, think about three things. Who created the data set? Is it part of a credible organization? When was the data last refreshed?|

 If you have original data from a reliable organization and it's comprehensive, current, and cited, it ROCCCs! There's lots of places that are known for having good data. Your best bet is to go with the vetted public data sets, academic papers, financial data, and governmental agency data.

## Data ethics and privacy

We all have our own personal biases, not to mention subconscious biases that make ethics even more difficult to navigate. That's why we have data ethics.

Ethics refers to well-founded standards of right and wrong that prescribe what humans ought to do, usually in terms of rights, obligations, benefits to society, fairness or specific virtues.

Data ethics refers to well-founded standards of right and wrong that dictate how data is collected, shared, and used. Data ethics tries to get to the root of the accountability companies have in protecting and responsibly using the data they collect. Here are some of the different aspects of data ethics:
- Ownership: who owns the data? It isn't the organization that invested time and money collecting, storing, processing, and analyzing it. It's individuals who own the raw data they provide, and they have primary control over its usage, how it's processed and how it's shared.
- Transaction transparency: all data processing activities and algorithms should be completely explainable and understood by the individual who provides their data. 
- Consent: an individual's right to know explicit details about how and why their data will be used before agreeing to provide it. They should know answers to questions like why is the data being collected? How will it be used? How long will it be stored?
- Currency: individuals should be aware of financial transactions resulting from the use of their personal data and the scale of these transactions. If your data is helping to fund a company's efforts, you should know what those efforts are all about and be given the opportunity to opt out.
- Privacy: preserving a data subject's information and activity any time a data transaction occurs. This is sometimes called information privacy or data protection. It's all about access, use, and collection of data. It also covers a person's legal right to their data
- Openness: free access, usage, and sharing of data. 

### Data anonymization
Personally identifiable information, or PII, is information that can be used by itself or with other data to track down a person's identity. 

Data anonymization is the process of protecting people's private or sensitive data by eliminating that kind of information. Typically, data anonymization involves blanking, hashing, or masking personal information, often by using fixed-length codes to represent data columns, or hiding data with altered values. 

#### What types of data should be anonymized?
Healthcare and financial data are two of the most sensitive types of data. These industries rely a lot on data anonymization techniques. After all, the stakes are very high. That’s why data in these two industries usually goes through de-identification, which is a process used to wipe data clean of all personally identifying information.

Data anonymization is used in just about every industry. That is why it is so important for data analysts to understand the basics. Here is a list of data that is often anonymized:

- Telephone numbers
- Names
- License plates and license numbers
- Social security numbers
- IP addresses
- Medical records
- Email addresses
- Photographs
- Account numbers

For some people, it just makes sense that this type of data should be anonymized. For others, we have to be very specific about what needs to be anonymized. Imagine a world where we all had access to each other’s addresses, account numbers, and other identifiable information. That would invade a lot of people’s privacy and make the world less safe. 


## Undestand open data
### Openness
When referring to data, openness refers to free access, usage and sharing of data.

- Be available and accessible to the public as a complete dataset: Open data must be available as a whole, preferably by downloading over the Internet in a convenient and modifiable form.
- Be provided under terms that allow it to be reused and redistributed: Open data must be provided under terms that allow reuse and redistribution including the ability to use it with other datasets.
- Allow universal participation so that anyone can use, reuse, and redistribute the data: Everyone must be able to use, reuse, and redistribute the data. There shouldn't be any discrimination against fields, persons, or groups. No one can place restrictions on the data like making it only available for use in a specific industry. 

One of the biggest benefits of open data is that credible databases can be used more widely. More importantly, all of that good data can be leveraged, shared, and combined with other data. 

A whole lot of resources are needed to make the technological shift to open data. Interoperability is key to open data's success. Interoperability is the ability of data systems and services to openly connect and share data. For example, data interoperability is important for health care information systems where multiple organizations such as hospitals, clinics, pharmacies, and laboratories need to access and share data to ensure patients get the care that they need. This is why your doctor is able to send your prescription directly to your pharmacy to fill. They have compatible databases that allow them to share information. But this kind of interoperability requires a lot of cooperation.

## Terms and definitions for Course 3, Module 2
Bad data source: A data source that is not reliable, original, comprehensive, current, and cited (ROCCC) 

Bias: A conscious or subconscious preference in favor of or against a person, group of people, or thing

Confirmation bias: The tendency to search for or interpret information in a way that confirms pre-existing beliefs

Consent: The aspect of data ethics that presumes an individual’s right to know how and why their personal data will be used before agreeing to provide it

Cookie: A small file stored on a computer that contains information about its users

Currency: The aspect of data ethics that presumes individuals should be aware of financial transactions resulting from the use of their personal data and the scale of those transactions

Data anonymization: The process of protecting people's private or sensitive data by eliminating identifying information

Data bias: When a preference in favor of or against a person, group of people, or thing systematically skews data analysis results in a certain direction

Data ethics: Well-founded standards of right and wrong that dictate how data is collected, shared, and used

Data interoperability: A key factor leading to the successful use of open data among companies and governments

Data privacy: Preserving a data subject’s information any time a data transaction occurs

Ethics: Well-founded standards of right and wrong that prescribe what humans ought to do, usually in terms of rights, obligations, benefits to society, fairness, or specific virtues

Experimenter bias: The tendency for different people to observe things differently (also called observer bias)

Fairness: A quality of data analysis that does not create or reinforce bias 

First-party data: Data collected by an individual or group using their own resources

General Data Protection Regulation of the European Union (GDPR): Policy-making body in the European Union created to help protect people and their data

Good data source: A data source that is reliable, original, comprehensive, current, and cited (ROCCC) 

Interpretation bias: The tendency to interpret ambiguous situations in a positive or negative way

Observer bias: The tendency for different people to observe things differently (also called experimenter bias)

Open data: Data that is available to the public

Openness: The aspect of data ethics that promotes the free access, usage, and sharing of data

Sampling bias: Overrepresenting or underrepresenting certain members of a population as a result of working with a sample that is not representative of the population as a whole

Transaction transparency: The aspect of data ethics that presumes all data-processing activities and algorithms should be explainable and understood by the individual who provides the data

Unbiased sampling: When the sample of the population being measured is representative of the population as a whole

# Module 3 - All about databases