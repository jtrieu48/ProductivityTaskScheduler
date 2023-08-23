
# Task Scheduler
 
 > Authors: [Giovanni Costagliola](https://github.com/gcost003), [Justin Trieu](https://github.com/jtrieu48), [Angelica Simityan](https://github.com/AngelicaSimityan), [Carlos Miranda ](https://github.com/kotooriiii)
 

## Project Description
 > * Why is it important or interesting to you?
As students, a Task Scheduler allows us to organize our daily lives. Being able to create detailed tasks with due dates and descriptions keeps us on top of our busy schedules. Keeping all of our tasks in a single application lets us catalog our lives in a convenient workspace.
 > * What languages/tools/technologies do you plan to use? (This list may change over the course of the project)
 >   * [toolname](link) - Short description
 > * What will be the input/output of your project?
 > * What are the two design patterns you will be using? For each design pattern you must explain in 4-5 sentences:
 >   * Why you picked this pattern and what feature you will implement with it
 >   * What problem you anticipate encountering when implementing your project that you will solve using the design pattern
 >   * Why the chosen design pattern will lead to a good solution to that problem
=======
 > * **Why is it important or interesting to you?**
> As students, a Task Scheduler allows us to organize our daily lives. Being able to create detailed tasks with due dates and descriptions keeps us on top of our busy schedules. Keeping all of our tasks in a single application lets us catalog our lives in a convenient workspace.
What languages/tools/technologies do you plan to use? (This list may change over the course of the project)
C++, github, PuTTy, gtest
 > * **What languages/tools/technologies do you plan to use? (This list may change over the course of the project)**
 > We will be using C++, github, PuTTy, and gtest. C++ for an objected oriented programming workspace since we are all most proficient at it. GitHub for version control system and for a backup repository. PuTTY to connect to Hammer. GTest to create unit tests and make sure the program's classes work as intended.
 > * **What will be the input/output of your project?**
 > Input will be taken from the users to generate visual blocks of Tasks with due dates, descriptions, and further details. Output will display a calendar with the tasks in a user-friendly manner. The program will notify users if their task is due today.
 >Output will display a calendar with the tasks in a user-friendly manner. The program will notify users if their task is due today.
 > * **What are the two design patterns you will be using? For each design pattern you must explain in 4-5 sentences:**
 >   * **Why you picked this pattern and what feature you will implement with it**
 >   * **What problem you anticipate encountering when implementing your project that you will solve using the design pattern**
 >   * **Why the chosen design pattern will lead to a good solution to that problem** <br>
 > We will be implementing the Structural-Composite design pattern as a part of our Task Scheduler. The composite structure, which focuses on creating multiple instances of a type of object, fits with the idea of creating multiple Tasks of varying details. We will be able to put the tasks into categories as well as organize them in a certain way. This will allow the Task Scheduler to categorize based on the type of work or priority. <br>
> We will also be using the Creational-Builder design pattern to handle the varying types of tasks. This pattern allows us to categorize our tasks with different types of object-creating paths. While the tasks will inherit from our base class, the Builder pattern enables us to create different types of the original object. This comes into consideration while creating different task templates for the different classifications of tasks: Work, Personal and Study. <br>
> So bascially these Builder pattern, Creational are design patterns about class instantiation or object creation. These patterns can be further categorized into Class-creational patterns and object-creational patterns. While class-creation patterns use inheritance effectively in the instantiation process, object-creation patterns use delegation effectively to get the job done.


## Class Diagram
 
 ![UML Diagram](https://github.com/cs100/final-project-cmira039-gcost003-jtrie002-asimi003/blob/master/resources/UMLDiagram.png)
 
 The Planner class will contain the entire collection of TaskInterfaces. The TaskInterfaces, while using the Composition strategy pattern, will allow us to remind the user using any class that is subclassed to TaskInterface. Some examples include: TaskList and Task. In addition, in order to categorize each Task, we will require to create the Classification class. We will be able to assign classifications to each Task. The Builder strategy pattern will be used to create Tasks from scratch. This will allow us to assign defaults and quickly construct objects.


## Screenshots
![screenshot1](https://github.com/cs100/final-project-cmira039-gcost003-jtrie002-asimi003/blob/master/resources/CS100_Screenshot1.png)

![screenshot2](https://github.com/cs100/final-project-cmira039-gcost003-jtrie002-asimi003/blob/master/resources/CS100_Screenshot2.png)

![screenshot3](https://github.com/cs100/final-project-cmira039-gcost003-jtrie002-asimi003/blob/master/resources/CS100_Screenshot3.png)

![screenshot4](https://github.com/cs100/final-project-cmira039-gcost003-jtrie002-asimi003/blob/master/resources/CS100_Screenshot4.png)

## Installation/Usage
The program installation requires someone to be able to call a .out file.

- The user is prompted with a main menu. They are shown 5 options which are : “Create a task”, “Remove a task”, “View all reminders”, “Edit a task”, “Undo”, and “Exit”
- Creating a task allows the user to create a task or a tasklist.
  - Task creation asks the user to enter title, description, classification, due date, and end date.
- Removing a task allows the user to remove a task from the planner.
  - Asks the user for the title of the task.
- Viewing all reminders displays each task to the console.
  - Displays simply to the console.
- Edit a task changes the task details
  - Task edit asks the user to edit a title, description, classification, due date, OR end date.
- Undo reverts back to the previous task before editing.
  - Simply undos.
- Exit, exits the program

## Testing
For testing, we created test cases and tested each individual task, classification, builder, and planner class in order to validate the cases. We also tested examples using the planner for undoing tasks.
Tasks and classifications are IMMUTABLE in testing.
