0x03-ES6_data_manipulation

This project contains tasks for learning to manipulate data in ECMAScript 2015 (ES6).

Tasks To Complete
 0. Basic list of objects
0-get_list_students.js contains a script that exports a function named getListStudents with the following requirements:

Returns an array of objects.
Each object should have three attributes: id (Number), firstName (String), and location (String).
The array contains the following students in the order they're listed:
Guillaume, id: 1, in San Francisco.
James, id: 2, in Columbia.
Serena, id: 5, in San Francisco.
 1. More mapping
1-get_list_student_ids.js contains a script that exports a function named getListStudentIds with the following requirements:

Returns an array of ids from a list of object.
This function is taking one argument which is an array of objects - and this array is in the same format as the return value of getListStudents from the previous task.
If the argument is not an array, the function returns an empty array.
You must use the map function on the array.
 2. Filter
2-get_students_by_loc.js contains a script that exports a function named getStudentsByLocation with the following requirements:

Returns an array of objects who are located in a specific city.
It should accept a list of students (from getListStudents) and a city (string) as parameters.
You must use the filter function on the array.
 3. Reduce
3-get_ids_sum.js contains a script that exports a function named getStudentIdsSum with the following requirements:

Returns the sum of all the student ids.
It should accept a list of students (from getListStudents) as a parameter.
You must use the reduce function on the array.
 4. Combine
4-update_grade_by_city.js contains a script that exports a function named updateStudentGradeByCity with the following requirements:

Returns an array of students for a specific city with their new grade.
It should accept a list of students (from getListStudents), a city (String), and newGrades (Array of “grade” objects) as parameters.
newGrades is an array of objects with this format:
{
  studentId: Number,
  grade: Number,
}
 5. Typed Arrays
5-typed_arrays.js contains a script that exports a function named createInt8TypedArray with the following requirements:

Returns a new ArrayBuffer with an Int8 value at a specific position.
It should accept three arguments: length (Number), position (Number), and value (Number).
If adding the value is not possible the error Position outside range should be thrown.
 6. Set data structure
6-set.js contains a script that exports a function named setFromArray with the following requirements:

Returns a Set from an array.
It accepts an argument (Array, of any kind of element).
 7. More set data structure
7-has_array_values.js contains a script that exports a function named hasValuesFromArray with the following requirements:

Returns a boolean if all the elements in the array exist within the set.
It accepts two arguments: a set (Set) and an array (Array).
 8. Clean set
8-clean_set.js contains a script that exports a function named cleanSet with the following requirements:

Returns a string of all the set values that start with a specific string (startString).
It accepts two arguments: a set (Set) and a startString (String).
When a value starts with startString you only append the rest of the string. The string contains all the values of the set separated by -.
 9. Map data structure
9-groceries_list.js contains a script that exports a function named groceriesList with the following requirements:

Returns a map of groceries with the following items (name, quantity):
"Apples", 10
"Tomatoes", 10
"Pasta", 1
"Rice", 1
"Banana", 5
 10. More map data structure
10-update_uniq_items.js contains a script that exports a function named updateUniqueItems with the following requirements:

Returns an updated map for all items with initial quantity at 1.
It should accept a map as an argument. The map it accepts for argument is similar to the map you create in the previous task.
For each entry of the map where the quantity is 1, update the quantity to 100. If updating the quantity is not possible (argument is not a map) the error Cannot process should be thrown.
 11. Weak link data structure
100-weak.js contains a script that meets the following requirements:

Export a const instance of WeakMap and name it weakMap.
Export a new function named queryAPI. It should accept an endpoint argument like so:
{
  protocol: 'http',
  name: 'getUsers',
}
Track within the weakMap the number of times queryAPI is called for each endpoint.
When the number of queries is >= 5 throw an error with the message Endpoint load is high.
