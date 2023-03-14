# Lab Report 5  

In this lab, I will be revisiting Lab Report 3, where I researched different uses of the grep command. This time however, I will be researching even more commands that can be used with 'grep'. I will still include the commands I researched last time, but the new ones will be on top. 
    
    
The reason that I chose to do this is because I felt that this was the most interesting lab for me, because I was able to learn new ways to use the most useful command in my opinion, which is grep. In this lab report, I will research and learn even more uses of the command.     
  
  
In this lab, I will research more commands that can be used with 'grep', show two examples of an input and an output for each command, and explain why it is that this command can be useful.   
  
  
By doing this, I learned a lot more about the grep command, and I learned how to use more commands in useful ways.
  
  
## The 'grep' Command   

The grep command is a command used to search and match text files contained in the regular expression. This command is very important because it can help find files in large databases. 
  
 There are many different commands that can be used with grep, and here are a few of them.  
 
 ## New Commands  
   
## -w  

Input: 

```
grep -w vista berlitz1_vista.txt
```       
  
  
Output:  

```
$ grep -w vista berlitz1 vista.txt
written 2/travel guides/berlitz1/WhereToFrance.txt:
written 2/travel guides/berlitz1/whereToFrance.txt:
written 2/travel guides/berlitz1/WhereToFrance.txt:
written 2/travel guides/berlitz1/WhereToGreek.txt:
written 2/travel guides/berlitz1/WhereToJerusalem.txt:
vista was originally planned for Napoleon to see from his bedroom in
The little port town of Cancale - with a wide vista across
Saint-Philippe bastion and the Tour Bidouane opening up a vista along
ancient port, now silted up. From here, the vista of the whole town can
crowned by the conical roof of the Dormition Abbey. This sweeping vist
written_2/travel guides/berlitz1/WhereToLakeDistrict.txt:

```      

By using the grep -w command, we are able to find a specific word in a file. In this exampl, we found all of the paths of files that include the word "vista" and where the word is used. This command is useful for when we need to search a lot of files for a keyword, we can find the files without filling the command line. 
  
Another example of using this command would be the following:      

Input:

```
find written_2/ | grep -w Bahamas
```   

Output:  

```
$ find written 2/ | grep -w Bahamas
written 2/travel guides/berlitz2/Bahamas-History.txt
written 2/travel guides/berlitz2/Bahamas-Intro.txt
written 2/travel guides/berlitz2/Bahamas-WhatToDo.txt
written 2/travel guides/berlitz2/Bahamas-WhereToGo.txt
```    

In this example, the command can be useful if we are trying to sort files that contain a certain keyword in order.    

## -v  

Input:  

```
find written_2/ | grep -v History
```     

Output:  

```
$ find written 2/ | grep -v History
written 2/
written 2/non-fiction
written 2/non-fiction/OUP
written 2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written 2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written 2/non-fiction/OUP/Abernathy/ch3.txt
written 2/non-fiction/OUP/Abernathy/ch6.txt
written 2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/cho.txt
written 2/non-fiction/OUP/Berk
written 2/non-fiction/OUP/Berk/ch1.txt
written 2/non-fiction/OUP/Berk/ch2.txt
written 2/non-fiction/OUP/Berk/CH4.txt
written 2/non-fiction/OUP/Berk/ch7.txt
written 2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chc.txt
written 2/non-fiction/OUP/Castro/chL.txt
written 2/non-fiction/OUP/Castro/chM.txt
written 2/non-fiction/OUP/Castro/chN.txt
written 2/non-fiction/OUP/Castro/cho.txt
written 2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/cho.txt
written 2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chv.txt
written 2/non-fiction/OUP/Castro/chw.txt
written 2/non-fiction/OUP/Castro/chY.txt
written 2/non-fiction/OUP/Castro/chZ.txt
```     
  
The grep -v command is an interesting one that I found, that essentially does the opposite of the previous command I talked about. This command lists the files where a certain keyword is not used. This is useful for sorting files and omitting ones without the keyword that is needed.   

Here is another example of this command:  

Input:  

```
find written_2/ | grep -v Paris
```  
  
  
  Output:  
  
  ```
$ grep -v Paris
written 2/
written 2/non-fiction
written 2/non-fiction/OUP
written 2/non-fiction/OUP/Abernathy
written_2/non-fiction/OUP/Abernathy/ch1.txt
written_2/non-fiction/OUP/Abernathy/ch14.txt
written 2/non-fiction/OUP/Abernathy/ch15.txt
written_2/non-fiction/OUP/Abernathy/ch2.txt
written 2/non-fiction/OUP/Abernathy/ch3.txt
written 2/non-fiction/OUP/Abernathy/ch6.txt
written 2/non-fiction/OUP/Abernathy/ch7.txt
written_2/non-fiction/OUP/Abernathy/ch8.txt
written_2/non-fiction/OUP/Abernathy/cho.txt
written 2/non-fiction/OUP/Berk
written 2/non-fiction/OUP/Berk/ch1.txt
written 2/non-fiction/OUP/Berk/ch2.txt
written 2/non-fiction/OUP/Berk/CH4.txt
written 2/non-fiction/OUP/Berk/ch7.txt
written 2/non-fiction/OUP/Castro
written_2/non-fiction/OUP/Castro/chA.txt
written_2/non-fiction/OUP/Castro/chB.txt
written_2/non-fiction/OUP/Castro/chc.txt
written 2/non-fiction/OUP/Castro/chL.txt
written 2/non-fiction/OUP/Castro/chM.txt
written 2/non-fiction/OUP/Castro/chN.txt
written 2/non-fiction/OUP/Castro/cho.txt
written 2/non-fiction/OUP/Castro/chP.txt
written_2/non-fiction/OUP/Castro/cho.txt
written 2/non-fiction/OUP/Castro/chR.txt
written_2/non-fiction/OUP/Castro/chv.txt
written 2/non-fiction/OUP/Castro/chw.txt
written 2/non-fiction/OUP/Castro/chY.txt
written 2/non-fiction/OUP/Castro/chZ.txt
``` 
  
  
Here, the output is esentially the same, because the same files also don't contain the keyword "Paris", but again this command would be useful for finding which files do not contain a keyword in order to organize them. 
  
  
## -n  

