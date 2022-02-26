# Pandas_Activities
Using pandas to clean and sort data

## Overview

 Analysis of school and student data.



Here is the list of deliverables for the analysis of the school district: 

- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:
  - Top 5 and bottom 5 performing schools, based on the overall passing rate
  - The average math score received by students in each grade level at each school
  - The average reading score received by students in each grade level at each school
  - School performance based on the budget per student
  - School performance based on the school size 
  - School performance based on the type of school

At least one of the datasets needs to be cleaned before any analysis can be performed. She would like you to use Pandas to do a more thorough inspection of the datasets than you did when you opened them with Excel. Cleaning the data is essential because any missing, malformed, or incorrect data in the rows can jeopardize the analysis.

**Remember** when Maria asked what anomaly you noticed in the `students_complete.csv` file? You found that one of the students' names had the prefix "Dr." Now Maria wants you to find all the students' names that have a professional prefix or suffix. Once you get all the incorrect student names, your next task is to clean the names by removing these professional prefixes and suffixes. Maria is not sure how these names came to have professional prefixes or suffixes, but it's important they are removed. These names are not coinciding with the school records, so the students' scores can't be added their student portfolio and may cause problems when they apply to colleges. Moreover, we can't drop these names because this would affect the total student count of the district as well as the individual schools, which will negatively impact the analysis.

In the `student_names` list, we can use a `for`loop to iterate through the list, split each name, and print out the name and the length of the name.

In a new cell, add the following code and run the cell.

```python
# Split the student name and determine the length of the split name.
for name in student_names:
    print(name.split(), len(name.split()))
```

## Resources

For more information about Python modules and packages, reading CSV files, and using the `head()` and `tail()` methods in Pandas, refer to the following documentation:

- [Importing Python modules and packages (Links to an external site.)](https://www.pythonlikeyoumeanit.com/Module5_OddsAndEnds/Modules_and_Packages.html)
- [Reading a CSV file into a Pandas DataFrame (Links to an external site.)](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html)
- [Using .head() on a DataFrame (Links to an external site.)](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.head.html)
- [Using .tail() on a DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.tail.html)
