# Q1(a): Explain the classification of basic HTML tags with examples.

HTML (Hypertext Markup Language) is a markup language used for creating web pages. HTML tags are used to define the structure and content of a web page. There are many HTML tags available, but they can be classified into six basic types:

1.  Structural Tags: Structural tags define the basic structure of an HTML document. They include the <html>, <head>, and <body> tags.

Example:

```php
<!DOCTYPE html>
<html>
  <head>
    <title>My Web Page</title>
  </head>
  <body>
    <h1>Welcome to My Web Page</h1>
    <p>This is a paragraph of text.</p>
  </body>
</html>
```

2.  Heading Tags: Heading tags are used to create headings on a web page. They range from &lt;h1&gt; (the most important) to &lt;h6&gt; (the least important).

Example:

```css
<h1>Main Heading</h1>
<h2>Sub-Heading</h2>
<h3>Sub-Sub-Heading</h3>
```

3.  Paragraph Tags: Paragraph tags are used to create paragraphs of text.

Example:

```css
<p>This is a paragraph of text.</p>
```

4.  Link Tags: Link tags are used to create hyperlinks to other web pages or to other parts of the same web page.

Example:

```php
<a href="http://www.example.com">Link Text</a>
```

5.  Image Tags: Image tags are used to display images on a web page.

Example:
```php
<img src="image.jpg" alt="Image Description">
```

6.  List Tags: List tags are used to create ordered or unordered lists.

Example:

```css
<ul>
  <li>List Item 1</li>
  <li>List Item 2</li>
  <li>List Item 3</li>
</ul>

<ol>
  <li>List Item 1</li>
  <li>List Item 2</li>
  <li>List Item 3</li>
</ol>
```

These are the six basic types of HTML tags with examples. It's important to note that these tags can be used in combination with each other to create complex web pages.

# Q1(b): Distinguish <img> element and its attributes with suitable example.

The `<img>` element in HTML is used to embed an image in a web page. It is a self-closing tag, meaning it does not require a closing tag. The `<img>` element has several attributes that can be used to specify various properties of the image, such as its source, width, height, alt text, and more. Here's a brief explanation of some of the most commonly used attributes:

*   `src`: This attribute specifies the URL of the image file to be displayed. It is a required attribute.
*   `alt`: This attribute specifies the alternative text that should be displayed if the image cannot be displayed or if the user is using a screen reader.
*   `width` and `height`: These attributes specify the width and height of the image, in pixels or as a percentage of the container's width or height.
*   `title`: This attribute specifies additional information about the image that can be displayed as a tooltip when the user hovers over the image.

Example:

```css
<img src="image.jpg" alt="A beautiful sunset" width="800" height="600">
```

This code will display an image of a sunset with a width of 800 pixels and a height of 600 pixels. The `src` attribute specifies the URL of the image file, while the `alt` attribute provides a text description of the image. If the image cannot be displayed, the alternative text "A beautiful sunset" will be displayed instead.

<br/>
  
# Q2(a): Explain various attributes in &lt;a href> element with example

The `<a>` element in HTML is used to create hyperlinks that point to other web pages or resources. The `href` attribute is the most important attribute of the `<a>` element, as it specifies the URL of the page or resource that the hyperlink points to. Here are some of the other attributes that can be used with the `<a>` element:

*   `target`: This attribute specifies where to open the linked document. It can take one of several values, such as `_self` (the default), which opens the linked document in the same frame as the current document, or `_blank`, which opens the linked document in a new window or tab.
*   `rel`: This attribute specifies the relationship between the current document and the linked document. It is used for search engine optimization and security purposes. For example, you can use the `rel="nofollow"` attribute to tell search engines not to follow the link, or the `rel="noopener"` attribute to prevent the linked document from accessing the current document's window object.
*   `title`: This attribute specifies additional information about the linked document that can be displayed as a tooltip when the user hovers over the link.
*   `download`: This attribute specifies that the linked document should be downloaded instead of displayed in the browser. You can use this attribute to provide a link to a file download.
*   `type`: This attribute specifies the MIME type of the linked document. It is usually used for linked resources such as stylesheets or scripts.

