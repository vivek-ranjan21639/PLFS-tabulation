# About Author 
**Name:** Vivek Ranjan

**Email id:** vivekranjan21639@gmail.com

**LinkedIn:** https://www.linkedin.com/in/vivek-ranjan-iit-delhi/ 




## Name of the Project: Fetching PLFS data and generating multi-index table from it.

### About PLFS
PLFS, or the Periodic Labour Force Survey, is a survey conducted by the National Statistics Office (NSO) in India to collect data on employment and unemployment. 
It's designed to provide more frequent labour force data than the previous annual surveys. PLFS collects data through two approaches: Usual Status (US) and Current Weekly Status (CWS). 
Usual Status refers to ratios for long term (refrenec period for US is 360 days) wh;e CWS refers to employmenta nd unemployment ration for short time duration (reference period for CWS is 7 days). 

***Note:*** **PLFS is executed based on agriculture year (July -June). However, data is also provided based on agriculture year for allingnmment with international requirtements to be used as data source.** 

***Link:*** https://microdata.gov.in/NADA/index.php/catalog/PLFS/?page=1&sort_order=desc&ps=15&repo=PLFS

***Note:*** Till 2023-24 PLFS data used to contain two types of data file. On epertained to  **'perv'** which is person level data and one if **'hhrv'** which is household level data. for our analysi purpose perv is required. 
hhrv is used for the purpose of enlisting, indentification and updation of the dataframe. **So, we would only focus on 'perv' data.**

### Understanding Data files
Till PLFS 2023-24 uit level data was provided as a txt file with no headers specified. the guidlines for the hader was given in another excel file named as data layout. We have to extract he column names from the data layout file 
and read the unit level txt dat with the help of it. Also, values of all the column are coded which you can find in the document of guide for field staff file. 
mult in the last column is nothing but the population projection for the sample unit.

### Objective of this project
This project was not meant to do generate entire table from the unit level data but only to showcase how to do it for the users who wish to use the data. objective of this projectys are as follow:
- To understand about the data files
- How to fetch and read the data files
- How to generate complex multi-index tables which is used in final report of PLFS.
