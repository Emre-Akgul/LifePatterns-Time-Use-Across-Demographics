# Time Usage Analysis Project 

## Overview
The Time Usage project is a comprehensive analysis tool developed using Apache Spark to study and visualize how different demographics allocate their time across various activities such as primary needs (sleep, eat, etc.), work, and leisure. Based on the American Time Use Survey (ATUS) dataset, this Scala application provides insights into lifestyle patterns across different genders, age groups, and employment statuses.

## Getting Started
### Prerequisites
Java 8 or above

Scala 2.12.x

sbt 1.x

Apache Spark 3.x

### Installation
Ensure Java and Scala are installed on your system.

Install sbt, which will handle the project's dependencies.

Download and install Apache Spark.

### Running the Application
Clone this repository to your local machine.

Navigate to the project directory.

Use the command sbt run to compile and execute the project.

The application reads the ATUS dataset from src/main/resources/timeusage/atussum.csv, performs data processing to summarize time usage, and outputs the analysis.

## Key Components
TimeUsage: The main object that initializes SparkSession and orchestrates the data processing flow.

TimeUsageInterface: Defines the structure and expected behaviors for data processing, including reading data, transforming, and summarizing time usage.

TimeUsageRow: A case class representing a row of the summarized dataset.

## Features
Data Reading: Reads and infers the schema of the ATUS dataset.

Column Classification: Classifies dataset columns into primary needs, work, and other activities based on predefined prefixes.

Data Summarization: Aggregates time spent on different activities into broader categories and summarizes by demographics.

Grouped Analysis: Provides three forms of grouped analysis - standard DataFrame aggregations, SQL-based aggregations, and type-safe Dataset aggregations.

Customizable Analysis: Supports analyzing time usage based on different groupings such as working status, sex, and age.
## Usage
The application automatically processes the ATUS dataset to highlight how various demographics allocate their time. It showcases the power of Apache Spark in handling and analyzing large datasets efficiently. 

Users can extend the application by modifying the timeUsageByLifePeriod method to explore different hypotheses or by adding new analyses.

## Acknowledgments
This project is based on the American Time Use Survey (ATUS) dataset.

The dataset is provided by Kaggle and is documented here:

https://www.kaggle.com/bls/american-time-use-survey

## Contact Information
For any additional questions or collaboration opportunities, feel free to contact me at emreakgulcs@gmail.com or visit my GitHub Profile.
