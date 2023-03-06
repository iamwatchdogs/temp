# Q1(a): Distinguish between Java and JavaScript?

Although Java and JavaScript share a similar name, they are two completely different programming languages. Here are some of the main differences between Java and JavaScript:

1.  **Purpose:** 
Java is a general-purpose programming language used for building standalone applications, web applications, and enterprise-level applications. On the other hand, JavaScript is a client-side scripting language used for creating interactive web applications that run inside a web browser.
    
2.  **Syntax:** 
Java and JavaScript have different syntaxes. Java uses curly braces and semicolons to define code blocks and statements, whereas JavaScript uses curly braces and optional semicolons. Java is a strongly-typed language, which means that variables must be declared with their data types, while JavaScript is a loosely-typed language, where variables do not need to be declared with a specific data type.
    
3.  **Execution:** 
Java is compiled to bytecode and executed on the Java Virtual Machine (JVM), while JavaScript is interpreted and executed by a web browser's JavaScript engine.
    
4.  **Libraries and frameworks:** 
Both Java and JavaScript have a wide range of libraries and frameworks to choose from. Java has many popular frameworks for building web applications, such as Spring, Hibernate, and Struts, while JavaScript has many popular libraries and frameworks for client-side web development, such as React, Angular, and Vue.js.
    
5.  **Community:** 
Both Java and JavaScript have large and active communities of developers. However, Java has been around for much longer and has a more mature community, while JavaScript has seen rapid growth in recent years and has a very active and dynamic community.
    
In summary, Java and JavaScript are two distinct programming languages with different syntaxes, purposes, and execution environments. While they may share some similarities, they are used for different types of applications and have different strengths and weaknesses.

# Q1(b):  Explain keywords and operators supported by javascript.

Keywords and operators are two fundamental components of the JavaScript programming language. Here's an overview of keywords and operators in JavaScript:

Keywords: Keywords are reserved words in the JavaScript language that have a special meaning and cannot be used as identifiers (such as variable or function names). Here are some of the most common keywords in JavaScript:

*   `const`: declares a constant variable that cannot be reassigned a new value
*   `let`: declares a block-scoped variable that can be reassigned a new value
*   `var`: declares a variable with function scope (older way of declaring variables in JavaScript)
*   `function`: declares a function
*   `return`: specifies the value that a function should return
*   `if/else`: used for conditional statements
*   `switch/case`: used for multi-way conditional statements
*   `for/while/do-while`: used for looping
*   `try/catch/finally`: used for error handling

Operators: Operators are symbols or keywords that perform operations on one or more operands (values or variables). Here are some of the most common operators in JavaScript:

*   Arithmetic operators: + (addition), - (subtraction), \* (multiplication), / (division), % (modulus)
*   Assignment operators: = (simple assignment), +=, -=, \*=, /=, %= (compound assignments)
*   Comparison operators: == (equality), != (inequality), === (strict equality), !== (strict inequality), > (greater than), < (less than), >= (greater than or equal to), <= (less than or equal to)
*   Logical operators: && (logical AND), || (logical OR), ! (logical NOT)
*   Bitwise operators: & (bitwise AND), | (bitwise OR), ^ (bitwise XOR), ~ (bitwise NOT), << (left shift), >> (right shift)
*   Unary operators: + (unary plus), - (unary minus), ++ (increment), -- (decrement)
*   Ternary operator: ?: (conditional operator)

These are just a few examples of the many keywords and operators supported by JavaScript. Understanding these keywords and operators is essential to writing effective JavaScript code.

<br/>

# Q2(a):  Define local and global variables.

In JavaScript, variables can have either local or global scope.

Local Variables: A local variable is a variable declared inside a function or a block. It is only accessible within the function or block in which it is declared. Local variables are created when a function or block is executed and destroyed when the function or block completes. Here's an example of a local variable in JavaScript:

```js
function myFunction() {
  let x = 10; // x is a local variable
  console.log(x);
}
myFunction(); // output: 10
console.log(x); // output: Uncaught ReferenceError: x is not defined
```

