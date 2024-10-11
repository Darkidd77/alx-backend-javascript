TypeScript

This project includes tasks designed to teach TypeScript usage.
Tasks Overview:
0. Creating a Student Interface

In the file task_0/js/main.ts, the following is implemented:

    Define an interface called Student with the properties: firstName (string), lastName (string), age (number), and location (string).
    Create two student objects, then store them in an array called studentsList.
    Using vanilla JavaScript, generate a table, and for each student in the array, add a new row displaying their first name and location.
    Ensure Webpack runs without any type errors.
    Use TypeScript for all applicable variables.

1. Building a Teacher Interface

In task_1/js/main.ts, the following features are implemented:

    Define a Teacher interface with firstName (string) and lastName (string), which are immutable after initialization.
    Add fullTimeEmployee (boolean) and location (string), which are required attributes.
    Include yearsOfExperience (number), which is optional.
    Allow additional attributes like contract (boolean) to be added dynamically.

2. Extending the Teacher Interface

In task_1/js/main.ts:

    Create a Directors interface that extends Teacher, adding a required numberOfReports (number) property.

3. Teacher Details Printer

In task_1/js/main.ts:

    Implement a function printTeacher that accepts firstName and lastName, and returns a string combining the first letter of firstName with the full lastName (e.g., "J. Doe").
    Define an interface printTeacherFunction to describe this function.

4. Student Class Definition

In task_1/js/main.ts:

    Create a class StudentClass that has:
        A constructor accepting firstName and lastName.
        A workOnHomework method returning "Currently working".
        A displayName method that returns the student's firstName.
    Ensure both the class and its constructor are described by interfaces.
    Webpack should run without TypeScript errors.

5. Advanced Types (Part 1)

In task_2/js/main.ts:

    Define a DirectorInterface with the methods workFromHome, getCoffeeBreak, and workDirectorTasks, each returning a string.
    Define a TeacherInterface with methods workFromHome, getCoffeeBreak, and workTeacherTasks, each returning a string.
    Implement a Director class using DirectorInterface, with methods returning appropriate messages.
    Implement a Teacher class using TeacherInterface, with appropriate methods.
    Write a createEmployee function that accepts a salary (number or string). If the salary is less than 500, it returns a Teacher; otherwise, a Director.

6. Employee-Specific Functions

In task_2/js/main.ts:

    Implement a function isDirector that checks if an employee is a director.
    Implement executeWork, which calls workDirectorTasks for directors and workTeacherTasks for teachers.

7. String Literal Types

In task_2/js/main.ts:

    Define a Subjects string literal type that only allows "Math" or "History".
    Write a function teachClass that takes todayClass as an argument and returns "Teaching Math" or "Teaching History" based on the input.

8. Ambient Namespaces

In task_3/js/interfaces.ts:

    Define a RowID type equal to a number.
    Define a RowElement interface with firstName (string), lastName (string), and optional age (number).

In task_3/js/crud.d.ts:

    Export type declarations for CRUD functions and import RowID and RowElement.
    Use the CRUD library to manage database entries, and create rows and update them accordingly.

9. Namespace and Declaration Merging

In task_4/js/subjects/:

    Create a Teacher interface in a Subjects namespace requiring firstName and lastName.
    In Subject.ts, export a Subject class with a teacher and setter for the teacher.
    Extend the Teacher interface in Cpp.ts, adding experienceTeachingC (optional, number), and define Cpp class with getRequirements and getAvailableTeacher methods.

10. Update Main File

In task_4/js/main.ts:

    Export constants for Cpp, Java, and React subjects.
    Create a Teacher object with experienceTeachingC = 10 and demonstrate the methods for each subject.

11. Brand Convention & Nominal Typing

In task_5/js/main.ts:

    Define MajorCredits and MinorCredits interfaces, each with a credits number and a unique brand.
    Write sumMajorCredits and sumMinorCredits functions to sum credits from respective types.
