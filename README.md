# Project Name
> Extract and Load latest N paper submissions from arXiv

## Table of contents
* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Features](#features)
* [Status](#status)
* [Inspiration](#inspiration)
* [Contact](#contact)

## General info
This is a data extraction/parse, and load into 1) .csv file 2) PostgresDB, which pulls metadata on the latest N paper submissions from the Computer Science arXiv, which is currently hosted by Cornell University.<br />


It can be accessed at https://arxiv.org/list/cs/new, and through an RSS feed at http://arxiv.org/rss/cs<br /><br />
The arXiv project (pronounced "archive" – the X represents the Greek letter chi), it’s an active repository for sharing scientific research in mathematics, physics, and computer science, among others – almost all papers in the fields of mathematics and physics are self-archived on the arXiv repository.
It’s an excellent resource as well for Artificial Intelligence and Machine Learning research.<br />

Screenshots below show:

1) df, csv, and postgre outputs and validations in Jupytner Notebook<br />
2) table created and validation in PgAdmin (Postgres DB)<br />


## Screenshots
![JupyterNotebook](https://github.com/eugene-datascience/O2E-Demo/blob/master/jupyternotebook.JPG)<br />
![Postgres](https://github.com/eugene-datascience/O2E-Demo/blob/master/postgrestable.JPG)

## Technologies<br />
*Ananconda 3 (64-bit) with Jupyter Notebook<br />
*PostreSQL 13 (64-bit)<br />
*pgAdmin 4 v4.30 (released Jan. 28, 2021)

## Setup
Install the following software <br />
https://www.anaconda.com/products/individual<br /><br />
To setup local database (set any master password)
https://www.postgresql.org/download/<br /><br />
To access local database through admin GUI<br />
https://www.pgadmin.org/download/<br />

1. Anaconda Navigator >> Launch Jupyter Notebook >> Open ARXIV_O2E_PULL.IPYNB file<br />
2. Open Postgres DB: PgAdmin4, set any master password<br />

## Code Example
Query confirms data availability:  <br />
SELECT * FROM arxiv_rss

## Features
List of features ready and TODOs for future development
* Import ARXIV RSS feed and parse 
* Write to 'ARXIVdata.csv'
* Write to Postgres DB table 'arxiv_rss'
* Validate Postgres DB with SQL Queries (validated 375 records, 371 stated by arXiv website)

To-do list:
* SSH Tunneling for remote access

## Status
Project is: complete

## Inspiration
Project inspired by Rupin Varma | Talent Acquisition Specialist, O2E Brands

## Contact
Created by [@
eugene-datascience](eugene.wong003@gmail.com) - feel free to contact me!
