**SENG 637 - Dependability and Reliability of Software Systems**

**Lab. Report \#4 – Mutation Testing and Web App Testing**

| Group \#:      |     |
| -------------- | --- |
| Student Names: |     |
|                |     |
|                |     |
|                |     |

# Introduction.
This assignment comprises two parts, in the first phase, we aim to increase the mutation coverage score by writing new test cases and using the test cases from the project's last phase. For this purpose, we used the Mutation
Testing approach. This method is a type of software testing in which certain statements of the source code are changed to check if the test cases can find errors in the source code or not. We used the
Pitest tool, an automated mutation testing system, which could produce different mutated programs, to run our test cases, and report the mutation coverage report. It also provides a log about which mutation is
detected by our test cases (killed) and which survived. The system under test (SUT) is called JFreeChart, a library for creating professional charts. It is an open-source Java framework for chart
calculation, creation, and display. JFreeChart makes it easy for developers to display professional quality charts in their applications.
First, we analyze ten mutations by reading the mutation report log, and we explain which of them were killed by which original test case and how it is killed. Then, we report some equivalence mutations and try to detect them automatically. After that, we design the new test cases to increase the mutation coverage report. Then, we highlight some of the
advantages and disadvantages of mutation testing.
In the second phase of this assignment, we use Selenium IDE, a framework for testing web applications, to understand automated Graphical User Interface (GUI) testing and some of the features that record and
replay test cases. GUI testing is the process of ensuring the proper functionality of the GUI for a specific application. We chose the Shop Smart Canada page as our SUT after familiarizing ourselves with the
selenium tool extension in Chrome, we implemented test cases for ten different functionalities.


# Analysis of 10 Mutants of the Range class 

# Report all the statistics and the mutation score for each test class
## Range.ExpandToinclude PIT Summery before
![image](https://github.com/jui-kumkum/SENG637_Assignment4_Group4/blob/main/Images/ExpandtoIncludeBEFORE/PIT%20summery%20before(rangeExpandToinclude).png)



## Range.ExpandToinclude PIT Mutation before
![image](https://github.com/jui-kumkum/SENG637_Assignment4_Group4/blob/main/Images/ExpandtoIncludeBEFORE/PIT%20Mutation(rangeExpandToinclude).png)




## Range.ExpandToinclude PIT Summery after
![image](https://github.com/jui-kumkum/SENG637_Assignment4_Group4/blob/main/Images/ExpandtoIncludeAFTER/RangeExpandtoInclude%20PIT%20Summery.png)

## Range.ExpandToinclude PIT Mutation after
![image](https://github.com/jui-kumkum/SENG637_Assignment4_Group4/blob/main/Images/ExpandtoIncludeAFTER/RangeExpandtoInclude%20PIT%20Mutation.png)

## Range.getCentralValue():
A new test case was generated, and I mutated 2.0 with 1.0, KILLED. The analysis of the mutation was we return this.lower / 2.0 + this.upper / 2.0;
It replaces 2.0 with 1.0
If this. lower == 0 in the test case, the test case could not kill this one.
One test case method that could kill this one:
GetCentralValueWhenABSofBoundIsNotEqual():
● Range = (-4.0,2.0)

## DataUtilitiesCreateNumberArray2D PIT Summery before
![image](https://github.com/jui-kumkum/SENG637_Assignment4_Group4/blob/main/Images/DataUtilitiesBefore/Numer2DArrayPIT%20Summery.png)

## DataUtilitiesCreateNumberArray2D PIT Mutation before
![image](https://github.com/jui-kumkum/SENG637_Assignment4_Group4/blob/main/Images/DataUtilitiesBefore/Numer2DArrayPITMutation.png)



# Analysis drawn on the effectiveness of each of the test classes

# A discussion on the effect of equivalent mutants on mutation score accuracy

# A discussion of what could have been done to improve the mutation score of the test suites

# Why do we need mutation testing? Advantages and disadvantages of mutation testing

# Explain your SELENUIM test case design process

# Explain the use of assertions and checkpoints

# how did you test each functionaity with different test data

# How the team work/effort was divided and managed

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the assignment itself
