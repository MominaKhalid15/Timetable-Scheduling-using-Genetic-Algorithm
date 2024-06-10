# Timetable-Scheduling-using-Genetic-Algorithm
Project Description
This project addresses the classical problem of timetable scheduling in a university environment. The aim is to create individual timetables for each semester, ensuring minimal clashes between sections, professors, and rooms. The objective is to assign time slots for each section in a particular room to be taught by a particular professor for a specific course.


Problem Constraints:

Hard Constraints
The following hard constraints are implemented in the project:

1.Classes can only be scheduled in free classrooms.

2.A classroom should be big enough to accommodate the section. There are two categories of classrooms: classroom (60) and large hall (120).

3.A professor should not be assigned two different lectures at the same time.

4.The same section cannot be assigned to two different rooms at the same time.

5.A room cannot be assigned to two different sections at the same time.

6.No professor can teach more than 3 courses.

7.No section can have more than 5 courses in a semester.

8.Each course would have two lectures per week not on the same or adjacent days.

9.Lab lectures should be conducted in two consecutive slots.

10.15-minute breaks are allowed between consecutive classes to ensure sufficient time for transitions.

Genetic Algorithm Implementation:

The timetable scheduling problem is solved using a genetic algorithm with the following steps:

Initial Population: An initial population of random bitstrings is generated.

Fitness Evaluation: Each candidate in the population is evaluated based on the objective function, which is the inverse or negative of the sum of all conflicts/clashes.

Selection: Tournament selection is used to select parents for the next generation.

Crossover: Parents are crossed over to create children, with a certain probability of crossover.

Mutation: Bitstrings are mutated with a certain mutation rate.

Generation Cycle: The process of evaluation, selection, crossover, and mutation is repeated for a number of generations.
