# Lab Report 3

## ```find``` command ```-name```
For the command line ``` find ```, one interesting command-line option is the ``` -name ``` option. This command-line option for the ``` find ``` command line  allows you to search for all the files with a certain name. 
### Example 1
For example, ``` find ./technical -name biomed ``` will provide the output, 

``` ./technical/biomed ``` 

What this command does is it provides all the files in the ``` ./technical ``` directory with ``` biomed ``` in it. 
### Example 2
Another example is ``` find ./technical -name government ``` which will provide the output,

``` ./technical/government ``` 

What this command does is it provides all te files in the ``` ./techical ``` directory with ``` government ``` in it. I found the ``` -name ``` command-line option on [man7](https://man7.org/linux/man-pages/man1/find.1.html).


## ```find``` command ```-type```
For the command line ``` find ```, another interesting command-line option is the ``` -type ``` option. This command-line option for the ``` find ``` command line allows you to search for all the files by a certain type. 
### Example 3
For example, ``` find ./techincal -type d ``` will provide the output,

```
./technical
./technical/government
./technical/government/About_LSC
./technical/government/Env_Prot_Agen
./technical/government/Alcohol_Problems
./technical/government/Gen_Account_Office
./technical/government/Post_Rate_Comm
./technical/government/Media
./technical/plos
./technical/biomed
./technical/911report
```

What this command does is it provides all the files in the ``` ./techincal ``` directory with type ``` d ``` or in other words with a directory type. 
### Example 4
Another example is ``` find ./technical -type f ``` which will provide the output,

```
./technical/biomed/1471-2121-2-3.txt
./technical/biomed/1471-213X-1-11.txt
./technical/biomed/1472-684X-1-5.txt
./technical/biomed/1476-4598-1-6.txt
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-13.1.txt
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-3.txt
./technical/911report/chapter-2.txt
```

There is a lot more lines of code to this example output that I can't fit on this page but what this command does is it provides all the files in the ``` ./technical ``` directory with type ``` f ``` or in other words with a file type. I found the ``` -type ``` command-line option on [man7](https://man7.org/linux/man-pages/man1/find.1.html).


## ```find``` command ```-mtime```
For the command line ``` find ```, another interesting command-line option is the ``` -mtime ``` option. This command-line option for the ``` find ``` command line allows you to search for all the files by how long ago they were modified. 
### Example 5
For example, ``` find ./technical -mtime -7 ``` will provide the output,

```
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-3.txt
./technical/911report/chapter-2.txt
./technical/911report/chapter-1.txt
./technical/911report/chapter-5.txt
./technical/911report/chapter-6.txt
./technical/911report/chapter-7.txt
./technical/911report/chapter-9.txt
./technical/911report/chapter-8.txt
./technical/911report/preface.txt
./technical/911report/chapter-12.txt
./technical/911report/chapter-10.txt
./technical/911report/chapter-11.txt
```

There is a lot more lines of code to this example output that I can't fit on this page but what this command does is it provides all the files in the ``` ./technical ``` directory with files that were modified within the last 7 days. 
### Example 6
Another example is ``` find ./technical -mtime -3 ``` will provide the output, 

```
./technical/911report/chapter-13.4.txt
./technical/911report/chapter-13.5.txt
./technical/911report/chapter-13.1.txt
./technical/911report/chapter-13.2.txt
./technical/911report/chapter-13.3.txt
./technical/911report/chapter-3.txt
./technical/911report/chapter-2.txt
./technical/911report/chapter-1.txt
./technical/911report/chapter-5.txt
./technical/911report/chapter-6.txt
```

There is a lot more lines of code to this example output that I can't fit on this page but what this command does is it provides all the files in the ``` ./technical ``` directory with files that were modified within the last 3 days. I found the ``` -mtime ``` command-line option on [man7](https://man7.org/linux/man-pages/man1/find.1.html). 


## ```find``` command ```-user```
Lastly, for the command line ``` find ```, another interesting command-line option is the ``` -user ``` option. This command-line option for the ``` find ``` command line allows you to search for a files that are owned by a specific user. 
### Example 7
For example, ``` find ./technical -user justinshen ``` will provide the output,

```
./technical/biomed/1471-2202-4-2.txt
./technical/biomed/1471-2172-3-9.txt
./technical/biomed/gb-2001-2-3-research0007.txt
./technical/biomed/1471-2199-2-6.txt
./technical/biomed/bcr567.txt
./technical/biomed/gb-2002-3-10-research0055.txt
./technical/biomed/1471-2121-2-3.txt
./technical/biomed/1471-213X-1-11.txt
./technical/biomed/1472-684X-1-5.txt
./technical/biomed/1476-4598-1-6.txt
./technical/911report
```

There is a lot more lines of code to this example output that I can't fit on this page but what this command does is it provides all the files in the ``` ./technical ``` directory with files that are owned by justinshen. 
### Example 8
Another example is ``` find ./technical -user andrewsou ``` will provide the output, 

``` find: -user: andrewsou: no such user ``` 

What this command does is it provides all the files in the ``` ./technical ``` directory with files that are owned by andrewsou, which in this case there are no files that are owned by andrewsou in the ``` ./technical ``` directory. I found the ``` -user ``` command-line option on [man7](https://man7.org/linux/man-pages/man1/find.1.html).
