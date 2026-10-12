# CST8912 Lab 4

**Student Name**: Collin MacLeod
**Student ID**: macl0379
**Course**: CST8912 Cloud Solutions Architecture
**Semester**: Fall 2026

## Introduction

In this lab, you will explore the main features of cloud SQL database for azure and learn how to deploy and manage the service by connecting and querying the database, copy data from source to target using azure data factory. In this lab, source is azure sql database (a PAAS service provided by Microsoft) and destination is azure storage account container.

## Screenshots with Analysis

### Database Setup

The resources setup for this lab was straight forward as most PaaS operations are. The key resources that were introduced in this lab were the SQL Database and SQL Server. The creation for the server was easy tied into the creation sequence for the SQL Database but more complex solutions are available. The storage account was setup with basic configuration to allow for ease of access and a simple endpoint to send data through the Database Fatory

#### Review Creation Page for SQL Database showing Options
![Review Creation Page for SQL Database showing Options](Screenshots/SQL%20Database%20Setup.png)

#### SQL Server Overview Page
![SQL Server Overview Page](Screenshots/SQL%20Server%20Setup.png)

### SQL Queries & Data Factory Tools

SQL Queries are a powerful way to search through data. With the ability to filter through data many things are possible. These can be used in conjuction with Data Factory tools to great effect. Connections and endpoints that can be used by a Data Factory is highly customizable and works well with many other services allowing it to be used with IaaS, PaaS, SaaS or on-premises systems. In the lab, we preformed a one time copy of data that is sent to any chosen endpoint. This simple example does show how this tool can be used but the possibilites are endless. If sets of data are required to be backed up in a specific storage container weekly. In the example of customer records, a command line script can quickly filter records for customers from region A (that requires data to be stored within that region) and send data to a properly configured storage account.

#### Example of SQL Query
![Example of SQL Query](Screenshots/SQL%20Query.png)

#### Selecting Data to Copy from Database
![Selecting Data to Copy from Database](Screenshots/Selecting%20Folder%20from%20Database.png)

#### Setting Data Copy Destination
![Setting Data Copy Destination](Screenshots/Copy%20Data%20Tool%20Destination.png)

#### Data Factory Copy Data Action Summary
![Data Factory Copy Data Action Summary](Screenshots/Data%20Factory%20Copy%20Data%20Action%20Summary.png)

#### Success! Data file in chosen endpoint container
![Success! Data file in chosen endpoint container](Screenshots/Data%20Received.png)

### Cleanup

#### Proof of Project Cleanup
![Proof of project cleanup](Screenshots/Project%20Cleanup.png)

## Reflections

While this was a simple action the power of these services is obvious and incredibley useful for data managment and allows for many automations. These seem like tools that are used frequently in many database systems for backups, reporting and more.
