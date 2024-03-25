# **Object Basics**
Objects are a type of primitive in JS. **Objects allow you to map keys to values**. See following example.
![alt text](<Screenshot 2024-03-24 at 2.29.19 PM.png>)
- Objects allow you to map keys to values. For example 'lastName' could map to 'Time' and 'isOld' could map to 'true'. **When you want to know the name property of the object, you look it up and get the value back (in this case, 'Time')**.
- Object Format - It has a `key`, followed by a `:`, followed by a `value`, then a `,`. However the last key/value in the object omits the comma. This is a common syntax error, include the comma in the list of keys and ommit the last comma or you will be met with the error message: *Uncaught SyntaxError: Unexpected identifier*
- Objects are one of the built-in types in JS. `Objects consist of unordered key-value pairs`.
    - In the Obj1 example the set of keys are "firstName, lastName, isOld" and the values are "'Father', 'Time', true"
- After creating an object we can access the values using the object's keys. 
![alt text](<Screenshot 2024-03-24 at 2.36.59 PM.png>)
You can use dot notation or bracket notation, respectively.
- //When using bracket notation be sure to define variables inside with "". See below:
![alt text](<Screenshot 2024-03-24 at 2.42.15 PM.png>)
- It is best practice to use dot notation (if you can), but there are cases where you'll need to use bracket notation.
![alt text](<Screenshot 2024-03-24 at 3.01.07 PM.png>)
    - as seen with "objj.3; , resulted in syntax error and we can't use dot notation.
    - But with "objj[3]; , this resulted in "Three", we need to use bracket notation.
    - Essentially, use the bracket notation when you need to evaluate an expression or pass in a variable to get the name of the key. Use the dot notation when you know the name of the key and it is not a variable or expression.

**Keys are ALWAYS strings in JS**
- It is important to note that they type of a key in JS is always a string. In example below, we create an object of an employee ID to an employee name.
![alt text](<Screenshot 2024-03-24 at 3.13.58 PM.png>)
To Access key 704 to get the value "Douglas" we cannot use dot notation. Must use bracket notation and the value inside the bracket is a string.
![alt text](<Screenshot 2024-03-24 at 3.16.34 PM.png>)
    - The takeaway here is even though we did not quote the key name when creating the idToName object, JS automatically converted the number to a string. **EVERY key in a JS object is a string!**.

**Adding/Removing from Objects**

* **ADDING** -to add properties or functions/methods to an object we can use dot or bracket notation (as before, dot is preferred, but not always possible).
    - enter `object name`, `.` , then `name of new property`.

![alt text](<Screenshot 2024-03-24 at 3.26.17 PM.png>)

* **REMOVING** - to remove, use `delete` keyword, followed by object name.value.  It is the same format as adding, but with delete (and a space) in front.

![alt text](<Screenshot 2024-03-24 at 3.41.38 PM.png>)

Exercises: 

![alt text](<Screenshot 2024-03-24 at 3.48.20 PM.png>)

## **Object Iteration**
One of the paramount concepts in programming it iteration (looping). If we want to print out all the values in an object, you can type each command individually (time consuming) or through looping. *Looping is advantageous for saving time AND in cases where we don't know the keys that an object has.

* Note: we used for...of to iterate over arrays and strings. This does NOT work with objects 
(will result in error). Must use for...in.

* **To iterate over objects, we use a `for...in` loop.**

![alt text](<Screenshot 2024-03-25 at 11.33.47 AM.png>)

In the above example, "singleKey" is a variable that will be assigned to each key on the "oobj" object. To access the key's value use the bracket notation.

* **if...in: determining if a key exists in an object**

* There are times where you'll want to check and see if a certain key exists in an object. For this use an if...in statement.

The structure for the command is: if ("key" in objectName){console.log("Message");}

    - If the key existis in the object, the command will ensue, in this case a console.log message. If requirements are not met, nothing will return.

![alt text](<Screenshot 2024-03-25 at 11.43.01 AM.png>)

Exercises:
![alt text](<Screenshot 2024-03-25 at 12.24.16 PM.png>)

Solution:
![alt text](<Screenshot 2024-03-25 at 12.24.42 PM.png>)

//don't really understand. get concept about ther ${} annotation, but had trouble recalling/applying.

### **Exercises**
  
![alt text](<Screenshot 2024-03-25 at 1.15.09 PM.png>)

1. programming.languages.push("Go);
2. programming.difficulty = "7";
3. delete programming.jokes;
4. programming.isFun = true;
5. ![alt text](<Screenshot 2024-03-25 at 1.18.17 PM.png>)
6. ![alt text](<Screenshot 2024-03-25 at 1.18.32 PM.png>)
7. ![alt text](<Screenshot 2024-03-25 at 1.19.58 PM.png>)
