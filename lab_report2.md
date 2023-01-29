# Lab Report 2

## Servers and Bugs

**StringServer**

<img width="629" alt="Screen Shot 2023-01-29 at 12 24 06 PM" src="https://user-images.githubusercontent.com/122562580/215353919-e23daa83-2e8d-4f88-9aa6-cd6b069e8560.png">

**First Added Message:**
<img width="1031" alt="Screen Shot 2023-01-29 at 12 26 54 PM" src="https://user-images.githubusercontent.com/122562580/215354100-5203a155-98d2-4645-b86e-61a169269505.png">

In order for this first string to display, the **handleRequest** method in the handling class is called. This method has a URI parameter which takes in a URL as its argument. In this instance the URL is `http://localhost:4000/add-message?s=FirstString!`. Along with this, an empty string called `list` is instantiated in order to store the relevant strings from the URL query.

Once this method is called it checks the path of URI parameter. If the paramter is equal to "/add-message" the method will then instantiate a String array that separates the query into two parts at the equal sign. If the first parameter is equal to "s" the handleRequests method will concatenate the second paramter to the empty string followed by a new line separator. Once this is complete the string value is updated to contain the first message and is then returned in order to display on the webpage.

**Second Added Message**
<img width="1042" alt="Screen Shot 2023-01-29 at 12 27 38 PM" src="https://user-images.githubusercontent.com/122562580/215354860-0c9eea3f-fedc-417a-a453-5eab6a7b3d3e.png">

Similar to the first added message, in order for this second message to display properly the **handleRequest** method is called again. When this method is called, it will again take in a URL as its argument. In this case, the URL is now `http://localhost:4000/add-message?s=Second String!!` because a different message is being added.

Since this is the second time the method has been called, `list` is currently carrying the previous message(s) and will concatenate this new message which will also be followed by a concatenated line separator. When this is completed the new value of the string is formatted and returned to the webpage where it displays the previous message(s) followed by the newly added message on a new line.
