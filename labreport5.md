## Lab report 5: Researching a different command from lab report 3
I researched 4 `grep` commands in lab report 3, so I'm going to do another 4 `grep` command in this lab report. I looked up for the options at the website: [https://en.wikibooks.org/wiki/Grep](https://en.wikibooks.org/wiki/Grep)          
### 1: grep -b command
The first command I tried is:        
```
grep -b  "Lydia" written_2/non-fiction/OUP/Berk/*.txt
```
the output is:      
```
written_2/non-fiction/OUP/Berk/ch1.txt:1133:•Bob and Sharon, parents of a 4-year-old: Our daughter, Lydia, could recite her ABCs and count from 1 to 20 by age 2 1/2. When we looked for a preschool, many programs appeared to do little more than let children play, so we chose one with lots of emphasis on academics. To me, Lydia’s preschool seems like great preparation for kindergarten and ﬁrst grade, but each morning, Lydia hates to go. Why is Lydia, who’s always been an upbeat, curious child, so unhappy?
written_2/non-fiction/OUP/Berk/ch1.txt:24274:Recall 4-year-old Lydia’s dislike of her academic preschool, described at the beginning of this chapter. Lydia’s negative reaction is certainly consistent with research ﬁndings. The behaviorist presumption that development can be mechanically engineered by social input, guaranteeing brighter, socially more mature children, is not borne out by the evidence.
```
the second command I tried is:
```
grep -b "1807" written_2/travel_guides/berlitz2/Algarve-History.txt 
```
the output is:           
```
10979:In 1807 the French invaded Lisbon, causing the royal family to flee to Brazil. Spain, followed by Portugal, rose up against the French occupation, in what came to be known as the Peninsular War.
```
According to the website, `grep -b` command gives a historical curiosity: precede each matching line with a block number.