Input: 

```
grep -n Paris written_2/travel_guides/berlitz2/Paris-WhereToGo.txt
```    

Output:  

```
271 
```     

The grep -n command returns the line number where a certain keyword is used. This is useful for trying to locate a certain word within a file. In this example, we are searching for where the keyword 'Paris' appears in that path.
  
  
Another example:      

Input:

```
grep -n Lucayans written_2/travel_guides/berlitz2/Bahamas.txt
``` 
 
   
Output: 
```
574 
```      

In this example now, we see that the keyword "Lucayans" is found on line 574 of the certain file. This is useful for locating parts of a long file to read about a certain keyword. 



   
## -c
  
The grep -c command prints only a count of the lines that match a pattern in a file. For example, you will give them comand grep -c "Lucayans" written_2.txt. This will return a number like "2". It will look like this.   

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -c "Lucayans" written_2.txt
     
[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ 2
```          
The reason that this is a useful command for this example is that it gives you the number of lines that match the pattern in a file that you pass it. For example, instead of having to manually count how many times "Lucayans" appears in a set of files, you can simply use the grep -c command and it will return the number for you, which in this case was 2 files. This can help with file management, word counts, and many more things. 

Here is another example of me doing it using the word "Athens" instead:


```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -c "Athens" written_2.txt
     
[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ 174
```        

In this example, this is a useful command because it gives you the number of lines that match "Athens" in the written_2 folder, when you pass it the command. Instead of having to manually count how many times the pattern appears in a written_2, you can simply use the grep -c command and it will return the number for you. In this case, it was 174. 

    
## -r  

The grep -r command lists all of the files within a directory where a certain keyword appears. For example, in the following screenshot, I typed in "grep -r "Lucayans" and it gave me all of the files within the written_2 directory where the word "Lucayans" appears. 
  
My command:  

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -r "Lucayans" 
     
```      

![Image](-r1.jpeg)    
  
This is useful in this example because you pass "Lucayans" with the grep -r command, and it only gives you the files where "Lucayans" appears.   


Here is the same command used again but now with the keyword "Athens". As you can see, the result is not short!      
  
My command:  

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -r "Athens" 
     
```     

![Image](athenslong.jpeg)   

This is a very useful command because it returns the files where a certain keyword that is passed appears. The reason that this is useful is because if you have a large database with many files, but you only want to read about a certain topic, you can find which files to look into for this topic by using grep -r, without having to read through each file until you find it. Not only does it return the files, but it only returns the file names so that your terminal is not filled up with a lot of words, and you can simply look at which files to read into. 


  
## -l
Another grep command that is commonly used is -l. By using the -l, it means that you are asking for it to show the file name, not the result itself. As you can see, this now shows you where the word "Lucayans" appears, but not the entire file itself.    

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -rl "Lucayans" 
     
```     

![Image](-r2.jpeg)    

This was a useful command in this example because as you can see, when it was passed "Lucayans" with the grep -rl command, it only returned the file names where that keyword appeared. This made it very easy for me to see which files 

Here is another example of using the grep -l command with another key word "Athens".    

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -rl "Athens" 
     
```   

![Image](athens.jpeg)     

The reason that this is a very useful command is because it returns the file names where a certain keyword that is passed appears. This is useful because if you have a large number of files, but you only want to read about a certain topic, you can find which files to look into for this topic by using grep -r, without having to read through each file until you find it. Not only does it return the files, but it only returns the file names so that your terminal is not filled up with a lot of words, and you can simply look at which files to read into. 

## -o  

Another useful grep command is grep -o. The -o command means that you want to only print the matched parts of a matching line,
 with each such part on a separate output line. Here is an example of this command:  
 
 Input:  
 
 
 ```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -o "Lucayans" written_2.txt
     
```     
Output:   
 ```
Lucayans
Lucayans
Lucayans
Lucayans
Lucayans

```         

This is an example where the command will be useful because if I am looking for a list of the matching parts of a keyword without all of the text, I can use this command and it only gives me the keywords. 

Here is another example of this using the keyword "Athens" instead.   

Input:  
 
 
 ```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -o "Athens" written_2.txt
     
```     
Output:   
 ```
Athens
Athens
Athens
Athens
Athens

```         

In this example, the command is useful because I wanted all of the times the keyword "Athens" was printed in the files, and it returned it to me without the text which makes it very easy to read and locate without filling the entire terminal. 
  
It is clear that there are many different options for using grep commands, and these are just some of the few. The best part about this is that for every task that you need to do with your command line, there is an optimal way to find it, and it just has to be found!

  
For citation purposes, I found my grep command line options at this URL:   
  
[Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)


