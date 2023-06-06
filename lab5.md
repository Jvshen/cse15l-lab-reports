# Lab Report 3
## Part 1
### Edstem Posts

Student's question:

![Image](StudentResponse1.jpg)

TA's response:

![Image](TAResponse1.jpg)

Student's response:

![Image](StudentResponse2.jpg)

TA's response:

![Image](TAResponse2.jpg)

Student's response:

![Image](StudentResponse3.jpg)

### Information about setup
- The file and directory structure needed for this setup was taken from week 7 lab. This included the JUnit files, ```ListExamples.java```, ```ListExamplesTests.java```, and ```test.sh```.
- The contents of each file before fixing bug are as follows:
  - ![Image](TestActual.jpg) 
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
    - I changed the first while loop: ``````

