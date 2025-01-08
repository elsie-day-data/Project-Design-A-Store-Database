# Box Office Hits SQL Database

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Preparation](#data-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results Or Findings](#results-or-findings)
- [Insights](#insights)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References or Resources](#references-or-resources)

---
### Project Overview
---

This data analysis project aims to create my own store from scratch by: 1) creating a table with at least 5 columns and 15 items, 2) order the items by price, 3) show at least one statistic about the items.

<img width="186" alt="Screenshot 2025-01-07 at 9 06 43 PM" src="https://github.com/user-attachments/assets/ed56991a-191b-4823-9a2e-c99b0826c334" />

<img width="161" alt="Screenshot 2025-01-07 at 9 06 56 PM" src="https://github.com/user-attachments/assets/59acaf4d-af95-4062-8b28-6c84f36b252f" />

<img width="423" alt="Screenshot 2025-01-07 at 9 07 18 PM" src="https://github.com/user-attachments/assets/aa8dfc0b-95be-4889-9afa-c6e1c08d718f" />
<img width="434" alt="Screenshot 2025-01-07 at 9 07 32 PM" src="https://github.com/user-attachments/assets/21c5cc96-6ef5-4df8-818a-e6f5e49ada3e" />




<img width="396" alt="Screenshot 2025-01-07 at 9 07 43 PM" src="https://github.com/user-attachments/assets/29402d41-a06c-4061-9f1a-9dcb4b2ddd89" />

<img width="430" alt="Screenshot 2025-01-07 at 9 07 49 PM" src="https://github.com/user-attachments/assets/80cecf56-a863-4520-9f75-9a93db2de897" />


---
### Data Sources
---

Plant List Data: The primary dataset used for this was Perplexity.

---
### Tools
---

- SQL Lite

---
### Data Preparation
---
In the initial data preparation phase, I performed the following tasks:
1. Created a plant list using ```/** Plant list: **/```.
2. Created the table with 6 columns for my plant list to go into using ```CREATE TABLE plants```.
4. Used the ```INSERT INTO``` command to insert the previously created list of 15 plants into the newly created table.
5. Used THE  ```SELECT * FROM``` and ```ORDER BY price``` to load the data into the table and sort by the plant price.
6. Created an aggregate function query to give me the total value of the Spider Plant if I sold all 10. (See below for code details)

---
### Exploratory Data Analysis
---

EDA involved exploring the movie data to answer key questions such as:
1. What would I like to sell in my plant store?
2. What are the values I would like to see regarding my plants?
3. What would the value of the Spider Plant be if I sold all 10 plants in stock?

---
### Data Analysis
---

Interesting code/features worked with:

```SELECT name, quantity, price, (quantity * price) AS total_sale_amount
FROM plants
WHERE name = 'Spider Plant';
```

---
### Results or Findings
---

The analysis results are summarized as follows:
- The results revealed that the value of the Spider Plant sales would be $120 in total.

---
### Insights
---

I wasn't able to do this without looking at some examples. Also, I had to get help from Perplexity to figure out the aggregate data query on the Spider Plants. 

The hierarchical steps to take in the future are, pair a basic SELECT statement with: 
  1. Column(s) selection
  2. A calculation field
  3. Table specification
  4. A filter condition

---
### Recommendations
---

- Could continue to evaluate the cost of the total sales for each plant.

---
### Limitations
---

There were no limitations in this database. In the future I will use this section to detail any outliers or adjustments I had to make to the data to protect the accuracy of analysis I'm working to achieve.

---
### References or Resources
---

1. [Khan Academy](https://www.khanacademy.org/computing/computer-programming/sql/sql-basics/pp/project-design-a-store-database)
