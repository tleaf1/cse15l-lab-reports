# Lab Report 2

## Servers and Bugs

**StringServer**

<img width="629" alt="Screen Shot 2023-01-29 at 12 24 06 PM" src="https://user-images.githubusercontent.com/122562580/215353919-e23daa83-2e8d-4f88-9aa6-cd6b069e8560.png">

**First Added Message:**
<img width="1031" alt="Screen Shot 2023-01-29 at 12 26 54 PM" src="https://user-images.githubusercontent.com/122562580/215354100-5203a155-98d2-4645-b86e-61a169269505.png">

In order for this first string to display, the **handleRequest** method in the handling class is called. This method has a URI parameter which takes in a URL as its argument. In this instance the URL is `http://localhost:4000/add-message?s=FirstString!`. Along with this, an empty string called `list` is instantiated in order to store the relevant strings from the URL query.

Once this method is called it checks the path of URI parameter. If the paramter is equal to "/add-message" the method will then instantiate a String array that separates the query into two parts at the equal sign. If the first parameter is equal to "s" the handleRequests method will concatenate the second paramter to the empty string followed by a new line separator. Once this is complete the string value is updated to contain the first message and is then returned in order to display on the webpage.

**Second Added Message:**
<img width="1042" alt="Screen Shot 2023-01-29 at 12 27 38 PM" src="https://user-images.githubusercontent.com/122562580/215354860-0c9eea3f-fedc-417a-a453-5eab6a7b3d3e.png">

Similar to the first added message, in order for this second message to display properly the **handleRequest** method is called. When this method is called, it will again take in a URL as its argument. In this case, the URL is now `http://localhost:4000/add-message?s=Second String!!` because a different message is being added.

When this URL is passed through to the message, if the path is equal to "/add-message" a new string array is instantiated to hold the values of the query that are split at the equal sign. In the same fashion, if the first parameter is equal to "s", the second parameter will be concatenated to the empty string `list `.

Since this is the second time the method has been called, `list` is currently carrying the previous message(s), followed by a line separator, and will concatenate this new message which will also be followed by a concatenated line separator. When this is completed the new value of the string is formatted and returned to the webpage where it displays the previous message(s) followed by the newly added message on a new line.

**A Bug in ArrayExamples**

Here is an example of a failure inducing input for the reverseInPlace method:
```
@Test
  public void testReverseInPlace2() {
    int[] input2 = {1,2,3,4,5};
    ArrayExamples.reverseInPlace(input2);
    assertArrayEquals(new int[] {5,4,3,2,1}, input2);
  }
  ```
Here is an example of an input that does not produce a failure:
  ```
  @Test 
	public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
  ```
Displayed here are the outcomes of running these two inputs in JUnit:
<img width="643" alt="Screen Shot 2023-01-29 at 1 11 37 PM" src="https://user-images.githubusercontent.com/122562580/215355945-ad3e93f4-7975-4afd-9beb-45d54c8926a1.png">

Here is the original code with the bug that produced the symptom:
```
static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i++) {
      arr[i] = arr[arr.length - i - 1];
    }
  }
```
Here is the updated code with the fix for the bug:
```
static void reverseInPlace(int[] arr) {
    int [] temp = new int[arr.length];
    for(int i = 0; i < arr.length; i++) {
      temp[i] = arr[arr.length - i - 1];
    }
    for (int k = 0; k < arr.length; k++) {
      arr[k] = temp[k];
    }
  }
```
This fix addresses the issue because the original code has the input array updating and assigning new values to itself which causes an incorrect index value to be assigned once the array has iterated through half of its length.

However, by creating a temporary array of the same length, all correct values of the input array can be assigned to the right index location in the temporary array. Once this is done we can update the new values of the input array with the correct values from the temporary array.

**What I Learned in Lab**

One thing I learned in lab is the structure and function of URLs. Before the lab I did not know that the URL was separated into different parts and thought it was just the name of the website followed by ".com" and that everything after was gibberish. Now I know that it is made up of parts that include the name/location of the website but also is separated into different paths based on where one is navigating (my different github repositories as an example) as well as queries in order to have the website perform a function.

