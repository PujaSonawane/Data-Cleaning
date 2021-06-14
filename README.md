# Data-Cleaning
This project involves the data cleaning and data normalization
Technology used: Python 
Platform: Jupyter Notebook
Packages Used: OS, pandas, CSV, Matplotlib, Colour, re

How to run the program: 
1. load the .ipynb file in Jupyter notebook environment
2. Give the path of the folder of data
3. Give the export path where you want to export the files
4. Run the individual cell in sequence as it is numbered. See the csv files in desktop file system in export path.

Cleaned Database files:
![image](https://user-images.githubusercontent.com/22337746/121931206-4fafee00-cd11-11eb-833c-be827ccbad5b.png)

Database Schema:
![image](https://user-images.githubusercontent.com/22337746/121931263-62c2be00-cd11-11eb-8182-3e5e09076e37.png)


Person-char: This table contains the person_id and the characteristics that person has reported
Char-var: This table consist of unique combination of characteristic and its respective variant.
Variant- This table consist of 5 columns: 
1.	Person_id – id for person whose genotype is decoded
2.	rsid 
3.	position- The position within the chromosome this variant is found in
4.	chromosome: The chromosome this variant is found on. Note that this is not always a number
5.	genotype: A string of 'A's, 'T's, 'C's, and 'G's represents genotype
All the tables above can be linked together with one common field in each table.

Optimizations:
In the code I have handled the file reading from folder and subfolder, it additionally handles the reading of files those end with “.txt “only

Noticed that columns file format is depending on number of columns in file. Different functions to clean different file formats so that something goes wrong with one format will not hamper cleaning of other formatted files.

Handled the normalization of variants of characteristics.

Project can be found at: https://github.com/PujaSonawane/Data-Cleaning

