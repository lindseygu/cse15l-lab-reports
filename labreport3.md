## Lab Report 3: Researching Commands
I looked up for grep command line options at the website https://en.wikibooks.org/wiki/Grep
### grep -o command
The first command I tried is:        
```
grep -o "vista" written_2/travel_guides/berlitz1/*.txt 
```         
The output result is:         
```
written_2/travel_guides/berlitz1/IntroDublin.txt:vista
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt:vista
written_2/travel_guides/berlitz1/IntroMadeira.txt:vista
written_2/travel_guides/berlitz1/WhereToFrance.txt:vista
written_2/travel_guides/berlitz1/WhereToFrance.txt:vista
written_2/travel_guides/berlitz1/WhereToFrance.txt:vista
written_2/travel_guides/berlitz1/WhereToGreek.txt:vista
written_2/travel_guides/berlitz1/WhereToIbiza.txt:vista
written_2/travel_guides/berlitz1/WhereToIbiza.txt:vista
written_2/travel_guides/berlitz1/WhereToIsrael.txt:vista
written_2/travel_guides/berlitz1/WhereToJerusalem.txt:vista
written_2/travel_guides/berlitz1/WhereToJerusalem.txt:vista
written_2/travel_guides/berlitz1/WhereToJerusalem.txt:vista
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:vista
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt:vista
written_2/travel_guides/berlitz1/WhereToMadeira.txt:vista
```                  
The second command I tried is:       
```
grep -o "1807" written_2/travel_guides/berlitz2/*.txt
```       
The output result is:
```
written_2/travel_guides/berlitz2/Algarve-History.txt:1807
written_2/travel_guides/berlitz2/Boston-WhereToGo.txt:1807
written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt:1807
written_2/travel_guides/berlitz2/Poland-History.txt:1807
written_2/travel_guides/berlitz2/Portugal-History.txt:1807
```            
According to the website, grep -o command will give output results of the matched parts of a matching line. In these two examples, the output is giving separate line results for each lines in the .txt files that contain the input string. This command might be useful when you want to know how many lines in the given directory does a specific word occurs, since it will give you every lines where the word occurs with its path.             
### grep -l command
The first command I tried is:        
```
grep -l "Lydia" written_2/non-fiction/OUP/Berk/*.txt
```         
The output result is:       
```
written_2/non-fiction/OUP/Berk/ch1.txt
```        
The second command I tried is:      
```
grep -l "constitutional" written_2/non-fiction/OUP/*/*.txt
```
The output result is:      
```
written_2/non-fiction/OUP/Fletcher/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch10.txt
written_2/non-fiction/OUP/Fletcher/ch2.txt
written_2/non-fiction/OUP/Fletcher/ch5.txt
written_2/non-fiction/OUP/Fletcher/ch6.txt
written_2/non-fiction/OUP/Fletcher/ch9.txt
```        
According to the website, grep -l command gives the files only that matches the input string. In the first example, there's only one file that contains the string "Lydia", so only one line is printed as the output. In the second example, there are multiple files that contain the input string. This command is useful when you don't care how many times a string occurs in a particular file, you only want to know what files contain the input string one or multiple times.           
### grep 


