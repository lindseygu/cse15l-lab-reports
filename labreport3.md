## Lab Report 3: Researching Commands
I looked up for grep command line options at the website: [https://en.wikibooks.org/wiki/Grep](https://en.wikibooks.org/wiki/Grep)
### 1: grep -o command
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
According to the website, `grep -o` command will give output results of the matched parts of a matching line. In these two examples, the output is giving separate line results for each lines in the .txt files that contain the input string. This command might be useful when you want to know how many lines in the given directory does a specific word occurs, since it will give you every lines where the word occurs with its path.             
### 2: grep -l command
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
According to the website, `grep -l` command gives the files only that matches the input string. In the first example, there's only one file that contains the string "Lydia", so only one line is printed as the output. In the second example, there are multiple files that contain the input string. This command is useful when you don't care how many times a string occurs in a particular file, you only want to know what files contain the input string one or multiple times.                
### 3: grep -c command
The first command I tried is:       
```
grep -c "1807" written_2/travel_guides/berlitz2/Algarve*.txt
```        
The output result is:       
```
written_2/travel_guides/berlitz2/Algarve-History.txt:1
written_2/travel_guides/berlitz2/Algarve-Intro.txt:0
written_2/travel_guides/berlitz2/Algarve-WhatToDo.txt:0
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:0
```         
The second command I tried is :      
```
grep -c "constitutional" written_2/non-fiction/OUP/Fletcher/*.txt
```     
The output result is:        
```
written_2/non-fiction/OUP/Fletcher/ch1.txt:15
written_2/non-fiction/OUP/Fletcher/ch10.txt:11
written_2/non-fiction/OUP/Fletcher/ch2.txt:12
written_2/non-fiction/OUP/Fletcher/ch5.txt:7
written_2/non-fiction/OUP/Fletcher/ch6.txt:28
written_2/non-fiction/OUP/Fletcher/ch9.txt:15
```        
According to the website, `grep -c` command gives the count(number of matching words) for the files under the input path. For the first example, the output result shows five files in the directory with one path of one match. For the second example, shows each line the number of directories with matching words. This command is useful when you want to check the occurance time of the search word in each individual files in the path pattern, instead of just the matched files.          
### 4: grep -n command 
The first command I tried is:      
```
grep -n "Lydia" written_2/non-fiction/OUP/Berk/*.txt
```
The output result is:      
```
written_2/non-fiction/OUP/Berk/ch1.txt:9:•Bob and Sharon, parents of a 4-year-old: Our daughter, Lydia, could recite her ABCs and count from 1 to 20 by age 2 1/2. When we looked for a preschool, many programs appeared to do little more than let children play, so we chose one with lots of emphasis on academics. To me, Lydia’s preschool seems like great preparation for kindergarten and ﬁrst grade, but each morning, Lydia hates to go. Why is Lydia, who’s always been an upbeat, curious child, so unhappy?
written_2/non-fiction/OUP/Berk/ch1.txt:54:Recall 4-year-old Lydia’s dislike of her academic preschool, described at the beginning of this chapter. Lydia’s negative reaction is certainly consistent with research ﬁndings. The behaviorist presumption that development can be mechanically engineered by social input, guaranteeing brighter, socially more mature children, is not borne out by the evidence.
```          
The second command I tried is:       
```
grep -n "1807" written_2/travel_guides/berlitz2/Boston-WhereToGo.txt
```       
The output result is:      
```
17:In the 19th century so many leading intellectuals lived here that the city became known as “The Athens of the United States.” On Chestnut Street alone, there lived historian Francis Parkman, actor Edwin Booth, author Julia Ward Howe, and painter John Singer Sargent. Louisa May Alcott and Nathaniel Hawthorne resided on Pinckney Street, while Beacon Street which Oliver Wendell Holmes dubbed “the sunny street that holds the sifted few” boasted historian William Prescott. At number 10 Beacon, stop at the Boston Athenaeum (Tel. 227-0270; guided tours Tuesday and Thursday at 3pm; reservations needed), a haven for writers and intellectuals since it was established in 1807. The 750,000-volume collection is amazing, but so too is the interior of the 1849 building, which is exquisitely furnished with antiques, busts of Benjamin Franklin, Daniel Webster, and others, and several paintings by John Singer Sargent and Gilbert Stuart. Farther along Beacon at number 45, Harrison Gray Otis died in the house that Bulfinch designed for him. Don’t miss the London-style Louisburg Square surrounded by some of the finest Greek Revival homes in New England.
```             
According to the website, `grep -n` command gives each matching output line with a line number. In my first example, the first matching result's line number is 9 and the second one is 54. In my second example, the line number is 17. This command is useful when you want to know the specific line number each time the matching string occurs in a file.
