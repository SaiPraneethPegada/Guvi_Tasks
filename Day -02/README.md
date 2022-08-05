# Day_02_Task

## Write a blog on difference between Document and Window Object.

|Document							 	|	   Window						 |
|-----------------------------------------------------------------------|----------------------------------------------------------------|
|It represents any HTML document or web page that is loaded in the browser.		|It represents a browser window or frame that displays the contents of the webpage.|   
|It is loaded inside the window.							|It is the very first object that is loaded in the browser.|
|It is the object of window property.							|It is the object of the browser.|
|All the tags, elements with attributes in HTML are part of the document.		|Global objects, functions, and variables of JavaScript are members of the window object.|
|We can access the document from a window using the window.document			|We can access the window from the window only. i.e., window.window|
|The document is part of BOM (browser object model) and DOM (Document object model)	|The window is part of BOM, not DOM.|
|Properties of document objects such as title, body, cookies, etc. can also be accessed by a window like this window.document.title	|Properties of the window object cannot be accessed by the document object.
|syntax: document.propertyname;								|syntax: window.propertyname;|
|Example: document.title :  will return the title of the document			|Example:window.innerHeight : will return the height of the content area of the browser|

----

### Properties of Document:

> Syntax: document.property_name;
	
*Few property_name Examples:*
		
		- activeElement: It returns the currently active elements in the document.
		
		- body: It returns the contents of the body element.
		
		- cookie: It returns the cookie of the current document.
		
		- designMode: It is used to set documents as editable or read-only.
		
		- domain: It returns the domain name of the document server.
		
		- embeds: It returns the collection of all embedded elements.
		
		- URL: It returns the complete URL of the document.
		
		- forms: It returns all the elements of the form.
		
		- referrer: It returns the URI of the page that is linked to the current page.
		
		- scripts: It returns all script elements present in the document.



## Methods of Document:

> Syntax: document.method_name;
	
*Few method_name Examples:*
		
		- addEventListener(): It is used to attach an event handler to the specified element.
		
		- adoptNode(): It is used to adopt a node from another document and it returns a node object, representing the adopted node.
		
		- createComment(): It is used to create a comment node with some text.
		
		- createElement(): It is used to create HTML element .
		
		- createEvent(): It is used to create a new events object.
		
		- getElementById(): It returns the object of the given ID. If no object with that id exists then it returns null.
		
		- getElementsByClassName(): It returns an object containing all the elements with the specified class names in the document as objects.
		
		- getElementsByName(): It returns an object containing all the elements with the specified name in the document as objects.
		
		- getElementsByTagName(): It returns an object containing all the elements with the specified tag names in the document as objects.
		
		- querySelector(): It returns the first element that matches a specified CSS selector(s) in the document.
		
		- querySelectorAll(): It returns a collection of an element’s child elements that matches a specified CSS selector(s) in the document

----

## Properties of Window:

> Syntax: window.property_name;
	
*Few property_name Examples:*
		
		- console: It returns a reference to the console object which provides access to the browser’s debugging console.

		- defaultStatus: It is used to define the default message that will be displayed in 

		- Document : It returns a reference to the document object of that window.

		- History: It provides information on the URLs visited in the current window.

		- Length: It represents the number of frames in the current window.

		- Location: It contains the URL of the current window.

		- innerHeight: It is used to get the height of the content area of the browser window.

		- innerWidth: It is used to get the width of the content area of the browser window.

		- Navigator: It returns a reference to the navigator object.

		- outerHeight: It will get the height of the outside of the browser window.

		- outerWidth: It will get the width of the outside of the browser window.

		- Status: It overrides the default status and places a message in the status bar.

		- Toolbar: It will result in the toolbar object, whose visibility can be toggled in the window.




## Methods of Window:

> Syntax: window.method_name;

*Few method_name Examples:*
		
		- alert(): It is used to display an alert box. It displays a specified message along with an OK button and is generally used to make sure that the information comes through the user.
		
		- clearInterval(): It clears the interval which has been set by the setInterval() function before that.
		
		- clearTimeout(): It clears the timeout which has been set by the setTimeout()function before that.
		
		- close(): It is used for closing a certain window or tab of the browser which was previously opened.
		
		- confirm(): It is used to display a modal dialog with an optional message and two buttons i.e. OK and Cancel. It returns true if the user clicks “OK”, and false otherwise.
		
		- focus(): It is used to give focus to an element in the current window.
		
		- open(): It is used to open a new tab or window with the specified URL and name.
		
		- prompt(): It is used to display a dialog with an optional message prompting the user to input some text
		
		- setInterval(): It repeats a given function at every given time interval.
		
		- setTimeout(): It executes a function, after waiting a specified number of milliseconds.
		
