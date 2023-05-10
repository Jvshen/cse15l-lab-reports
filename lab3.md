For the command line ``` find ```, one interesting command-line option is the ``` -name ``` option. This command-line option for the ``` find ``` command line  allows you to search for all the files with a certain name. For example, ``` find ./technical -name biomed ``` will provide the output, ``` ./technical/biomed ```. What this command does is it provides all the files in the ``` ./technical ``` directory with ``` biomed ``` in it. Another example is ``` find ./technical -name government ``` which will provide the output ``` ./technical/government ```. What this command does is it provides all te files in the ``` ./techical ``` directory with ``` government ``` in it.

For the command line ``` find ```, another interesting command-line option is the ``` -type ``` option. This command-line option for the ``` find ``` command line allows you to search for all the files by a certain type. For example, ``` find ./techincal -type d ``` will provide the output,
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
What this command does is it provides all the files in the ``` ./techincal ``` directory with type ``` d ``` or in other words with a directory type. Another example is ``` find ./technical -type f ``` which will provide the output,
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
There is a lot more lines of code to this example output that I can't fit on this page but what this command does is it provides all the files in ``` ./technical ``` directory with type ``` f ``` or in other words with a file type.