In this example, the variable `x` is declared inside the `myFunction()` function and can only be accessed within the function. When the function is executed, `x` is assigned the value of 10 and then printed to the console. Outside of the function, `x` is not defined and trying to access it will result in a reference error.

Global Variables: A global variable is a variable declared outside a function or block. It is accessible throughout the entire program, including any functions or blocks. Global variables are created when the program starts and are destroyed when the program terminates. Here's an example of a global variable in JavaScript:


```js
let y = 20; // y is a global variable
function myFunction() {
  console.log(y);
}
myFunction(); // output: 20
console.log(y); // output: 20
```

In this example, the variable `y` is declared outside the `myFunction()` function and can be accessed within the function and outside of it. When the function is executed, `y` is printed to the console with a value of 20. Outside of the function, `y` is also 20 and can be accessed and manipulated throughout the entire program.

It's important to use local and global variables appropriately in order to avoid naming conflicts and unintended consequences.

# Q2(b): Explain variables and control structures in Java script.

Variables and control structures are two fundamental concepts in JavaScript. Here's an overview of what they are:

Variables: A variable is a container that holds a value. In JavaScript, variables can be declared using the keywords `let`, `const`, or `var`. Here's an example of how to declare a variable in JavaScript:

```javascript
let x = 5; // x is a variable that holds the value 5
const y = "Hello"; // y is a variable that holds the string "Hello"
var z = true; // z is a variable that holds the boolean value true
```

In this example, the `let`, `const`, and `var` keywords are used to declare variables with different data types (number, string, and boolean). Once a variable is declared, its value can be accessed, updated, or reassigned throughout the program.

Control Structures: Control structures are used to control the flow of execution in a program. In JavaScript, there are several types of control structures, including:

*   Conditional statements: `if`, `else if`, `else`, and the ternary operator (`?:`) are used to execute different blocks of code depending on certain conditions.
*   Loops: `for`, `while`, and `do...while` are used to execute a block of code multiple times until a certain condition is met.
*   Switch statements: `switch` and `case` are used to execute different blocks of code depending on the value of a variable or expression.

Here's an example of how to use a conditional statement in JavaScript:

```javascript
let age = 25;
if (age >= 18) {
  console.log("You are an adult");
} else {
  console.log("You are not an adult");
}
```

In this example, the `if` statement checks if the `age` variable is greater than or equal to 18. If it is, the program prints "You are an adult" to the console. Otherwise, it prints "You are not an adult".

Overall, variables and control structures are essential components of JavaScript programming that allow for dynamic and flexible programming.

<br/>

# Q3(a): What is Date object? How it is manipulated? Enter your DOB and find the age.

The `Date` object in JavaScript is a built-in object that represents a date and time. It provides methods to get and set various properties of a date, such as the year, month, day, hour, minute, second, and millisecond.

To create a new `Date` object in JavaScript, you can use the `new` keyword followed by the `Date()` constructor function. Here's an example of how to create a `Date` object representing the current date and time:

```javascript
let currentDate = new Date();
console.log(currentDate); // output: Sat Mar 06 2023 11:09:56 GMT-0500 (Eastern Standard Time)
```

Once you have a `Date` object, you can manipulate its properties using various methods. For example, you can get the year of a date using the `getFullYear()` method:

```javascript
let year = currentDate.getFullYear();
console.log(year); // output: 2023
```

You can also set the year of a date using the `setFullYear()` method:

```javascript
currentDate.setFullYear(2022);
console.log(currentDate); // output: Fri Mar 06 2022 11:09:56 GMT-0500 (Eastern Standard Time)
```

To find your age based on your date of birth (DOB), you can create two `Date` objects - one for your DOB and one for the current date - and then calculate the difference between them in years. Here's an example of how to do that:

```javascript
let dob = new Date("1990-01-01"); // replace with your own DOB
let today = new Date();
let ageInMilliseconds = today - dob;
let ageInYears = ageInMilliseconds / (1000 * 60 * 60 * 24 * 365.25); // 1 year = 365.25 days
console.log(ageInYears); // output: your age in years based on your DOB
```