Example:


```php
<a href="http://www.example.com" target="_blank" rel="noopener" title="Example Website">Visit Example Website</a>
```

This code will create a hyperlink that points to the "[http://www.example.com](http://www.example.com)" URL. The `target` attribute is set to `_blank`, which will open the linked document in a new window or tab. The `rel` attribute is set to `noopener`, which prevents the linked document from accessing the current document's window object. The `title` attribute specifies that the linked document is an "Example Website". Finally, the link text "Visit Example Website" is displayed to the user.

# Q2(b): Explain clearly about lists in HTML

In HTML, there are three types of lists that you can use to organize content: ordered lists, unordered lists, and definition lists.

1.  Ordered Lists (`<ol>`): An ordered list is a numbered list where each list item is marked with a number. You can use the `<ol>` tag to create an ordered list, and each list item is marked with the `<li>` tag.

Example:

```css
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```

2.  Unordered Lists (`<ul>`): An unordered list is a list of items that are marked with bullet points. You can use the `<ul>` tag to create an unordered list, and each list item is marked with the `<li>` tag.

Example:

```css
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ul>
```

3.  Definition Lists (`<dl>`): A definition list is a list of terms and their definitions. You can use the `<dl>` tag to create a definition list, and each term is marked with the `<dt>` tag, while the definition is marked with the `<dd>` tag.

Example:
```css
<dl>
  <dt>Term 1</dt>
  <dd>Definition 1</dd>
  <dt>Term 2</dt>
  <dd>Definition 2</dd>
  <dt>Term 3</dt>
  <dd>Definition 3</dd>
</dl>
```

Lists can be nested within each other, allowing you to create more complex structures. To nest a list, you simply create a new list inside a list item. For example:

```css
<ol>
  <li>First item</li>
  <li>Second item
    <ul>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ul>
  </li>
  <li>Third item</li>
</ol>
```

This creates an ordered list with three items, where the second item contains a nested unordered list with two subitems.

<br/>

# Q3(a): Explain `<frame>` element and its attributes with suitable example.

The `<frame>` element is used to divide a webpage into multiple sections, where each section can load a different webpage or document. This element is mostly used in conjunction with the `<frameset>` element to create framesets.

Here are some of the attributes that can be used with the `<frame>` element:

*   `src`: This attribute specifies the URL of the webpage or document to be displayed in the frame.
*   `name`: This attribute specifies a name for the frame. This name can be used as the target for hyperlinks or form submissions that should be displayed in the frame.
*   `scrolling`: This attribute specifies whether or not to display scrollbars in the frame. It can take one of three values: `yes` (to display scrollbars), `no` (to hide scrollbars), or `auto` (to display scrollbars only if necessary).
*   `frameborder`: This attribute specifies whether or not to display a border around the frame. It can take one of two values: `1` (to display a border) or `0` (to hide the border).
*   `marginwidth` and `marginheight`: These attributes specify the width and height of the margin around the frame, respectively.
*   `noresize`: This attribute specifies whether or not to allow the user to resize the frame. It can take one of two values: `yes` (to allow resizing) or `no` (to prevent resizing).

Example:

```php
<frameset cols="25%,75%">
  <frame src="menu.html" name="menu" scrolling="yes" frameborder="1">
  <frame src="content.html" name="content" scrolling="yes" frameborder="1">
</frameset>
```

This code creates a frameset with two frames: one on the left that displays a menu and another on the right that displays content. The `cols` attribute of the `<frameset>` element specifies the width of each frame, where the first frame takes up 25% of the width and the second frame takes up 75% of the width. The `src` attribute of each `<frame>` element specifies the URL of the webpage or document to be displayed in the frame. The `name` attribute of each `<frame>` element specifies a name for the frame. The `scrolling` attribute of each `<frame>` element specifies that scrollbars should be displayed in the frame. The `frameborder` attribute of each `<frame>` element specifies that a border should be displayed around the frame.

# Q3(b): What is CSS? Explain the syntax and usage of CSS.

