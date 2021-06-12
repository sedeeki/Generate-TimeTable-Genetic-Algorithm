# Generate-TimeTable-Genetic-Algorithm
Generate a timetable using genetic algorithm 


The input data that comes from the excel file is the same as the assignment says to use as input. The 
classes used are timetable which has list of teachers, sections, classrooms. The classrooms have classes 
in them and their room number. The classes have section, type, teacher, start time, duration etc.
The genetic algorithm populates the dictionary of days with list of all classrooms.
The classes have available room numbers which are picked randomly and hence the class is added to the 
classroom with tat room number.
The start time is also randomly assigned to each class.
After populating the population of timetables, the fitness function assigns scores to each time table and 
sorts them in descending order, with the first having the highest score. 
Then, all our cross overed with the next index to their own and mutated if random number is below the 
mutation rate provided
The new population is run through the fitness function and then sorted. 
The top 50 percent of the new population replaces the below 50 percent of the old population 
Hence a new population is returned and a function is called to check if there exists a time table with 
score of 53 that means all constraints are fulfilled. 
If value of 53 is not found, the process is repeated.