In this example, the `new Date()` constructor is used to create a `Date` object representing your DOB, and another one representing the current date. The difference between the two dates is calculated in milliseconds using the subtraction operator, and then converted to years using the formula `(milliseconds / (1000 * 60 * 60 * 24 * 365.25))`, where 1 year is equal to 365.25 days on average. The result is your age in years based on your DOB.

# Q3(b): What is array? How to define array is JavaScript?

An array is a data structure in JavaScript that stores a collection of values of any data type (such as numbers, strings, or objects) in a single variable. The values in an array are indexed, which means they can be accessed and manipulated using their position in the array.

To define an array in JavaScript, you can use the `[]` brackets and separate the values with commas. Here's an example of an array that stores some numbers:

```javascript
let numbers = [1, 2, 3, 4, 5];
```

In this example, the `numbers` array stores the values 1, 2, 3, 4, and 5. You can access individual elements of an array using their index, which starts at 0 for the first element. For example, to access the first element of the `numbers` array, you would use `numbers[0]`.

Arrays in JavaScript are dynamic, which means you can add or remove elements from them at any time using various methods. For example, you can add elements to the end of an array using the `push()` method:

```javascript
numbers.push(6);
```

In this example, the `push()` method adds the value 6 to the end of the `numbers` array. You can also remove elements from an array using the `pop()` method, which removes the last element:

```javascript
numbers.pop();
```

In this example, the `pop()` method removes the value 6 from the end of the `numbers` array.

Overall, arrays are a powerful and flexible data structure in JavaScript that allow you to store and manipulate collections of values in a single variable.

<br/>

# Q4(a): Write a javascript program that asks the user to enter two numbers, obtains the two numbers from the user and outputs text that displays the sum, product, difference and quotient of the two numbers.

Here's a JavaScript program that asks the user to enter two numbers, obtains the numbers from the user using the `prompt()` function, and outputs text that displays the sum, product, difference, and quotient of the two numbers:

```javascript
let num1 = prompt("Enter the first number:");
let num2 = prompt("Enter the second number:");

num1 = parseFloat(num1); // convert to a number
num2 = parseFloat(num2); // convert to a number

let sum = num1 + num2;
let product = num1 * num2;
let difference = num1 - num2;
let quotient = num1 / num2;

let output = "The sum of " + num1 + " and " + num2 + " is " + sum + "\n" +
             "The product of " + num1 + " and " + num2 + " is " + product + "\n" +
             "The difference between " + num1 + " and " + num2 + " is " + difference + "\n" +
             "The quotient of " + num1 + " and " + num2 + " is " + quotient;

alert(output);
```

In this program, the `prompt()` function is used to obtain the two numbers from the user as strings. The `parseFloat()` function is then used to convert the strings to numbers.

The program then calculates the sum, product, difference, and quotient of the two numbers using basic arithmetic operators (`+`, `*`, `-`, and `/`). The results are stored in the `sum`, `product`, `difference`, and `quotient` variables, respectively.

Finally, the program creates a string using the `+` operator and the results, and displays the string using the `alert()` function. The `\n` character is used to create line breaks in the output string.

# Q4(b):  Explain properties of document object.

In JavaScript, the `document` object represents the current web page that is being displayed in the browser. It provides a wide range of properties and methods that allow you to manipulate the content and behavior of the web page.

Here are some common properties of the `document` object:

1.  `document.title`: This property gets or sets the title of the web page that is displayed in the browser's title bar.
    
2.  `document.body`: This property gets the `<body>` element of the web page, which is the main content area.
    
3.  `document.cookie`: This property gets or sets the cookies associated with the web page.
    
4.  `document.URL`: This property gets the URL of the current web page.
    
5.  `document.referrer`: This property gets the URL of the web page that referred the user to the current web page.
    
6.  `document.forms`: This property gets a collection of all the `<form>` elements on the web page.
    
7.  `document.images`: This property gets a collection of all the `<img>` elements on the web page.
    
8.  `document.links`: This property gets a collection of all the `<a>` elements on the web page that have a `href` attribute.
    
9.  `document.scripts`: This property gets a collection of all the `<script>` elements on the web page.
    
10.  `document.documentElement`: This property gets the root element of the web page, which is typically the `<html>` element.
    

