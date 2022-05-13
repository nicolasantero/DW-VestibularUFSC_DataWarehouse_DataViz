# DataWarehouse_DataViz-Entrance Exam UFSC

## Data Visualization
- [Link Dashboard PowerBI](https://app.powerbi.com/view?r=eyJrIjoiMWE5MzI0MmQtYWVjNC00N2JhLTlmMDEtMWZjZjllNDU0Yzc3IiwidCI6ImZhNzk1MzFjLThjZTUtNGJkMy05N2VlLTI0NWU2ZWUyNjZiOCJ9&pageName=ReportSection)

## SOFTWARES
- UniController
- HeidiSQL
- Pentaho Data Integration
- SQL Power Architect
- Power BI


## PROJECT
1. Analyze the socio-academic model of the Coperve entrance exams from 2008 to 2012 in order to implement a Data Mart to support the following analysis;

	- To support the decision making of the Secretary of State of SC and to evaluate the performance in the subjects of the candidates from the state public schools, comparing them to the private and federal schools.

2. Create a star schema (dimensional model) to support the analyses analyses;

3. Define the physical design for the Data Mart, following standardization, establish a transition area for the ETL process;

4. Creating the Data Mart Front End in an OLAP Tool.


## FOLDERS
- Back-end (information needed to access the database, folder with the
scripts/kettle files used in ETL, dimensional modeling);
- Front-end (information needed to access the data visualization);

## INSTRUCTIONS

- Create a local MySQL connection , in this project UniController was used to create the connection;

- Using a MySQL database manager (HeidiSQL) and connect to the MySQL connection;

- Open the vestibular data dump in the database manager;

- Use the file Script_Create_DW to create the DataWarehouse Fact and Dimensions table, but still without any data;

- With the modeling created in HeidiSQL, Spoon (Pentaho Data Integration) was used to perform the ETL steps, connecting to the same SQL connection of the DataWarehouse and the vestibular data source;

- In Spoon, the sql connection is used to pull the acceptance exam data, perform the transformations and then load in the respective dimensions and facts from the DataWarehouse database;

- The file dw_ufsc_with_data.sql contains the DataWarehouse populated with the data after the Load Step;

Translated with www.DeepL.com/Translator (free version)


## MODELING
- Relational Modeling of the source database
![Relational Model](https://github.com/nicolasantero/DW-VestibularUFSC_DataWarehouse_DataViz/blob/main/Modelos/modelagem_relacional.png?raw=true)
- Dimensional Modeling of the DataWarehouse
![Modelo Dimensional](https://raw.githubusercontent.com/nicolasantero/DW-VestibularUFSC_DataWarehouse_DataViz/main/Modelos/modelagem_DW.JPG?raw=true)

