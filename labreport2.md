# Lindsey Gu's Lab Report Week3: Servers and Bugs
## Part 1
I created a web server called String Server that will return the current String added through the query part of the url and keeps the added Strings. The below screenshots shows the codes and what the web page looks like according to the input url.    
         
<img width="478" alt="Screen Shot 2023-01-25 at 11 37 15 PM" src="https://user-images.githubusercontent.com/122554943/215300565-988621e3-5fdf-4e21-bd12-095764a325b6.png">
In this case, the method called is handleRequest, and the relevant argument is the input url and one revelant string variable is str that gets updates with the input argument. From this specific request, the String str changes from an empty String to "Hello".        
<img width="539" alt="Screen Shot 2023-01-25 at 11 37 29 PM" src="https://user-images.githubusercontent.com/122554943/215300571-35266353-572e-4ef6-afb6-1d647235119f.png">
In this case, the method called is handleRequest, and the relevant argument is the input url and one revelant string variable is str that gets updates with the input argument. From this specific request, the String str changes from "Hello" to "Hello\n How are you", where \n represents a new line.               
<img width="791" alt="Screen Shot 2023-01-28 at 6 20 18 PM" src="https://user-images.githubusercontent.com/122554943/215300882-902a3d34-5af2-4d8c-bd1c-626c98e3b1c7.png">
         
## Part 2
