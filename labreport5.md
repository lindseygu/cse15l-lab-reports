## Lab report 5: Researching a different command from lab report 3
In lab report 3, I originally researched the `grep` command, so in this lab report I'm going to research the `find` command options. The website I'm looking at is [https://man7.org/linux/man-pages/man1/find.1.html](https://man7.org/linux/man-pages/man1/find.1.html)        
### 1.find -name command
the first command I typed is:
```
find written_2 -name ch1.txt
```
the output is:     
```
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Rybczynski/ch1.txt
written_2/non-fiction/OUP/Kauffman/ch1.txt
written_2/non-fiction/OUP/Fletcher/ch1.txt
```
the second command I typed is:    
```
find written_2 -name HandRJamaica.txt 
```
the output it:       
```
written_2/travel_guides/berlitz1/HandRJamaica.txt
```
According to the website, the `find -name` command searches a specific file under the specified directory and return its relative path. In my examples, the output is all of the matched files of the input name ending with.txt, with their paths provided. This command is useful when you don't remember the path for a certain file under a certain directory.

### 2.find -mtime n command
the first command I typed is:      
```
find written_2 -mtime -30 
```
the output is:      
```
written_2
written_2/non-fiction
written_2/non-fiction/OUP
written_2/non-fiction/OUP/Berk
written_2/travel_guides
written_2/travel_guides/berlitz1
```
the second command I typed is:
```
find written_2 -mtime -20
```
the output is:
```
written_2
written_2/travel_guides
written_2/travel_guides/berlitz1
```
According to the website, the `find -mtime n` command returns files with data was last modified less than, more than or exactly n*24 hours ago. In the two examples I tried, I use the `-n` to indicate for less than the number of n. In the first example, the returned files are modified less than 30 days and the second example returns files modified less than 20 days ago. This command is useful when you want to know what are the files modified recently, given a certain number of days.

### 3.find -depth command
the first command I typed is:
```
find written_2/non-fiction/OUP/Abernathy -depth
```
the output is:
```
written_2/non-fiction/OUP/Abernathy/ch2.txt
written_2/non-fiction/OUP/Abernathy/ch3.txt
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch6.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/ch9.txt
written_2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written_2/non-fiction/OUP/Abernathy
```
the second command I typed is:
```
find written_2/non-fiction/OUP/Berk -depth  
```
the output is:
```
written_2/non-fiction/OUP/Berk/ch2.txt
written_2/non-fiction/OUP/Berk/ch1.txt
written_2/non-fiction/OUP/Berk/CH4.txt
written_2/non-fiction/OUP/Berk/ch7.txt
written_2/non-fiction/OUP/Berk
```
According to the website, the `find -depth` command returns each directory's contents before the directory itself. In my two examples, the returned are all the files under the maximum level below the given path. This command is useful when you want to see the paths of files under a certain directory before doing the next steps.

### 4. find -size n command
the first command I typed is:
```
find written_2 -size +250
```
the output is:
```
written_2/travel_guides/berlitz1/WhereToIndia.txt
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToMalaysia.txt
written_2/travel_guides/berlitz1/WhereToJapan.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
```
the second command I typed is:
```
find written_2 -size +400
```
the output is:
```
written_2/travel_guides/berlitz1/WhereToItaly.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
```
According to the website, the `find -size n` command returns files uses less than, more than or exactly n units of space, rounding up. In the two examples, I uses `+` symbol before the number `n` to get files greater than the input number sizes. This command is useful when you want to know the files smaller than, right equal to , or greater than a certan file size under a certain directory.




