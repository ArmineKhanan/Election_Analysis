# Election_Analysis
UC Berkeley BootCamp challenge 3 (Python)

# Overview of Election Audit

# Election Audit Results
## Candidates
Total number of votes cast
A complete list of candidates who received votes

Total number of votes each candidate received

Percentage of votes each candidate won

The winner of the election based on popular vote


## Turnout

The voter turnout for each county

The percentage of votes from each county out of the total count

The county with the highest turnout

# Election Audit Summary
Script reusability
```
# Add our dependencies.
import csv
import os
#Sets current directory
os.chdir(os.path.dirname(os.path.abspath(__file__)))
# Assign a variable to load a file from a path.
file_to_load = os.path.join("election_results.csv")
# Assign a variable to save the file to a path.
file_to_save = os.path.join("election_analysis.txt")

```
The data consists of a number for the ballot ID and a name for the county and candidate, respectively. 
