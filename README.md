##  🎯 Purpose
This repo represents the final graduation project (covid dataset ) for Sprints Big data masterclass .

Masterclass link:

https://sprints.ai/course/Big-Data-MasterClass-1345046


## 🍀 Sponsors
This project exists thanks to :  ** Eng. Ahmed Reda ** and **Eng. Amr Saleh **
</p>

<p align="center">
		<img width="30%" src="https://user-images.githubusercontent.com/94313948/235050112-a553a37a-3b9e-400b-86fc-03922562ff99.png">

</p>


## Main Business Requirement
this project aims to  Create an automated pipeline workflow from ingestion till visualization for COVID dataset 
1. show on a map the top 10 ranking
countries in death rate
2. show on a map the top 10 ranking
countries in testing rate
3. show the top 10 ranking countries in
testing rate on a pie chart


## Technical Requirements

1. Create Folder on the cloudera Virtual Machine 
2. Upload dataset “covid-19.csv” into VM using WinSCP 
3. Load the dataset to HDFS directory using HDFS cli commands in a shell script
4. Create database on Hive and create schema for each Hive loading stage

	I. 1st Hive staging table for pointing to dataset location to select data from
	
	II. 2nd Hive ORC table is partitioned by Country and data are loaded dynamically into it to speed query
	
	III. 3rd Final hive table to generate the final report which will generate output file to be visualized
	
5. Create an Oozie workflow actions from to run the HDFS shell script and execute the Hive queries



