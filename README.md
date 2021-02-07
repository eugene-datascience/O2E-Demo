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
This is a data extraction, parse, and load into Postgres, which pulls metadata on the latest N paper submissions from the Computer Science arXiv, which is currently hosted by Cornell University.<br />


It can be accessed at https://arxiv.org/list/cs/new, and through an RSS feed at http://arxiv.org/rss/cs<br /><br />
The arXiv project (pronounced "archive" – the X represents the Greek letter chi), it’s an active repository for sharing scientific research in mathematics, physics, and computer science, among others – almost all papers in the fields of mathematics and physics are self-archived on the arXiv repository.
It’s an excellent resource as well for Artificial Intelligence and Machine Learning research.<br />

The validations are done in Jupytner Notebook, and also PgAdmin for the Postgres DB. See screenshots.


## Screenshots
![JupyterNotebook](https://github.com/eugene-datascience/O2E-Demo/jupyternotebook.JPG)<br />
![Postgres](https://github.com/eugene-datascience/O2E-Demo/postgrestable.JPG)

## Technologies<br />
*Ananconda 3 (64-bit) with Jupyter Notebook<br />
*PostreSQL 13 (64-bit)<br />
*pgAdmin 4 (Windows), pgAdmin 4 v4.30 (released Jan. 28, 2021)

## Setup
Install the following software <br />
To open .IPYNB file (Jupyter Notebook)<br />
https://www.anaconda.com/products/individual<br /><br />
To setup local database
https://www.postgresql.org/download/<br /><br />
To access local database through admin GUI<br />
https://www.pgadmin.org/download/pgadmin-4-windows/


## Code Example
Query confirmation of data availability:  <br />
SELECT * FROM FROM public.arxiv_rss

## Features
List of features ready and TODOs for future development
* Import ARXIV RSS feed and parse 
* Write to ARXIVdata.csv
* Write to Postgres DB
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
