**Part 1: Serving up servers**

Basically I made a server which takes in strings from the query and prints them on the site. The code for this is below.

![image](https://maximpodgore.github.io/cse15l-lab-reports/week31.png)  

Essentially I made a handler that works with the basic server code to *handle* the things people type in the browser. This handler only responds to the path /add-string.
After the query "?"and the following "=" it will concatenate the terms left to a mega string. It will throw /n in there to make it appear on
the new line. That's basically it. The only thing that gets changed is that website display string that keeps on getting added to.
Here's some screenshots of it in action.

![image](https://maximpodgore.github.io/cse15l-lab-reports/week32.png)  

![image](https://maximpodgore.github.io/cse15l-lab-reports/week33.png)  

**Part 2: A Test of your patience**  

This is a test case that causes the reverseInPlace method to fail. 
![image](https://maximpodgore.github.io/cse15l-lab-reports/week34.png)  

This is a test case that the buggy reverseInPlaceMethod passes
![image](https://user-images.githubusercontent.com/56902053/215014706-59c6e1fa-954b-4ff3-bdcc-a9753915bdf5.png)  

And here is the output (Don't look at the terminal for the error message that's due to JDK and java mismatch)
![image](https://maximpodgore.github.io/cse15l-lab-reports/week46.png)  

Here is the buggy version of the code:  

`static void reverseInPlace(int[] arr) {  
    for(int i = 0; i < arr.length; i += 1) {  
      arr[i] = arr[arr.length - i - 1];     
    }}`
  
 `static void reverseInPlace(int[] arr) {  
    int[] newArray = new int[arr.length];  
    for(int i = 0; i < arr.length; i += 1) {   
      newArray[i] = arr[arr.length - i - 1];  
    }
    for(int i = 0; i < arr.length; i += 1) {    
      arr[i] = newArray[i];   
    }}`
  
  Basically the original function would write over the original array but midway it's gonna take the new late index values now early in the array and think they were the original early index values. We can solve that by creating a temp array and deep copying the result.
  
  **Part 3: The Debrief** 
  
  I definitely learned more about the terminology of bugs, debugging, and correct programs. Additionally, I learned how a server and urls work. Last but not least, I got better at nagivating the terminal by using arrow keys and learned how to clone repositories onto the ieng6 server. Thanks for reading
