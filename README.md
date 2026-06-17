Task Manager Application

Project Overview

I have built a Task Manager Application using HTML, CSS and Vanilla JavaScript. The main goal of this project was to learn how the DOM works and how JavaScript can be used to create web applications without using any frameworks or libraries. In this Task Manager, users can add tasks, edit tasks, complete tasks, search tasks and delete tasks. It also has a mode feature, examples of event propagation and a section that explains the Browser Rendering Pipeline.

Features

* Add tasks to the Task Manager Application
* Edit existing tasks in the Task Manager Application
* Mark tasks as completed in the Task Manager Application
* Delete tasks from the Task Manager Application
* Search tasks in the Task Manager Application
* Clear all tasks from the Task Manager Application
* The Task Manager Application has counters for completed and pending tasks
* The Task Manager Application has a Dark Mode and Light Mode toggle
* The Task Manager Application supports Local Storage
* The Task Manager Application uses Event Delegation
* The Task Manager Application demonstrates Event Bubbling and Event Capturing
* The Task Manager Application explains the Browser Rendering Pipeline


Parsing
When a browser gets an HTML file, it starts reading the code line by line. This is called parsing. The browser looks at the HTML structure, understands the elements like headings, paragraphs, buttons, forms and divs.

Tokenization
Before creating the DOM Tree the browser breaks the HTML code into pieces called tokens.
For example:
```<h1>Hello</h1>```

The browser finds:
* The opening tag: h1
* The text content: Hello
* The closing tag: h1
These pieces are called tokens.


DOM Tree
After parsing and tokenization the browser creates a DOM Tree. The DOM Tree shows the HTML document as a tree structure.
Example:
HTML
|
Body
|
Div
|
Button

JavaScript can modify these elements through the DOM.


In the Task Manager Application, task cards are created dynamically using DOM methods like:

* createElement()
* createTextNode()
* append()
* appendChild()


CSSOM Tree
The browser reads the CSS file and creates another tree called the CSSOM Tree. The CSSOM Tree has all the style rules that need to be applied to the HTML elements.

Render Tree
The browser combines the DOM Tree and CSSOM Tree to create the Render Tree. The Render Tree only has the elements that need to be displayed on the screen. After the Render Tree is created the browser displays the webpage.
The flow is:
HTML
→ Parsing
→ Tokenization
→ DOM Tree
CSS
→ CSSOM Tree
DOM Tree + CSSOM Tree
→ Render Tree


Attributes vs Properties
Attributes are defined inside HTML.
Example:
```<input value="Task">```


Property:
input.value

Attribute:
input.getAttribute("value")

Here, in the above example, we can see the difference:
* input.value returns the value of the Task Manager Application input.
* getAttribute("value") returns the value written in the HTML of the Task Manager Application.

Event Bubbling
Event Bubbling means the event starts from the target element and moves upward through its parent elements.
Example order:
Child
→ Parent
→ Grandparent
The Task Manager Application demonstrates bubbling using elements and console logs.

Event Capturing
Event Capturing works in the opposite direction of event bubbling.
The event starts from the element and moves toward the target element.

Example order:

Grandparent
→ Parent
→ Child

This behavior is demonstrated using addEventListener() with the parameter set to true.


Event Delegation
Event Delegation means attaching an event listener to a parent element instead of attaching separate listeners to every child element. In the Task Manager Application one event listener is attached to the task container.
Using event.target, actions such as:
* Edit tasks
* Complete tasks
* Delete tasks
These are handled efficiently. This approach improves performance. Reduces code duplication.

Technologies Used
* HTML
* CSS
* JavaScript (Vanilla JavaScript)
* DOM API
* Local Storage

Conclusion:
This project helped me understand DOM manipulation, event handling, event propagation attributes vs properties and how browsers render web pages. It also gave me hands-on experience in building a real-world interactive application using only Vanilla JavaScript. 
