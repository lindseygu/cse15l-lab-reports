# Lindsey Gu's Lab Report Week3: Servers and Bugs
## Part 1: Web Server      
I created a web server called String Server that will return the current String added through the query part of the url and keeps the added Strings. The below screenshots shows the codes and what the web page looks like according to the input url.    
         
<img width="478" alt="Screen Shot 2023-01-25 at 11 37 15 PM" src="https://user-images.githubusercontent.com/122554943/215300565-988621e3-5fdf-4e21-bd12-095764a325b6.png">               
In this case, the method called is handleRequest, and the relevant argument is the input url and one revelant string variable is str that gets updates with the input argument. From this specific request, the String str changes from an empty String to "Hello". Another value is the input url, which in this case is localhost:4000/add-message?s=Hello.This value is passed to the String list parameter but getQuery function to check if index 0 of the list is "s". Then the string "Hello" is added to str.                       
<img width="539" alt="Screen Shot 2023-01-25 at 11 37 29 PM" src="https://user-images.githubusercontent.com/122554943/215300571-35266353-572e-4ef6-afb6-1d647235119f.png">                
In this case, the method called is handleRequest, and the relevant argument is the input url and one revelant string variable is str that gets updates with the input argument. From this specific request, the String str changes from "Hello" to "Hello\n How are you", where \n represents a new line. Another value is the input url, which in this case is localhost:4000/add-message?s=How are you. This value is passed to the String list parameter but getQuery function to check if index 0 of the list is "s". Then the string "How are you" is added to str(which is not "Hello").                                                   
Here's the screenshot of the code(the structure is copied from the given code from lab2, then I make changes to fit this web server example):           
<img width="791" alt="Screen Shot 2023-01-28 at 6 20 18 PM" src="https://user-images.githubusercontent.com/122554943/215300882-902a3d34-5af2-4d8c-bd1c-626c98e3b1c7.png">       
         
## Part 2: Bugs from lab3          
One of the bugs from lab3 is the ReverseInPlace method, the original code is:         
```
static void reverseInPlace(int[] arr){
    for(int i = 0; i < arr.length);
        arr[i] = arr[arr.length - i - 1];
```         
The failure-inducing input(two written test cases) is below:     
```
@Test 
public void testReverseInPlace1() {
    int[] input1 = { 1, 2, 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3, 2, 1 }, input1);
	}

@Test 
public void testReverseInPlace2() {
    int[] input1 = { 0, 2, 4, 6 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 6, 4, 2, 0 }, input1);
	}
```           
And here are the results from the JUnit test:
<img width="682" alt="Screen Shot 2023-01-30 at 7 23 38 PM" src="https://user-images.githubusercontent.com/122554943/215655095-914daa8b-dae4-4df7-ae7f-5a6be22425c5.png">

<img width="683" alt="Screen Shot 2023-01-30 at 7 28 00 PM" src="https://user-images.githubusercontent.com/122554943/215655708-7dbc6d9a-0487-4495-b12c-7482af40484f.png">      
        
An input that  doesn’t induce a failure
