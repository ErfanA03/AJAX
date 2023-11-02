# AJAX
Demonstrates the use of AJAX (Asynchronous JavaScript and XML) to load content from an external source and update a specific part of the page without requiring a full page reload.
Here's a breakdown of what the code aims to do:

## HTML Structure:
The code provides a basic HTML structure.
It includes an external stylesheet "style.css" to style the page.
Within the div with a class of "main," there is a heading "Get The Latest Content" and a button with the text "Get Content" and the ID "btn_content." This button is used to trigger the AJAX request.

## JavaScript Code:
The JavaScript code is embedded within the HTML, just before the closing </div> tag.

### Step 1: Creating XMLHttpRequest Object:
It creates an XMLHttpRequest object named "ajax" to facilitate making asynchronous requests to the server.

### Step 2: Preparing the AJAX Request:
It configures the AJAX request by using the open method. The request is set to a GET request to the "content.html" file. This specifies the URL from which data will be fetched.

### Step 3: Defining the Response Callback:
An onreadystatechange event handler is defined. It listens for changes in the state of the AJAX request.
When the readyState of the request becomes 4 (indicating that the request is complete), it updates the content of the element with the ID "content" with the response received from the server (in this case, the content from "content.html").

### Step 4: Sending the AJAX Request:
The getContent function is defined, which is triggered when the "Get Content" button is clicked.
Inside this function, it sends the AJAX request to the server.
It also hides the "Get Content" button by changing its display style to 'none'.