CSS stands for Cascading Style Sheets. It is a style sheet language used to describe the presentation of a document written in HTML or XML. CSS separates the presentation of a document from its content, making it possible to define a single set of styles that can be applied to multiple documents.

Syntax: The basic syntax of CSS consists of a selector and a declaration block. The selector identifies the HTML element to which the styles should be applied, while the declaration block contains one or more property-value pairs that define the styles.

```css
selector {
  property1: value1;
  property2: value2;
  ...
}
```

Example: Suppose you want to change the color of the text in all `<h1>` elements to red. You can use the following CSS code:

```css
h1 {
  color: red;
}
```

This code defines a selector (`h1`) and a declaration block that sets the `color` property to `red`.

Usage: There are three main ways to apply CSS to an HTML document:

1.  External CSS: In this method, you create a separate CSS file with all the styles defined in it, and link to this file from the HTML document using the `<link>` element in the `<head>` section.

Example:

```php
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  ...
</body>
</html>
```

2. Internal CSS: In this method, you define the styles within the `<style>` element in the `<head>` section of the HTML document.

Example:

```php
<!DOCTYPE html>
<html>
<head>
  <style>
    h1 {
      color: red;
    }
  </style>
</head>
<body>
  ...
</body>
</html>
```

3. Inline CSS: In this method, you define the styles directly within the HTML element using the `style` attribute.

Example:

```php
<!DOCTYPE html>
<html>
<head>
</head>
<body>
  <h1 style="color: red;">This is a heading</h1>
  ...
</body>
</html>
```

Inline CSS is not recommended for large-scale styling as it can make the HTML document harder to read and maintain. However, it can be useful for making small, one-time changes to the styles of specific elements.

<br/>  
  
# Q4(a): Demonstrate the table tags and its attributes briefly

Tables in HTML are created using the `<table>` element and its associated elements. Here are some of the most commonly used attributes of the `<table>` element:

*   `border`: This attribute specifies the width of the border around the table. It can take a value of `0` (no border) or a positive integer (the width of the border in pixels).
*   `cellspacing`: This attribute specifies the amount of space to be left between the cells in the table. It can take a value of `0` (no space) or a positive integer (the amount of space in pixels).
*   `cellpadding`: This attribute specifies the amount of space to be left between the cell content and the cell border. It can take a value of `0` (no space) or a positive integer (the amount of space in pixels).
*   `width`: This attribute specifies the width of the table. It can take a value of `100%` (to fill the width of the container element) or a positive integer (the width of the table in pixels).
*   `height`: This attribute specifies the height of the table. It can take a value of `100%` (to fill the height of the container element) or a positive integer (the height of the table in pixels).
*   `align`: This attribute specifies the horizontal alignment of the table within its container element. It can take a value of `left`, `center`, or `right`.
*   `bgcolor`: This attribute specifies the background color of the table. It can take any valid color value in CSS, such as `#ffffff` or `red`.

Example:
  
```php
<table border="1" cellspacing="0" cellpadding="5" width="100%">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>Country</th>
  </tr>
  <tr>
    <td>John Doe</td>
    <td>25</td>
    <td>USA</td>
  </tr>
  <tr>
    <td>Jane Smith</td>
    <td>32</td>
    <td>Canada</td>
  </tr>
</table>
```

This code creates a table with a border width of `1`, no spacing between cells, and a padding of `5` pixels. The table fills the entire width of its container element. The `<tr>` elements define rows in the table, while the `<th>` and `<td>` elements define headers and cells within the rows, respectively. The `align` attribute is not used in this example, but it could be added to align the table to the left, center, or right. The `bgcolor` attribute is also not used in this example, but it could be added to set the background color of the table.

# Q4(b): What are external CSS rules? How to import external CSS files?

External CSS rules are styles that are defined in a separate CSS file, rather than in the `<head>` section of an HTML document. By defining styles in a separate file, they can be easily reused across multiple pages on a website, making it easier to maintain a consistent visual style.

To import an external CSS file into an HTML document, you can use the `<link>` element in the `<head>` section of the HTML document. The `href` attribute specifies the URL of the external CSS file, while the `rel` attribute specifies the relationship between the HTML document and the CSS file. The `type` attribute specifies the MIME type of the linked document, which should be set to `text/css` for CSS files.

