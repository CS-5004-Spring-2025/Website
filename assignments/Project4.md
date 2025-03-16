# Project 4 - Fitness Tracker Refactor and Extension

### Due - Thursday, March 27, 2025

Assignment Link: There is no new assignment link. Your Project 4 solution will
be submitted to your Project 3 repository.

***This assignment description and your new P4REFLECTION.md file have been added to
the repository from which your repository is forked. Before you begin work,
visit your repository on GitHub and select Sync fork.***

This project requires you to **refactor** your Fitness Tracker and
add additional features to the application.

## Functionality Requirements

The first two requirements ask you to *refactor* your solution. The following
resources may be helpful:

- [Refactoring: Improving the Design of Existing
Code](https://learning.oreilly.com/library/view/refactoring-improving-the/9780134757681/).
Recall, you have free access to the O'Reilly catalog here: [https://www.oreilly.com/library-access/](https://www.oreilly.com/library-access/)
- [https://refactoring.guru/refactoring](https://refactoring.guru/refactoring)

### Refactor to use MVC Pattern

You will modify your solution to use the Model, View, Controller pattern. At
minimum, you will create three packages: `tracker.model`, `tracker.view`, and
`tracker.controller`. Classes related to the model, view, and controller will be
moved to the appropriate package. 

### Refactor to Remove Code Smells

Read Chapter 3 of [Refactoring: Improving the Design of Existing
Code](https://learning.oreilly.com/library/view/refactoring-improving-the/9780134757681/).
Recall, you have free access to the O'Reilly catalog here:
[https://www.oreilly.com/library-access/](https://www.oreilly.com/library-access/)

Identify ***at least two*** code smells in your Project 3 solution and refactor your
solution to remove them.

You will describe the two smells and how you refactored your solution in your reflection.

### Feature Additions

You will add ***at least three*** additional features to your solution.

Below is a list of possible features. Note, it is expected that you spend some
time thinking through the exact functionality as well as how you will implement
the feature. It is intentional that the features are not spelled out for you exactly!

1. **Export data to JSON** - Provide a menu option to export the
   in-memory data structure to JSON files. An acceptable solution is to
   overwrite the original resources/*.json files with the data the user has
   added during the program execution.
2. **Modify calorie and exercise goals** - Provide menu options to allow the
   user to modify their calorie and exercise goals. Any View operations executed
   after the change will rely on the new goals. 
3. **Generate monthly exercise challenge** - Provide a menu option to allow the
   user to get a monthly exercise challenge. The challenge will recommend a
   number of daily exercise minutes based on the history from the previous
   month. As a example, your solution may determine the average number
   of minutes of exercise per day from the previous month and recommend that
   number. You may choose to implement a more sophisticated algorithm. For full
   credit, you will modify the user profile to store the challenge for the
   current month. *Note, you will need to think through when you update the user
   profile and how/when you determine the current month.*
4. **View weekly summary** - For the seven days prior to the current day,
   display *both* whether the workout goal was met **and** whether the calorie
   goal was met.
5. **Maintain food database** - (worth two features) Maintain a separate data
   structure and corresponding JSON file that track individual foods and their calorie
   values. When the user chooses to log a food, allow them the option of
   choosing from an existing food or adding a new food to the database.
6. **Suggest your own** - You may propose your own feature by seeing Sami during
   office hour. Implementing a feature without prior approval may result in not
   earning credit if the feature is not sufficiently challenging.

## Execution Requirements

The execution requirements are the same as the Project 3 requirements:

1. Your `main` method must be in a class called `FitnessTracker` in a package called `tracker`. We will run your solution as `java tracker.FitnessTracker`. You may assume that the data to be loaded on startup is in the *resources* directory in files named `profile.json`, `nutrition.json` and `fitness.json`.
2. `build.gradle.kts` has been updated to include the [Jackson](https://github.com/FasterXML/jackson) JSON parsing library as a dependency. You are responsible for updating `build.gradle.kts` if your solution depends on any other third-party libraries.

## Reflection

Submit your reflection in the file P4REFLECTION.md.

Your reflection will address the following three questions:

1. Describe the two code smells you identified in your Project 3 solution and
   how you fixed them for Project 4.
2. Summarize all three of the features you added. Make sure to describe any
   design decisions you had to make and provide a brief overview of how you
   implemented the feature.
3. How much time did you spend on the project? Which pieces required the most time?

## Grading Rubric

The assignment is worth 25 points in total. For criteria worth more than one point,
partial credit may be awarded. For criteria worth one point, the solution must
be completely correct to earn credit.

| Criterion                                 | Points | 
|-------------------------------------------|--------|
| MVC packages are implemented                | 2      |
| MVC Design is appropriate                   | 2      |
| Code smell refactor                          | 2      |
| Additional feature 1  - functionality      | 2      |
| Additional feature 1  - design                   | 2      |
| Additional feature 2  - functionality      | 2      |
| Additional feature 2  - design                   | 2      |
| Additional feature 3  - functionality      | 2      |
| Additional feature 3  - design                   | 2      |
| Testing is complete                       | 1      |
| Style check passes                        | 1      |
| Javadoc                                   | 1      | 
| Reflection                                | 4     | 
