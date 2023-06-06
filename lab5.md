# Lab Report 5
## Part 1
### Edstem Posts

Student's question:

![Image](StudentResponse1-1.jpg)

![Image](StudentResponse1-3.jpg)

![Image](StudentResponse1-4.jpg)

![Image](StudentResponse1-5.jpg)

TA's response:

![Image](TAResponse1.jpg)

Student's response:

![Image](StudentResponse2-1.jpg)
![Image](StudentResponse2-5.jpg)
![Image](StudentResponse2-4.jpg)

TA's response:

![Image](TAResponse2.jpg)

Student's response:

![Image](StudentResponse3.jpg)

### Information about setup
- The file and directory structure needed for this setup was taken from week 7 lab. This included the JUnit files, ```ListExamples.java```, ```ListExamplesTests.java```, and ```test.sh```.
- The contents of each file before fixing bug are as follows:
  - ![Image](TestActual-1.jpg)
  - ![Image](TestActual-2.jpg)
  - ![Image](TestExamples.jpg) 
  - ![Image](testsh.jpg)
- The full command line I ran to trigger the bug: 
  - ```bash test.sh <enter>```
- Description of what to edit:
  - First, I changed the JUnit run commands that were originally for Windows to Mac:
    - From ```javac -cp ".;lib/hamcrest-core-1.3.jar;lib/junit-4.13.2.jar" *.java```
    - and ```java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore ListExamplesTests```
    - To ```javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java```
    - and ```java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests```
  - Then I changed the While loop incrementation and indexes ```List.Examples.java```:
    - I changed the first while loop: ```while(index2 < list1.size()) {``` to ```while(index1 < list1.size()) {```, with ```index2 += 1;``` changing to ```index1 += 1;```
    - I then changed the second while loop: ```while(index1 < list2.size()) {``` to ```while(index2 < list2.size()) {``` with ```index1 += 1;``` changing to ```index2 += 1;```
    - Both while loops appear as so now:

```
while(index1 < list1.size()) {
      result.add(list1.get(index1));
      index1 += 1;
}
while(index2 < list2.size()) {
      result.add(list2.get(index2));
      // change index1 below to index2 to fix test
      index2 += 1;
}
return result;
```
At the end, the code was able to successfully run without any failures or errors:

![Image](Success.jpg)

## Part 2
Something I learned from my lab experience in the second half of this quarter was Vim. I learned that with Vim, you could edit a file through the terminal and change specific things about that file through the terminal. Using vim allows changing files to be a lot more convenient since you can edit the file straight through the terminal, not having to go directly in the file and changing it. Something that I also learned was the use of bash scripts. I learned that you can use bash scripts to carry out mutiple commands at once with only one command line. I also learned that CSE 15L teaches a lot of useful coding techniques!