Here is an example of how to import an external CSS file:

```html
<head>
  <link rel="stylesheet" type="text/css" href="styles.css">
</head>
```

In this example, the `styles.css` file is located in the same directory as the HTML file. If the file were located in a different directory, you would need to specify the full path to the file in the `href` attribute.

Once the CSS file has been imported, you can define styles in the file using the same syntax as you would in the `<style>` section of an HTML document. For example:

```css
/* styles.css */
body {
  background-color: #f5f5f5;
  color: #333333;
}

h1, h2, h3 {
  font-family: Arial, sans-serif;
  font-weight: bold;
  color: #007bff;
}

p {
  font-family: Georgia, serif;
  font-size: 18px;
  line-height: 1.5;
}
```

In this example, the styles defined in `styles.css` will be applied to all pages that import the file. To make changes to the styles, you only need to edit the CSS file, rather than modifying each individual HTML file.

# Q5(a): Explain how Forms are created with an example.

HTML forms are used to collect data from users, such as contact information or search queries. Forms are created using the `<form>` element, and can contain a variety of input elements, such as text fields, checkboxes, radio buttons, and more.

Here is an example of how to create a simple form with two input fields and a submit button:

```php
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">

  <label for="email">Email:</label>
  <input type="email" id="email" name="email">

  <input type="submit" value="Submit">
</form>
```

In this example, the `<form>` element defines the boundaries of the form. The `for` attribute of the `<label>` element associates the label with the input field, allowing users to click on the label to focus on the corresponding input field. The `id` and `name` attributes of the `<input>` elements are used to identify the input fields, and can be used to access the values entered by the user using JavaScript.

The `type` attribute of the first `<input>` element is set to `text`, which creates a simple text field where users can enter their name. The `type` attribute of the second `<input>` element is set to `email`, which creates a field where users can enter their email address, and the browser will validate the input to ensure it is a valid email address.

The last `<input>` element is of type `submit`, which creates a button that users can click to submit the form. When the button is clicked, the form data is sent to the server specified by the `action` attribute of the `<form>` element. If the `action` attribute is not specified, the form data will be sent to the current page.

This is just a simple example of how forms can be created in HTML. Forms can be customized in a variety of ways, including adding more input elements, specifying validation rules, and using JavaScript to interact with the form data.

# Q5(b): Write a program to create an Indian flag.

Creating an Indian flag using frames in HTML (not HTML5) involves creating three different frames and setting the background colors of each frame to the appropriate colors of the Indian flag. Here's an example of how it can be done:

```php
<html>
  <head>
    <title>Indian Flag using Frames</title>
  </head>
  <frameset rows="50%,50%">
    <frameset cols="50%,50%">
      <frame src="red.html" name="redFrame">
      <frame src="white.html" name="whiteFrame">
    </frameset>
    <frame src="green.html" name="greenFrame">
  </frameset>
  <noframes>
    <body>
      <p>This page requires a frames-compatible browser.</p>
    </body>
  </noframes>
</html>
```

This code creates a frameset with two rows and two columns, which creates a total of three frames. The top left frame is set to the color red, the top right frame is set to the color white, and the bottom frame is set to the color green. Each frame is given a unique name so that they can be targeted individually with CSS or JavaScript.

To create the content of each frame, we need to create three separate HTML files (`red.html`, `white.html`, and `green.html`) and set the background color of each file to the corresponding color of the Indian flag. Here's an example of what the `red.html` file might look like:

```php
<html>
  <head>
    <title>Indian Flag - Red</title>
  </head>
  <body bgcolor="#FF9933">
  </body>
</html>
```

Similarly, we would create `white.html` and `green.html` files and set their background colors to white and green, respectively.

Once we have all three HTML files created, we can load the main HTML file in a web browser to see the Indian flag created using frames.

<br/>
  
# Q6(a): Explain briefly the form input tag controls with example

HTML provides a variety of input elements that can be used within a form to collect user input. Here are some of the most commonly used form input tags:

1.  `<input type="text">`: Creates a text field where users can enter a single line of text.

