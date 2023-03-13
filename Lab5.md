**I automated Lab 6:**

Here is the code I used: 

`git clone git@github.com:MaximPodgore/lab7.git
cd lab7/
javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples
sed -i '43 s/index1/index2/' ListExamples.java
javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java
java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore TestListExamples
git add ListExamples.java
git commit -m  "index1 bug removed"
git push`

I used sed with the -i so it changes the file itself and replaces index1 with index2 at line 43 without me having to press a key other than `<enter>`. Other than that
there isn't anything unique. I enjoyed the lab a lot. I used the command `scp script.sh cs15lwi23afs@ieng6.ucsd.edu:./` to get the script onto the remote computer. After 
that I simply use `ssh cs15lwi23afs@ieng6.ucsd.edu` to log in, and then `bash script.sh` to run it. One thing to keep in mind is to use a fresh fork for this and 
`rm -rf lab7/` if the clone is still on the remote computer. 


PS: My code works perfectly, I have had my friends run it on their accounts, but for some reason it doesn't work on mine.
The test failure is one that isn't supposed to happen. Example:

![image](https://user-images.githubusercontent.com/56902053/224827236-7c19cbf9-0785-4580-b3e6-b4f337342a37.png)  

![image](https://user-images.githubusercontent.com/56902053/224829033-8bbf52cd-89a4-4491-a310-1630018745b9.png)
