# YouTube-Data-Harvesting
## Introduction
This project aims to develop a user-friendly Streamlit application that utilizes the Google API to extract information on a YouTube channel, stores it in a SQL database, and enables users to search for channel details and join tables to view data in the Streamlit app.
## Project Objective:
I completed a streamlit user interface project for YouTube data gathering and warehousing. This project pulls data from YouTube and saves it in a MySQL database using a YouTube API key. Then it retrieves information from MySQL and produces a reply for every one of the ten sample queries. 
## Developer Guide 

### 1. Tools Install

* Visual Studio.
* Python 3.11.0 or higher.
* MySQL.
* Youtube API key.

### 2. Requirement Libraries to Install

* pip install google-api-python-client
* mysql-connector-python
* mysql
* pandas
* Datetime
* streamlit

### 3. Import Libraries
**Youtube API libraries**
* import googleapiclient.discovery
* from googleapiclient.discovery import build

**SQL libraries**
* import mysql.connector
* import pymysql

**Datetime library**
* from datetime import datetime

**Pandas**
* import pandas as pd

**Dashboard libraries**
* import streamlit as st

### 4. Process
#### a) Extracting the data

Using the YouTube channel id and the YouTube API developer console, collect the specific YouTube channel data. Using the playlist id, we can extract video data from a specific channel.

#### b) Processing the data

Take the necessary information from the extracted data.

#### c) Load  data 

Create the required tables and database. Then an insert query stores the data in the MySQL database.

#### d) Access MySQL DB 

Using the pymysql library and access tables, establish a connection to the MySQL server and get access to the specified MySQL DataBase.

#### e) Filter the data

Apply SQL queries to process the information obtained from the tables in accordance with the given questions. Next, create a DataFrame format out of the processed data.

#### f) Visualization 

Finally, make use of Streamlit to build a dashboard. Provide the user with dropdown options on the dashboard.

## User Guide

#### Step 1. Data collection zone

Search **channel_id**, copy and **paste on the input box** and click the **View Channel Details** button.

#### Step 2. Data Storage Zone

Paste the copied **channel_id** on the **input box** and click the **Collect and Store Channel Data**

#### Step 3. Data View Zone

By clicking the **Channels, Videos and Comments** radio, you can see the data in a tabular form.

#### Step 4. Analysis Zone

* By selecting the Queries provided in the **dropdown box** we can analyse the data which we have **collected and stored**. 

#### Notes:
* First, you need to provide your YouTube Developer Console API key in the coding section - 'api_key'.
* Secondly, the MySQL connection will only function if you enter your original login, host, and password.
