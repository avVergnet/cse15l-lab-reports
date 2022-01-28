 <font size="12"> Lab Report 2 Week 4</font>

# Change #1 to fix a bug

* Screenshot of the code change diff from Github: ![Image](ss4lab1.PNG)

* Link to the test file for a failure-inducing input that prompted you to make that change:
  * [Test file #3](test-file3.md) and [test file #4](test-file4.md) contained the failure-inducing input. 

* Sympton of failure-inducing input by showing the output of running the file at the command line for version where it was failling: ![Image](ss4lab2.PNG)

* Relationship between the bug, the symptom, and the failure-inducing input.
  * This bug was very intersting as it had multiple failure-inducing input: [test file #3](test-file3.md) and  [test file #4](test-file4.md). This bug which was that we did not have a checker to for empty brackets two different failure-inducing input which caused similar symptoms in each. For [test file #4](test-file4.md), the symptom was: ![Image](ss4Lab3.PNG)

# Change #2 to fix a bug

* Screenshot of the code change diff from Github: ![Image](ss4Lab4.PNG)

* Link to the test file for a failure-inducing input that prompted you to make that change:
  * [Test file #6](test-file6.md) contained the failure-inducing input. 

* Sympton of failure-inducing input by showing the output of running the file at the command line for version where it was failling: ![Image](ss4Lab5.PNG)

* Relationship between the bug, the symptom, and the failure-inducing input.
  * The problem is that the way embeding images and links in markdown is very similar. The only difference is the exclamation mark in front of it. The bug is that when our program reads a markdown file with an image in it, it should not consider it as a link. We know this from the symptom seen above in the command line. We are expecting an empty list but are getting page.com as a link. This happened becuase [test file #6](test-file6.md) contained an image and our program read it as a link.


# Change #3 to fix a bug

* Screenshot of the code change diff from Github: ![Image](ss4Lab6.PNG)

* Link to the test file for a failure-inducing input that prompted you to make that change:
  * [Test file #5](test-file5.md) contained the failure-inducing input. 

* Sympton of failure-inducing input by showing the output of running the file at the command line for version where it was failling: ![Image](ss4Lab7.PNG)

* Relationship between the bug, the symptom, and the failure-inducing input.
  * 