Example:

```html
<label for="name">Name:</label>
<input type="text" id="name" name="name">
```

2.  `<input type="email">`: Creates a text field where users can enter an email address. The browser will validate the input to ensure it is a valid email address.

Example:

```html
<label for="email">Email:</label>
<input type="email" id="email" name="email">
```

3.  `<input type="password">`: Creates a text field where users can enter a password. The text entered in the field is masked so that it is not visible to other users.

Example:

```html
<label for="password">Password:</label>
<input type="password" id="password" name="password">
```

4.  `<input type="checkbox">`: Creates a checkbox that users can select or deselect.

Example:

```html
<label for="subscribe">Subscribe to newsletter:</label>
<input type="checkbox" id="subscribe" name="subscribe" value="yes">
```

5.  `<input type="radio">`: Creates a radio button that users can select. Radio buttons are used when there are multiple options to choose from, but only one option can be selected.

Example:

```html
<label for="gender-male">Male</label>
<input type="radio" id="gender-male" name="gender" value="male">

<label for="gender-female">Female</label>
<input type="radio" id="gender-female" name="gender" value="female">
```

6.  `<select>` and `<option>`: Creates a dropdown menu where users can select one option from a list of options.

Example:

```html
<label for="country">Country:</label>
<select id="country" name="country">
  <option value="india">India</option>
  <option value="usa">USA</option>
  <option value="uk">UK</option>
</select>
```

These are just a few examples of the input tags available in HTML forms. Other input types include file uploads, hidden fields, date pickers, and more. By using a combination of input tags, developers can create powerful and flexible forms to collect data from users.

# Q6(b): What is difference between HTML and HTML5 input types?

HTML and HTML5 both provide a variety of input types that can be used within a form to collect user input. However, HTML5 introduces several new input types that were not available in previous versions of HTML. Here are some of the key differences between HTML and HTML5 input types:

1.  Date and time input types: HTML5 introduces new input types for collecting dates, times, and date/time combinations. These input types include `date`, `time`, `datetime-local`, and `month`, and they provide a more user-friendly way of collecting this type of data compared to using a text field.
    
2.  Email and URL input types: HTML5 provides input types specifically designed for collecting email addresses and URLs. These input types (`email` and `url`) can help to validate the user's input and provide a more user-friendly interface for entering this type of data.
    
3.  Color input type: HTML5 introduces a new input type (`color`) that allows users to select a color using a color picker.
    
4.  Range input type: HTML5 introduces a new input type (`range`) that allows users to select a value from a range using a slider. This is useful for collecting numeric values within a specific range.
    
5.  Search input type: HTML5 introduces a new input type (`search`) that provides a search box with built-in autocomplete suggestions.
    

Overall, HTML5 introduces several new input types that make it easier to collect specific types of data and provide a better user experience. However, it's important to note that not all browsers support all HTML5 input types, so developers may need to provide fallback options for older browsers or use JavaScript to provide a consistent user experience across all browsers.

<br/>
  
# Q7(a): Make use of the form tag to design a simple user registration form.

Sure! Here's an example of a simple user registration form using the HTML `<form>` tag:


```html
<!DOCTYPE html>
<html>
  <head>
    <title>User Registration Form</title>
  </head>
  <body>
    <h1>User Registration Form</h1>
    <form action="#" method="post">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name" required><br><br>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required><br><br>

      <label for="password">Password:</label>
      <input type="password" id="password" name="password" required><br><br>

      <label for="confirm_password">Confirm Password:</label>
      <input type="password" id="confirm_password" name="confirm_password" required><br><br>

      <label for="gender">Gender:</label>
      <input type="radio" id="male" name="gender" value="male" required>
      <label for="male">Male</label>
      <input type="radio" id="female" name="gender" value="female" required>
      <label for="female">Female</label><br><br>

      <label for="age">Age:</label>
      <input type="number" id="age" name="age" min="18" max="99" required><br><br>

      <input type="submit" value="Submit">
    </form>
  </body>
</html>
```

