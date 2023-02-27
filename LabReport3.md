# Lab Report 3  

In this lab report, I will be exploring different command line options for the grep command, and showing that there are many more ways to use it!  
  
## The 'grep' Command   

The grep command is a command used to search and match text files contained in the regular expression. This command is very important because it can help find files in large databases. 
  
 There are many different commands that can be used with grep, and here are a few of them. 
   
## -c
  
The grep -c command prints only a count of the lines that match a pattern in a file. For example, you will give them comand grep -c "Lucayans" written_2.txt. This will return a number like "2". It will look like this.   

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -c "Lucayans" written_2.txt
     
[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ 2
```      

Here is another example of me doing it using the word "Athens" instead:


```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -c "Athens" written_2.txt
     
[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ 174
```      

    
## -r  

The grep -r command lists all of the files within a directory where a certain keyword appears. For example, in the following screenshot, I typed in "grep -r "Lucayans" and it gave me all of the files within the written_2 directory where the word "Lucayans" appears. 
  
My command:  

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -r "Lucayans" 
     
```      

![Image](-r1.jpeg)    

Here is the same command used again but now with the keyword "Athens". As you can see, the result is not short!      
  
My command:  

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -r "Athens" 
     
```     

![Image](athenslong.jpeg) 


  
## -l
Another grep command that is commonly used is -l. By using the -l, it means that you are asking for it to show the file name, not the result itself. As you can see, this now shows you where the word "Lucayans" appears, but not the entire file itself.    

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -rl "Lucayans" 
     
```     

![Image](-r2.jpeg)  

Here is another example of using the grep -l command with another key word "Athens".    

```

[cs15lwi23aro@ieng6-203]:skill-demo1-data:297$ grep -rl "Athens" 
     
```   

![Image](athens.jpeg)   

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
  
It is clear that there are many different options for using grep commands, and these are just some of the few. The best part about this is that for every task that you need to do with your command line, there is an optimal way to find it, and it just has to be found!

  
For citation purposes, I found my grep command line options at this URL:   
  
[Link]([http://a.com](https://www.geeksforgeeks.org/grep-command-in-unixlinux/))
