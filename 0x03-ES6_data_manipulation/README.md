ES6 Data Manipulation

This project features a series of tasks aimed at mastering data manipulation in ECMAScript 2015 (ES6).
Tasks Overview
0. Basic List of Objects

The script 0-get_list_students.js exports a function named getListStudents with the following requirements:

    Returns an array of objects.
    Each object contains three properties: id (Number), firstName (String), and location (String).
    The array includes the following students in the specified order:
        Guillaume, id: 1, located in San Francisco.
        James, id: 2, located in Columbia.
        Serena, id: 5, located in San Francisco.

1. More Mapping

The script 1-get_list_student_ids.js exports a function named getListStudentIds with these specifications:

    Returns an array of IDs extracted from a list of objects.
    Takes one argument: an array of objects formatted like the output of getListStudents.
    If the argument is not an array, it returns an empty array.
    The map function must be utilized.

2. Filtering

The script 2-get_students_by_loc.js exports a function called getStudentsByLocation with the following requirements:

    Returns an array of objects for students located in a specific city.
    Accepts a list of students (from getListStudents) and a city (String) as parameters.
    The filter function should be applied.

3. Reducing

The script 3-get_ids_sum.js exports a function named getStudentIdsSum with these requirements:

    Returns the total sum of all student IDs.
    Accepts a list of students (from getListStudents) as a parameter.
    The reduce function must be used.

4. Combining Data

The script 4-update_grade_by_city.js exports a function called updateStudentGradeByCity with the following criteria:

    Returns an array of students from a specific city along with their updated grades.

    Accepts a list of students (from getListStudents), a city (String), and newGrades (an array of "grade" objects) as parameters.

    The newGrades array should follow this format:

    json

    {
      studentId: Number,
      grade: Number
    }

5. Typed Arrays

The script 5-typed_arrays.js exports a function named createInt8TypedArray with these requirements:

    Returns a new ArrayBuffer with an Int8 value at a specified position.
    Accepts three arguments: length (Number), position (Number), and value (Number).
    If the value cannot be added, an error "Position outside range" should be thrown.

6. Set Data Structure

The script 6-set.js exports a function named setFromArray with these requirements:

    Returns a Set created from an array.
    Accepts one argument: an array of any element type.

7. More on Set Data Structure

The script 7-has_array_values.js exports a function called hasValuesFromArray with the following criteria:

    Returns a boolean indicating whether all elements in the array exist within the set.
    Accepts two arguments: a set (Set) and an array (Array).

8. Cleaning Sets

The script 8-clean_set.js exports a function named cleanSet with these requirements:

    Returns a string of all set values that begin with a specified substring (startString).
    Accepts two arguments: a set (Set) and a startString (String).
    When a value starts with startString, only the remainder of the string is appended. The final string should list all values separated by a dash (-).

9. Map Data Structure

The script 9-groceries_list.js exports a function called groceriesList with the following requirements:

    Returns a map of grocery items with the following entries:
        "Apples", 10
        "Tomatoes", 10
        "Pasta", 1
        "Rice", 1
        "Banana", 5

10. Updating Map Data Structure

The script 10-update_uniq_items.js exports a function named updateUniqueItems with these criteria:

    Returns an updated map where all items initially have a quantity of 1.
    Accepts a map as an argument, which resembles the map created in the previous task.
    For each entry where the quantity is 1, update it to 100. If the argument is not a map, throw an error "Cannot process."

11. Weak Link Data Structure

The script 100-weak.js fulfills the following requirements:

    Exports a constant instance of WeakMap named weakMap.

    Exports a function called queryAPI, which accepts an endpoint argument like this:

    json

{
  protocol: 'http',
  name: 'getUsers'
}

Tracks the number of times queryAPI is called for each endpoint within the weakMap.

If the number of queries reaches 5 or more, throw an error with the message "Endpoint load is high."