In this example, we use the `<form>` tag to create a form for users to register on our website. The `action` attribute specifies where the form data should be submitted (in this case, we use `#` to indicate that the data should be handled by JavaScript). The `method` attribute specifies whether the data should be submitted using the GET or POST method (in this case, we use `POST`).

Within the `<form>` tag, we use various input tags to collect user input, including `<input type="text">` for the user's name, `<input type="email">` for their email address, `<input type="password">` for their password, `<input type="radio">` for their gender, and `<input type="number">` for their age.

Note that we use the `required` attribute on each input tag to indicate that the field is required and cannot be left blank. We also use the `min` and `max` attributes on the age input tag to ensure that the user enters an age between 18 and 99.

Finally, we use the `<input type="submit">` tag to create a submit button that the user can click to submit their registration form.

# Q7(b): Display the user registration form with diagram

As an AI language model, I am not able to create a diagram. However, I can provide you with the HTML code for a basic user registration form with labels, text input fields, and a submit button. You can then view the form in a web browser to see how it looks visually.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>User Registration Form</title>
  </head>
  <body>
    <h1>User Registration Form</h1>
    <form action="#" method="post">
      <label for="name">Name:</label>
      <input type="text" id="name" name="name"><br><br>

      <label for="email">Email:</label>
      <input type="email" id="email" name="email"><br><br>

      <label for="password">Password:</label>
      <input type="password" id="password" name="password"><br><br>

      <label for="confirm_password">Confirm Password:</label>
      <input type="password" id="confirm_password" name="confirm_password"><br><br>

      <label for="gender">Gender:</label>
      <input type="radio" id="male" name="gender" value="male">
      <label for="male">Male</label>
      <input type="radio" id="female" name="gender" value="female">
      <label for="female">Female</label><br><br>

      <label for="age">Age:</label>
      <input type="number" id="age" name="age"><br><br>

      <input type="submit" value="Submit">
    </form>
  </body>
</html>
```

This form includes text input fields for the user's name, email, and password, as well as radio buttons for their gender and a number input field for their age. The form also includes a submit button that the user can click to submit their registration information. You can view the form in a web browser to see how it looks visually.

<div align="center">
  
![image](https://user-images.githubusercontent.com/49478000/223190779-75795e5d-32a1-4fc2-b4f6-980deb321501.png)

</div>

<br/>
  
# Q8(a): Create a time table with 6-week days and five periods a day using HTML table tags.

Sure, here is an example of a time table with 6-week days and five periods a day using HTML table tags:


```html
<!DOCTYPE html>
<html>
<head>
	<title>Time Table</title>
</head>
<body>
	<table border="1">
		<tr>
			<th>Day</th>
			<th>Period 1</th>
			<th>Period 2</th>
			<th>Period 3</th>
			<th>Period 4</th>
			<th>Period 5</th>
		</tr>
		<tr>
			<td>Monday</td>
			<td>Mathematics</td>
			<td>English</td>
			<td>Science</td>
			<td>Social Studies</td>
			<td>Art</td>
		</tr>
		<tr>
			<td>Tuesday</td>
			<td>English</td>
			<td>Mathematics</td>
			<td>Social Studies</td>
			<td>Science</td>
			<td>Physical Education</td>
		</tr>
		<tr>
			<td>Wednesday</td>
			<td>Science</td>
			<td>Art</td>
			<td>Mathematics</td>
			<td>English</td>
			<td>Social Studies</td>
		</tr>
		<tr>
			<td>Thursday</td>
			<td>Social Studies</td>
			<td>Physical Education</td>
			<td>English</td>
			<td>Mathematics</td>
			<td>Science</td>
		</tr>
		<tr>
			<td>Friday</td>
			<td>Art</td>
			<td>Social Studies</td>
			<td>Physical Education</td>
			<td>Mathematics</td>
			<td>English</td>
		</tr>
		<tr>
			<td>Saturday</td>
			<td>Physical Education</td>
			<td>Science</td>
			<td>Art</td>
			<td>English</td>
			<td>Mathematics</td>
		</tr>
	</table>
