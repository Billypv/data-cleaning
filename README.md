# Readme

## Instructions

please put all files except for 2013_Bassetlaw_outlet.csv, branch_expenses.xlsx, branch_list.xlsx, products_list.csv and terminologies.txt into the data folder.
put 2013_Bassetlaw_outlet.csv in replacement_filesdata and the rest in other_files

## software required
if you are extracting the .ipynb file to a .py file, you will need to make sure you have the libraries required. These are found in the first cell of the jupyter notebook please install them with the following commands 
- pip3 install pandas
- pip3 install glob
- pip3 install fuzzywuzzy
- pip3 install python-Levenshtein
python-Levenshtein is optional, however it improves the fuzzywuzzy library by making it less time expensive.

## assumptions about data
- The data has typos
- The headers are not in the correct order
- Not all of the numeric data is numeric
- all of the strings are strings
- the supplementary files we were given are correct
- All numbers are correct to within 2 dp

## Interesting functions
I particularly enjoyed using the FuzzyWuzzy Library as matching strings that are not identical is something that I have been looking for a solution to for some time.
The Levenshtein function to determine how many edits two strings are from each other is a very interesting way to do this.

## Extracting Data
Once you have run all of the cells in order, you can find the cleaned data in the file cleaned_data, this is then split into sections for the requirements for the dash part of the task.
