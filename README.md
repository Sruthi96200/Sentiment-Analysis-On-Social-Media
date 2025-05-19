# Database Management for Sentiment Analysis on Social Media

This project presents a comprehensive database management solution tailored for large-scale sentiment analysis on social media platforms. It was developed as part of the IFT530 course at Arizona State University to demonstrate the design, development, and implementation of a scalable, query-optimized relational database system for storing and analyzing user-generated content.

##  Project Objective

With the exponential growth of social media, organizations are increasingly leveraging sentiment analysis to gain actionable insights into public opinion, brand perception, and user engagement. This project supports such analysis by providing a robust database infrastructure that enables efficient data storage, retrieval, and analytical processing across multiple platforms and languages.

##  Database Architecture

The relational schema follows a star-schema-inspired structure, incorporating both dimensional and fact tables to support OLAP-style queries and sentiment trend analysis.

### Dimension Tables:
- **Users** – Stores anonymized user identifiers.
- **Posts** – Contains raw post content and metadata.
- **Platforms** – Information on source platforms (e.g., Twitter, Instagram).
- **Hashtags** – Tracks hashtags used in posts.
- **Keywords** – Stores key terms extracted for sentiment classification.
- **Sentiment_Scores** – Holds computed sentiment metrics for posts.
- **Languages** – Details of supported languages.
- **Locations** – Geographical data associated with posts.

### Fact Tables:
- **Post_Analytics** – Aggregated metrics like likes, shares, comments.
- **Sentiment_Trends** – Time-series sentiment data (e.g., average sentiment per day).

An **Entity Relationship Diagram (ERD)** visually models all relationships and constraints, ensuring data normalization and referential integrity.

## Technical Components

- SQL scripts to create, populate, and manage all tables
- **Views** using JOIN operations and WHERE clauses for filtered analysis
- **Audit Table** with trigger-based change tracking and timestamps
- **Stored Procedure** and **User-Defined Function (UDF)** to demonstrate advanced SQL logic
- **Cursor** implementation for row-wise operations
- Header and inline comments for maintainability and clarity

## Use Cases

- Analyze public sentiment trends over time and geography
- Monitor social media engagement and platform-specific metrics
- Support NLP pipelines with structured, preprocessed datasets
- Enable dashboard integrations and BI reporting

## Tools & Technologies

- **SQL Server Management Studio (SSMS)**
- **T-SQL**
- **Git / GitHub** for version control
- **Draw.io / Lucidchart / dbdiagram.io** for ERD generation
- **PowerShell / Command Line** for repository management

## Repository Structure

Sentiment-Analysis-On-Social-Media/
│
├── SQL_Scripts/
│ ├── create_tables.sql
│ ├── insert_data.sql
│ ├── views_queries.sql
│ ├── audit_trigger.sql
│ ├── stored_procedure_udf.sql
│ └── cursor.sql
│
├── ERD/
│ └── Sentiment_DB_ERD.png
│
├── Screenshots/
│ └── ExecutedQueries.docx
│
└── Final_Report.docx

## 👩‍💻 Author

**Sruthi Keerthana Nuttakki**  
Graduate Student – Data Science, Analytics & Engineering  
Arizona State University  
--

> This project demonstrates the intersection of database engineering and social data mining—enabling real-time, scalable, and insightful sentiment analytics that can transform decision-making across domains.