</body>
</html>
```

This table includes six rows, one for each day of the week, and six columns, one for the day name and five for each period of the day. The table also includes a header row that displays the column titles. Each cell in the table contains a class subject for that day and period. You can customize this table to fit your needs by changing the subject names and other details.

# Q8(b): Organize the table.

Sure, here's an organized version of the table with a bit of added styling for readability:

```css
<!DOCTYPE html>
<html>
<head>
	<title>Time Table</title>
	<style>
		table {
			border-collapse: collapse;
			width: 100%;
		}
		th, td {
			padding: 8px;
			text-align: center;
			border: 1px solid black;
		}
		th {
			background-color: #ddd;
		}
		tr:nth-child(even) {
			background-color: #f2f2f2;
		}
	</style>
</head>
<body>
	<table>
		<tr>
			<th>Day</th>
			<th>Period 1</th>
			<th>Period 2</th>
			<th>Period 3</th>
			<th>Period 4</th>
			<th>Period 5</th>
		</tr>
		<tr>
			<td>Monday</td>
			<td>Mathematics</td>
			<td>English</td>
			<td>Science</td>
			<td>Social Studies</td>
			<td>Art</td>
		</tr>
		<tr>
			<td>Tuesday</td>
			<td>English</td>
			<td>Mathematics</td>
			<td>Social Studies</td>
			<td>Science</td>
			<td>Physical Education</td>
		</tr>
		<tr>
			<td>Wednesday</td>
			<td>Science</td>
			<td>Art</td>
			<td>Mathematics</td>
			<td>English</td>
			<td>Social Studies</td>
		</tr>
		<tr>
			<td>Thursday</td>
			<td>Social Studies</td>
			<td>Physical Education</td>
			<td>English</td>
			<td>Mathematics</td>
			<td>Science</td>
		</tr>
		<tr>
			<td>Friday</td>
			<td>Art</td>
			<td>Social Studies</td>
			<td>Physical Education</td>
			<td>Mathematics</td>
			<td>English</td>
		</tr>
		<tr>
			<td>Saturday</td>
			<td>Physical Education</td>
			<td>Science</td>
			<td>Art</td>
			<td>English</td>
			<td>Mathematics</td>
		</tr>
	</table>
</body>
</html>
```

In this version, the table is styled using CSS to have a collapsed border, centered text, and alternating row colors. The table also expands to 100% of its parent container, so it will adjust to fit the available space.

<br/>
  
# Q9(a): Create a login form with required elements

Sure, here's an example of a login form with required elements such as username and password fields and a submit button:


```html
<!DOCTYPE html>
<html>
<head>
	<title>Login Form</title>
</head>
<body>
	<h2>Login</h2>
	<form action="" method="post">
		<label for="username">Username:</label>
		<input type="text" id="username" name="username" required><br><br>
		<label for="password">Password:</label>
		<input type="password" id="password" name="password" required><br><br>
		<input type="submit" value="Login">
	</form>
</body>
</html>
```

This form includes two input fields, one for the username and one for the password, both of which are required using the `required` attribute. When the form is submitted, it will send the entered data to the server using the `POST` method, which can then be processed by server-side code.

# Q9(b): Define <div> and <span> tags with suitable example.

Both `<div>` and `<span>` tags are used in HTML to create containers that can be used for grouping and styling content.

The `<div>` tag is a block-level element that is typically used to group larger sections of content, such as a group of related elements or a section of a web page. It can be used to apply CSS styles to multiple elements at once by wrapping them in a `<div>` container. Here's an example:


```css
<div>
  <h2>Heading</h2>
  <p>This is some paragraph text.</p>
  <ul>
    <li>List item 1</li>
    <li>List item 2</li>
    <li>List item 3</li>
  </ul>
</div>
```

In this example, the `<div>` element is used to group together a heading, a paragraph, and an unordered list, which can then be styled using CSS.

On the other hand, the `<span>` tag is an inline-level element that is typically used for grouping smaller sections of content, such as a single word or phrase. It can also be used to apply CSS styles to specific parts of an element's content. Here's an example:

css

```css
<p>This is some <span>highlighted</span> text.</p>
```

In this example, the `<span>` element is used to wrap the word "highlighted", which can then be styled using CSS to apply a different color or font style.
