# Election Analysis

## Overview of Election Audit
### Framework
We are going to assist Colorado board of elections employee, Tom. The latter is trusted to deliver an election audit for a U.S. congressional precinct in Colorado. We will take into account three primary voting methods: mail-in ballots, punch cards, and direct recording electronic, or DRE, counting machines. After all the votes are counted, our job is to generate a vote count report to certify this U.S. congressional race. Moreover, to complete the audit we are tasked to also report on each county turnover rate.
Tom's manager is interested in applying the solution to audit not only other congressional districts, but also senatorial districts and local elections,  and wants to know if there's a way to automate the process using Python.

### Resources
To deliver an effective audit we are going to leverage the following resources:
* Well-defined task requirements
* Tabulated results of election 
* Software: The Command Line and Visual Studio

## Election Audit Results
All the results of audit can be accessed via  [Go to the Support Web Site](https://github.com/ArmineKhanan/Election_Analysis/blob/main/election_analysis.txt)
### Candidates
The first group of deliverables are the following which can be found in election_analysis.txt.
* Total number of votes
* A complete list of candidates who received votes
* Total number of votes each candidate received
* Percentage of votes each candidate won
* The winner of the election based on popular vote


### Turnout

* The voter turnout for each county
* The percentage of votes from each county out of the total count
* The county with the highest turnout

## Election Audit Summary
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
