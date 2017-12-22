# AWS-Account
This repository has a tutorial of how you create an AWS account on Macbook.

You need to follow the below given steps to create an AWS account and start a Ubuntu machine on Mac. You can also refer the word document for screenshots of these steps.

1. Visit aws.amazon.com and click on “Create a Free Account”
2. Enter the email address, password, confirm password and AWS account name and click on Continue.
3. Enter the contact information and make sure Personal is selected in the Account type.
4. Once you enter the personal details, there will be payment information that will be prompted to enter. For verification, there would be $1.00 deducted from the account.
5. To verify the account, you will need to enter a phone number. You will receive a call from automated system where you will be asked to enter a verification code which is prompted on the screen.
6. Once the verification is complete, you will need to select the Basic Plan and proceed.
7. This concludes the account creation. Next you will have to click on “Sign in to My Console”. Once you click that you will have to enter the username (which will be the email address which is associated with the account) and the password.
8. Once you login the following page. You will have to select Launch a virtual machine.
9. Once you select “Launch a virtual machine” the following page will be prompted where you have to select “Get Started”.
10. You will need to wait for few hours so that the account is completely created. Once the account is created, you will get a email from AWS Amazon. After the email, you can procced with the above mentioned and create an instance.
11. Select Ubuntu once the instance is created.
12. Select t2 as the instance type.
13. There will be a key pair that will be generated. Make sure that is saved safely as it will be required later.
14. Once the key is downloaded, you will need to create the instance by clicking on “Create the instance”.
15. It will take sometime for the instance to be created. Once it is created you will need to click on “Procced to the EC2 console”.
16. This page shows that the instance has been created successfully. 
17. Once the instance is created, you will need to connect your instance. Since this was created on a MacBook, to connect the instance the terminal was opened and “chmod 400 Instance2.pem” command is executed. 
    Later where the key was saved the “ssh – i “Instance2.pem Ubuntu@ec2-18-281-1-85.is.east-2.compute.amazonaws.com” command is executed to start the Ubuntu machine. 
18. Once the Ubuntu machine was connected to the instance, Java was installed on the machine using “sudo apt install default-jre” and “sudo apt install default-jdk”. 
    The files were transferred using WinSCP on a windows machine where the programs were saved. While establishing a connection with WinSCP, you will require the .ppk file which is generated using PuTTyGen application and the instance key. 
    The steps of how we created a file is provided later as well.
19. Once the files were transferred from the system to the Ubuntu machine, when you run the “ls” command their files on the system were listed. The test programs that were provided were saved and executed in the Ubuntu machine. 
    To run the server and client program, the rule in the security group section was changed to allow all traffic.There were different C program files created for each of the program.
20. To run the MPI programs the specific library was installed using the “sudo apt-get update” and “sudo apt install libopenmpi-dev” command. 
21. You can make a text file in Ubuntu in the following ways. 
    You can either make a directory or directly make a text file. Here I have made a directory named “programs” using the “mkdir programs” command. 
    Once this command is executed you can execute the “ls” to check if the directory has been created. Once the directory is created you can go into the directory with “cd programs” command. With the help of that you will now be inside the programs directory. 
    To make a text file you will need to use “cat > filename.txt”. Here we have used “cat > hello.txt”. Once that is done you can type the contents you need that text file and then press “control + D” so that the file is saved. You can again check if the file is created using “ls” command. 
    To remove the entire directory, you will need to use “rm –r “directory name” for instance we can use “rm –r programs” to delete the current directory that was created.

