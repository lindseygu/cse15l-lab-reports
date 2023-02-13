## Lab Report 3: Researching Commands
I looked up for grep command line options at the website https://en.wikibooks.org/wiki/Grep
### Grep -o command
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
According to the website, grep -o command will give output results of the matched parts of a matching line. In these two examples, the output is giving separate line results for each lines in the txt files that contain the input string.