These properties, along with many others, allow you to access and manipulate various aspects of the web page, such as its content, structure, and behavior.

<br/>

# Q5(a): What is function? Define a printName() function that takes string and a number N as arguments and prints the string N times

In JavaScript, a function is a block of code that performs a specific task or set of tasks. A function is defined using the `function` keyword, followed by the function name, a set of parentheses containing zero or more parameters (arguments), and a block of code that is executed when the function is called.

Here's an example of a `printName()` function that takes a string and a number `N` as arguments and prints the string `N` times:

```javascript
function printName(name, N) {
  for (let i = 0; i < N; i++) {
    console.log(name);
  }
}
```

In this example, the function `printName()` is defined with two parameters: `name` and `N`. The function uses a `for` loop to print the `name` parameter `N` times using the `console.log()` method.

To call the `printName()` function and pass it arguments, you can simply use the function name followed by a set of parentheses containing the argument values:

```javascript
printName("John", 5); // prints "John" five times
```

In this example, the `printName()` function is called with the arguments `"John"` and `5`, which causes it to print the string `"John"` five times using the `console.log()` method.

# Q5(b): Explain various string methods in Java script.

In JavaScript, there are many built-in methods for working with strings. Here are some of the most commonly used methods:

1.  `charAt(index)` - Returns the character at the specified index of a string.
2.  `concat(str1, str2, ..., strX)` - Concatenates two or more strings and returns the result.
3.  `indexOf(searchValue, startIndex)` - Searches a string for a specified value and returns the position of the first occurrence, or -1 if the value is not found.
4.  `lastIndexOf(searchValue, endIndex)` - Searches a string for a specified value and returns the position of the last occurrence, or -1 if the value is not found.
5.  `replace(searchValue, replaceValue)` - Searches a string for a specified value, and replaces it with another value or a regular expression pattern.
6.  `slice(startIndex, endIndex)` - Extracts a part of a string and returns a new string.
7.  `substring(startIndex, endIndex)` - Extracts the characters from a string, between two specified indices, and returns a new string.
8.  `toLowerCase()` - Converts a string to lowercase letters.
9.  `toUpperCase()` - Converts a string to uppercase letters.
10.  `trim()` - Removes whitespace from both ends of a string.
11.  `split(separator, limit)` - Splits a string into an array of substrings based on a specified separator and returns the result.
12.  `charAt()` - Returns the character at a specified index in a string.
13.  `startsWith()` - Returns true if a string starts with a specified character(s) or substring.
14.  `endsWith()` - Returns true if a string ends with a specified character(s) or substring.
15.  `includes()` - Returns true if a string contains a specified character(s) or substring.

These are just a few of the many methods available for working with strings in JavaScript. By combining these methods and using them in creative ways, you can manipulate and transform strings in a variety of ways to meet your programming needs.

<br/>

# Q6(a): Explain objects and constructors in Java script.

In JavaScript, objects are complex data structures that can contain properties and methods. An object is created by defining a set of key-value pairs within curly braces `{}`, where the keys are property names and the values are property values.

Here's an example of an object with two properties:

```javascript
let person = {
  name: "John",
  age: 30
};
```

In this example, the object `person` has two properties: `name` and `age`. The `name` property has the value `"John"`, and the `age` property has the value `30`.

Constructors in JavaScript are special functions that are used to create objects of a certain type. Constructors are defined using the `function` keyword, and they typically take one or more parameters that are used to set the initial properties of the object.

Here's an example of a constructor function that creates `Person` objects:

```javascript
function Person(name, age) {
  this.name = name;
  this.age = age;
}
```

In this example, the `Person` constructor takes two parameters: `name` and `age`. The constructor sets the `name` and `age` properties of the `Person` object using the `this` keyword.

To create a `Person` object using the constructor, you can use the `new` keyword followed by the constructor function name:

```javascript
let john = new Person("John", 30);
```

In this example, a new `Person` object is created with the name `"John"` and the age `30`. The `john` variable now points to the new `Person` object, which has the `name` and `age` properties set to `"John"` and `30`, respectively.

<br/>

# Q6(b): Write a Java Script code to generate the current date in words format “Day, Month Date, Year”. *(Hint: Monday, November 04, 2021)*

