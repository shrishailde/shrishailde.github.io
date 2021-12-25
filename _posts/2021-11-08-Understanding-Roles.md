---
layout: post
title: "The Role of Data Engineering and Analytics in an Organization"
tags: ["data engineering","data analytics"]
comments: true
---

### 1. Introduction

Before learning how to work with tools, it is very important to understand how a business works, how a business uses data, and how it can be useful. 

### 2. The Role of Analytics in an Organization

An organization exists to deliver value. There are 3 key groups who can benefit from this or that business:

* Business owners (shareholders);
* Employees;
* Customers.

![](/assets/images/20211108/roles.png)

The most important group is the customers, as many modern companies operate on the "customer obsession" principle.

In order for the business to grow, it is necessary to create more value for each of the groups. For customers, for example, customer experience. For employees - the level of balance between work and life, salary (work life balance, salary). For owners - income. All of these groups make decision making to successfully grow their businesses and get their jobs done. In order to make decisions, you need data. The data can be raw data or organized raw data. One of the tasks of the data engineer is to provide data to the groups described above for further decision making. Therefore, it is very important to understand how exactly the work done by the date engineer affects what happens to the business.

[Video 1: Importance of data to an organization](https://youtu.be/EHTmxmuhZ10){:target="_blank"}


## 3. Analytics Objectives

Analytics is the part of the business that uses data to provide information that is used to make decisions to make the business run efficiently. Analytics is needed for:

* Increased profits. If an analytical solution helps to make money, then everything is fine; if not, then there is a problem somewhere;
* Reduced costs. Cost tracking helps you save money;
* Researching new markets or products
* Compliance with requirements
* Avoiding risks

## 4. MindMap of data engineering

MindMap is a smart map, a tool for visual display of information.

![](/assets/images/20211108/demap.jpg)

* Data integration. ETL / ELT - extract, transform, load;
* Data Warehouse / Data Platform - modern data warehouse / data lake - file storage. Data platform = Data Lake + DW;
* Cloud (cloud) - cloud analytics;
* Batch - loading data in batches, this is how the classic ETL / ELT tool works / Stream - continuous data stream;
* Business Intelligence is a layer between IT and business user;
* SQL (Structured Query Language)
* Programming languages such as: Python, Scala, Java;
* MPP (Massive Parallel Processing) - an architectural feature of analytical data warehouses;
* Big Data;
* Spark is a fast and versatile data processing platform


## 5. Major roles in the data world

Traditional category:

* BI developer. Working with reports, dashboards, implementation of BI solutions (Tableau, Power BI, SAP). Often the responsibilities include providing business insights;
* ETL / ELT. Integration work ("techies");
* Report developer = BI engineer;
* DW developer / architect. Working with the solution and its architecture (how it looks and what it does);
* Data Modeler. Work with the business processes of the organization and the creation of a data model, according to which the future data warehouse will be created.

Data Engineer Category:

* Data Engineer (the classic understanding of a data engineer);
* Big Data engineer. Working with solutions related to non-relational databases;
* Cloud DE. Working with solutions in the cloud;
* Data Platform Engineer. Work with data warehouse and data lake solutions.

Profile category (Data Science, IT):

* Software Development Engineer. Good knowledge of algorithms, data structures. Sometimes the work is related to Big Data;
* Machine Learning Engineer. Good knowledge of mathematics, programming and libraries, deep learning framework;
* Visual Engineer. Working with data visualization using programming languages.
* Applied Scientist
* Research Scientist

Category advanced analytics (Forecasting elements):

* Data mining. Role before Data science;
* Data science. Good knowledge of mathematics, statistics, programming;
* Data analyst

**This blog focuses on the data engineer and traditional category roles.**

An engineer does not know everything about everything, he understands the basic principles and sees the ultimate goal, and then he creates using tools and skills. A data engineer who previously has been referred with following roles:

* Software developer
* Report Developer
* Data mining specialist
* BI Developer
* ETL developer
* DW developer

can be divided into 2 main types:

1. A programmer who became a Data Engineer.
2. BI / DW / ETL developer who became a Data Engineer.

Let's take a closer look at the differences. The task of the Data Engineer is to create a platform where data is automatically loaded, where it is transformed into an accessible form for end users (usually business users).

Data sources can be different: relational databases, SFTP, API, log files, sensors. Data types can also be different: structured data in tabular format, semi-structured (JSON, XML) and unstructured (video, audio).

Depending on the business requirements, the Data Engineer needs to create a data pipeline that will automatically pick up data and load it into the data platform (data warehouse or data lake). You need to choose tools for working with data.

Our goal is simple: to help businesses extract valuable information from data. To do this, you need to create an analytical solution where users can independently work with data, test their hypotheses and analyze business problems using the right metrics.

To build such a solution, you need a Data Engineer. In my case, this is not just creating a data stream, transforming and loading data. This is a full-fledged work with business units, understanding their needs and providing them with the tools to solve their problems.

One can use Java / Python programming languages, etc. to create a solution - Data Engineer - #1 ( Technical Data Engineer ), or one can use ready-made solutions that will allow you to create scalable and secure solutions, quickly achieve results - Data Engineer - #2 (let it be Result Oriented Data Engineer ).

Programming is indispensable even for type 2, but you do not need to be a programming guru, it is enough to understand how Python works and use small pieces of code to customize the solution.

## 6. Architecture of the analytic solution

![](/assets/images/20211108/solution.png)

3 layers of architecture:

* **Source Layer**- layer of data source systems OLTP (Online Transactional Processing) - transaction processing; systems quickly work to add data to the database, but are not designed for analytical queries; as a rule, data is created by business processes; from the first layer, all data goes to the data warehouse;

* **Storage Layer**- data storage for analytics (DW, Data Lake, Data Platform); it is desirable to have two layers in the data warehouse: Staging - a copy of all data from the first layer together; BL - data model;

* **Business Layer**- data access layer for business users through BI tools (Tableau, Power BI, SAP BO, Excel, QlikView) or SQL. Connecting to systems to view reports.

Sometimes another layer is used - Processing / Compute Layer, where the data is transformed before loading into the storage.

One more simplified architecture diagram (source: [2]) is as follows:

![](/assets/images/20211108/solution1.png)


# References:
[1] https://github.com/Data-Learn/data-engineering

[2] https://github.com/Artyom174
