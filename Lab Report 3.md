# Lab Report 3


## *Alternate Way to use grep #1 (`grep -r`):*

  *Source:* [https://man7.org/linux/man-pages/man1/grep.1.html](https://man7.org/linux/man-pages/man1/grep.1.html)

  *Example 1:*
  
   * Command:

```
$ grep -r "Lucayans" written_2
```
   
   * Output: 

```
written_2/travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peacef
ul Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from S
outh America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops 
and from what they caught from sea and shore. Nothing in the experience of these gentle people could h
ave prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 Oct
ober 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Ind
ians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his 
royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only tw
o weeks before sailing towards Cuba.
written_2/travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Baha
mas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago 
en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers 
dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the suppl
ies of water on their ships before they began the long journey back to Europe with their cargoes of Sou
th American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were re
moved from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hi
spaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```

   * The `grep -r` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, and it is printing the lines that match the pattern "Lucayans". This command is 
useful for searching through multiple directories and subdirectories rather than just one file.

  *Example 2:*
  
   * Command:

```
$ grep -r "Vista" written_2
```
   
   * Output: 

```
written_2/non-fiction/OUP/Castro/chB.txt:Buena Vista, Mateo, La Seis, Chiquis, El Sur and all
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt:        Greystone Mansion (905 Loma Vista Dr.), 
the spectacular neo-Gothic
written_2/travel_guides/berlitz1/WhereToMadeira.txt:        by car is Quinta da Boa Vista (Rua Luis Fig
ueiroa de Albuquerque). The
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt:Just 3 km (2 miles) down river from Portimão is 
Praia da Rocha, which became a holiday village for wealthy Portuguese families back at the end of the 1
9th century. It was “discovered” by the British in the 1930s, when this “beach of rocks,” strewn with e
xtravagantly shaped eroded stacks, provided an inspirational refuge for writers and intellectuals. The 
belle époque Hotel Bela Vista is a living monument from those days.
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:If you want a view of the whole city and the Nort
h Saskatchewan River on your way home, stop off at Vista 33, the observation level of the telephone bui
lding.
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt:High in the hills behind Ponce is Hacienda Bu
ena Vista. To get there, take Route 10, a major north-south artery. The road climbs steeply into dense 
vegetation and cooler air before you see signs for the hacienda; the climate and environmental conditio
ns here were ideal for the coffee that the plantation began to grow more than 150 years ago. The planta
tion fell into neglect in the 20th century, but since 1984 it has been returned to its original state b
y The Conservation Trust of Puerto Rico. Agricultural machinery such as coffee bean huskers can be seen 
in the original buildings, and the water mill and canals, which harnessed the power of the Canas River
, are now in working order. The facility shows how plantations used to operate and offer a fascinating 
insight into agricultural life in Puerto Rico all those years ago. Advance reservations are required fo
r the tours (see page 64).
```

   * The `grep -r` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, and it is printing the lines that match the pattern "Vista". This command is 
useful for searching through multiple directories and subdirectories rather than just one file.

## *Alternate Way to use grep #2 (`grep -r -o`):*

  *Source:* [https://man7.org/linux/man-pages/man1/grep.1.html](https://man7.org/linux/man-pages/man1/grep.1.html)
  
  *Example 1:*
  
   * Command:

```
$ grep -r -o "Lucayans" written_2
```
   
   * Output: 

```
written_2/travel_guides/berlitz2/Bahamas-History.txt:Lucayans
written_2/travel_guides/berlitz2/Bahamas-History.txt:Lucayans
```

   * The `grep -r -o` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, and it is printing only the matched parts of a matching line for the pattern "Lucayans", 
with each part on different output lines. This command is useful when searching for files that contain a 
particular word.

  *Example 2:*
  
* Command:

```
$ grep -r -o "vista" written_2
```
   
   * Output: 

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
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/China-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/China-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/China-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/China-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt:vista
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt:vista
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt:vista
```

   * The `grep -r -o` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, and it is printing only the matched parts of a matching line for the pattern "vista", 
with each part on different output lines. This command is useful when searching for files that contain a 
particular word.

## *Alternate Way to use grep #3 (`grep -r -l`):*

  *Source:* [https://man7.org/linux/man-pages/man1/grep.1.html](https://man7.org/linux/man-pages/man1/grep.1.html)
  
  *Example 1:*
  
* Command:

```
$ grep -r -l "Lucayans" written_2
```
   
   * Output: 

```
written_2/travel_guides/berlitz2/Bahamas-History.txt
```

   * The `grep -r -l` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, it is suppressing the normal output, and it is printing the name of each input file that 
contains the pattern "Lucayans". Although the output for this command is similar to the `grep -r -o` by 
printing the names of each input file that contains the given pattern, this command is useful when you do not
want the output to print duplicate files.

  *Example 2:*
  
* Command:

```
$ grep -r -l "vista" written_2
```
   
   * Output: 

```
written_2/travel_guides/berlitz1/IntroDublin.txt
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
written_2/travel_guides/berlitz1/IntroMadeira.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToGreek.txt
written_2/travel_guides/berlitz1/WhereToIbiza.txt
written_2/travel_guides/berlitz1/WhereToIsrael.txt
written_2/travel_guides/berlitz1/WhereToJerusalem.txt
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhereToMadeira.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
```

   * The `grep -r -l` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, it is suppressing the normal output, and it is printing the name of each input file that 
contains the pattern "vista". Although the output for this command is similar to the `grep -r -o` by 
printing the names of each input file that contains the given pattern, this command is useful when you do not
want the output to print duplicate files.

## *Alternate Way to use grep #4 (`grep -r -l -i`):*

  *Source:* [https://man7.org/linux/man-pages/man1/grep.1.html](https://man7.org/linux/man-pages/man1/grep.1.html)
  
  *Example 1:*
  
* Command:

```
$ grep -r -l -i "lucayans" written_2
```
   
   * Output: 

```
written_2/travel_guides/berlitz2/Bahamas-History.txt
```

   * The `grep -r -l -i` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, it is suppressing the normal output, and it is printing the name of each input file that 
contains the pattern "lucayans" while ignoring case distinctions in the files. Although the output for this 
command is useful when you want to search for files that contain a particular pattern regardless of the case
distinctions in the files.

  *Example 2:*
  
* Command:

```
$ grep -r -l -i "vista" written_2
```
   
   * Output: 

```
written_2/non-fiction/OUP/Castro/chB.txt
written_2/travel_guides/berlitz1/IntroDublin.txt
written_2/travel_guides/berlitz1/IntroLakeDistrict.txt
written_2/travel_guides/berlitz1/IntroMadeira.txt
written_2/travel_guides/berlitz1/WhereToFrance.txt
written_2/travel_guides/berlitz1/WhereToGreek.txt
written_2/travel_guides/berlitz1/WhereToIbiza.txt
written_2/travel_guides/berlitz1/WhereToIsrael.txt
written_2/travel_guides/berlitz1/WhereToJerusalem.txt
written_2/travel_guides/berlitz1/WhereToLakeDistrict.txt
written_2/travel_guides/berlitz1/WhereToLosAngeles.txt
written_2/travel_guides/berlitz1/WhereToMadeira.txt
written_2/travel_guides/berlitz2/Algarve-WhereToGo.txt
written_2/travel_guides/berlitz2/Athens-WhereToGo.txt
written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
written_2/travel_guides/berlitz2/CanaryIslands-WhereToGo.txt
written_2/travel_guides/berlitz2/China-WhereToGo.txt
written_2/travel_guides/berlitz2/Costa-WhereToGo.txt
written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
written_2/travel_guides/berlitz2/CstaBlanca-WhereToGo.txt
written_2/travel_guides/berlitz2/Nepal-WhatToDo.txt
written_2/travel_guides/berlitz2/Portugal-WhereToGo.txt
written_2/travel_guides/berlitz2/PuertoRico-WhereToGo.txt
written_2/travel_guides/berlitz2/Vallarta-WhereToGo.txt
```

   * The `grep -r -l -i` command is reading all of the files under each directory and subdirectory inside the
written_2 directory, it is suppressing the normal output, and it is printing the name of each input file that 
contains the pattern "vista" while ignoring case distinctions in the files. Although the output for this 
command is useful when you want to search for files that contain a particular pattern regardless of the case
distinctions in the files.