Here's a JavaScript code that generates the current date in the format "Day, Month Date, Year":

```javascript
let daysOfWeek = ["Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday"];
let monthsOfYear = ["January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"];

let currentDate = new Date();
let dayOfWeek = daysOfWeek[currentDate.getDay()];
let monthOfYear = monthsOfYear[currentDate.getMonth()];
let date = currentDate.getDate();
let year = currentDate.getFullYear();

let formattedDate = dayOfWeek + ", " + monthOfYear + " " + date + ", " + year;

console.log(formattedDate);
```

In this code, we first define two arrays: `daysOfWeek` and `monthsOfYear`, which contain the names of the days of the week and the months of the year, respectively.

Next, we create a new `Date` object using the `Date()` constructor. This creates a `Date` object that represents the current date and time.

We then use the `getDay()`, `getMonth()`, `getDate()`, and `getFullYear()` methods of the `Date` object to retrieve the day of the week, month, date, and year components of the current date.

Finally, we format the date string using string concatenation and print it to the console using the `console.log()` method. The output should be in the format "Day, Month Date, Year", like "Saturday, March 6, 2023".

<br/>

# Q7(a): Write a function findLongestWord() that takes a string of words and returns the longest word in that string?

Here's a JavaScript function `findLongestWord()` that takes a string of words and returns the longest word in that string:

```javascript
function findLongestWord(str) {
  let words = str.split(" ");
  let longestWord = "";
  
  for (let i = 0; i < words.length; i++) {
    if (words[i].length > longestWord.length) {
      longestWord = words[i];
    }
  }
  
  return longestWord;
}
```

In this function, we first use the `split()` method to split the input string `str` into an array of words, using a space character as the delimiter.

We then define a variable `longestWord` and initialize it to an empty string.

Next, we use a `for` loop to iterate through the words in the array. For each word, we check if its length is greater than the length of the current `longestWord`. If it is, we update the `longestWord` variable to the current word.

Finally, we return the `longestWord` variable, which contains the longest word in the input string.

For example, if we call the function with the input string `"The quick brown fox jumped over the lazy dog"`, the function will return the string `"jumped"`, since `"jumped"` is the longest word in the input string.

# Q7(b):  What is DHTML? How it is implemented?

DHTML stands for Dynamic HTML, which refers to a combination of technologies used to create dynamic and interactive web pages. DHTML typically includes HTML, CSS, and JavaScript, which are used together to create web pages that can respond to user actions and events, and dynamically update their content without requiring a full page reload.

DHTML is implemented using a combination of HTML, CSS, and JavaScript. HTML provides the basic structure and content of the page, while CSS is used to style the page and control its layout. JavaScript is used to add interactivity and dynamic behavior to the page, allowing it to respond to user actions and update its content without requiring a full page reload.

Some common examples of DHTML techniques include:

*   Dynamic menus and navigation bars that expand or collapse when the user clicks on them.
*   Image galleries and slideshows that allow the user to navigate through a series of images without reloading the page.
*   Interactive forms that validate user input and provide feedback without requiring a page reload.
*   Drag-and-drop interfaces that allow the user to drag elements around the page and rearrange them dynamically.

DHTML has largely been replaced by more modern web technologies like AJAX, which allow for even more dynamic and interactive web applications. However, many of the principles and techniques of DHTML are still used today in modern web development.

<br/>

# Q8(a): What is Document object model? Discuss the various DOM methods used with JavaScript.

The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. Essentially, the DOM provides a tree-like structure of the HTML elements on a web page that can be accessed and manipulated using JavaScript.

The DOM consists of a hierarchy of objects, each representing an element on the web page. These objects have properties that can be read and set using JavaScript, as well as methods that can be called to manipulate the elements and their attributes.

Some of the common DOM methods used with JavaScript include:

*   `getElementById()`: Retrieves an element on the page with a specific ID attribute.
*   `getElementsByTagName()`: Retrieves a collection of elements on the page with a specific tag name.
*   `getElementsByClassName()`: Retrieves a collection of elements on the page with a specific class name.
*   `createElement()`: Creates a new element on the page with a specified tag name.
*   `appendChild()`: Adds a new child element to an existing element on the page.
*   `removeChild()`: Removes a child element from an existing element on the page.
*   `setAttribute()`: Sets the value of an attribute on an element.
*   `getAttribute()`: Retrieves the value of an attribute on an element.

Using these and other DOM methods, you can manipulate the content and structure of a web page using JavaScript. For example, you can add new elements to the page, modify the contents of existing elements, and change the styles and attributes of elements based on user interactions or other events. The DOM provides a powerful interface for creating dynamic and interactive web pages.

# Q8(b): Define two arrays and join the arrays and display in sorted order.

Sure, here's an example JavaScript code to define two arrays, join them, and display the result in sorted order:

```javascript
// Define two arrays
const array1 = [4, 2, 8, 1, 5];
const array2 = [7, 6, 3, 9];

// Join the arrays
const joinedArray = array1.concat(array2);

// Sort the joined array
joinedArray.sort((a, b) => a - b);

// Display the sorted array
console.log(joinedArray);
```

In this example, we define two arrays `array1` and `array2`. We then join them using the `concat()` method, which creates a new array containing all the elements from both arrays in the order they were specified.

We then use the `sort()` method to sort the elements of the `joinedArray` in ascending order. Finally, we display the sorted array using the `console.log()` method.

Note that the `sort()` method sorts the array in place, meaning it modifies the original array rather than creating a new one. If you want to keep the original arrays unchanged, you should create a copy of them before joining them and sorting the result.

<br/>

# Q9(a): What is pattern matching object? Explain briefly.

In JavaScript, pattern matching is a technique for testing whether a value matches a particular pattern or structure. The Pattern Matching Object (PMO) is an experimental feature in JavaScript that provides a syntax for defining and using patterns in your code.

The PMO provides a way to match values against patterns using the `match()` method, which takes a pattern as an argument and returns an object that represents the matched value. The pattern can be any valid JavaScript expression that returns a value.

Here's an example of using the PMO to match a value against a pattern:

```javascript
const person = { name: "John", age: 30, email: "john@example.com" };

const result = person.match({ name: String, age: Number });

console.log(result); // { name: "John", age: 30 }
```

In this example, we define an object `person` with properties for `name`, `age`, and `email`. We then use the `match()` method to match the `person` object against a pattern that specifies the `name` property should be a `String` and the `age` property should be a `Number`.

The `match()` method returns an object that contains the properties that matched the pattern, in this case `{ name: "John", age: 30 }`. The `email` property is ignored because it doesn't match the pattern.

Note that the PMO is an experimental feature and is not yet part of the JavaScript standard. It is currently supported in some modern web browsers and can be used with the help of third-party libraries or polyfills.

# Q9(b): What do you mean by validation? How the Javascript validate the E-mail?

Validation refers to the process of checking whether input data meets certain requirements or constraints. Email validation is a common use case for validation, where we need to check whether an email address entered by a user is in a valid format.

JavaScript provides various methods for email validation. One way to validate an email address using JavaScript is to use a regular expression (regex) pattern that matches valid email addresses. Here's an example of how to validate an email address using regex in JavaScript:

javascript

```javascript
function validateEmail(email) {
  const pattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
  return pattern.test(email);
}
```

In this example, we define a function `validateEmail()` that takes an email address as a parameter. We then define a regex pattern that matches valid email addresses. The pattern uses the `test()` method to test whether the email address matches the pattern and returns `true` or `false` accordingly.

The regex pattern `^[^\s@]+@[^\s@]+\.[^\s@]+$` matches the following format:

*   `^[^\s@]+`: The email address must start with one or more characters that are not whitespace or '@'.
*   `@`: The email address must contain an '@' symbol.
*   `[^\s@]+`: The domain name must contain one or more characters that are not whitespace or '@'.
*   `\.`: The domain name must contain a '.' character.
*   `[^\s@]+$`: The domain name must end with one or more characters that are not whitespace or '@'.

The `test()` method returns `true` if the email address matches the pattern and `false` otherwise. We can use this function to validate email addresses entered by users in a web form or other input fields.
