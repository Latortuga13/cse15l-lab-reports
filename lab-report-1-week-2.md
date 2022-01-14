# Tutorial on how to log into the ieng6
## Step 1 Download VSCode
Download VS code and open it on your computer [Click here to download!](https://code.visualstudio.com/download) This website should have 4 different options, but you should pick the specific vscode download that applies to you. When opening the application it should look like this.
<br />   <br />
![image](https://user-images.githubusercontent.com/56976660/149557528-83f9b43b-5cb6-4b86-8669-5543a20a3bf3.png)\
## Step 2 Remotely Connecting
Many classes in Computer science use course-specific accounts. It is possible to use VScode to connect to a remote computer over the Internet to do work there.
If you’re on a computer that uses Windows operating system, you must install a program called OpenSSH, which is a program that can connect your computer to other computers that have this kind of account.
1. For the first step, open a terminal in VSCode. Your command will look like this, but with the aa replaced by the letters in your course-specific account.
<br /> *$ ssh cs15lwi22aa@ieng6.ucsd.edu* <br />
2. Second, you should get a message like this: 
<br />*⤇ ssh cs15lwi22aa@ieng6.ucsd.edu The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established. RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec. Are you sure you want to continue connecting (yes/no/[fingerprint])?* <br />
3. Respond __yes__ to this and press enter.
4. If you completed all of the above steps correctly, your terminal should look like this right now.
<br />   <br />
![image](https://user-images.githubusercontent.com/56976660/149551755-ea8b75fd-165a-44a2-bce3-79773601125b.png)
## Step 3 Trying Some Commands
Try typing these commands into your terminal.
-    cd ~
-    cd
-    ls -lat
-    ls -a
-    ls <directory> where <directory> is /home/linux/ieng6/cs15lwi22/cs15lwi22abc, where the abc is one of the other group members’ username
-    cp /home/linux/ieng6/cs15lwi22/public/hello.txt ~/
-    cat /home/linux/ieng6/cs15lwi22/public/hello.txt
-    pwd
 <br />
Here is an example of what using the pwd command should look like:
<br />   <br />
 
![image](https://user-images.githubusercontent.com/56976660/149568221-9f6827fa-e46a-4b12-86ec-670d65e8e631.png)
## Step 4 Moving Files with scp
We’ve seen how we can do some work on local and remote computers. One key step in working remotely is being able to copy files back and forth between the computers. There are lots of options for how to do this, for example, you could have sent yourself an email from another computer. One way of doing this is by using a command called scp.
<br /> Here is how you can use scp for yourself.
 1. first, make a class in java that does anything, in my example I had a class called WhereAmI which just consisted of a bunch of print statements/
 2. Next run this command: <br /> scp WhereAmI.java cs15lwi22aa@ieng6.ucsd.edu:~/ <br /> (obviously use your coursespecific account and your specific class instead of the ones in the example).
 3. Once you do this, you should see a password screen show up and you should just input your password from when you created your course-specific account.
 4. If you input your correct password, the result should appear like the image below.
 <br /> <br />
 ![image](https://user-images.githubusercontent.com/56976660/149577904-ea66fad4-5d57-4372-bd16-d07f8f459adb.png)
 ## Step 5 Setting an SSH Key
 As you have probably realized there is a big problem with using the scp command. Inputting yout password every time. Luckily, there is an easy fix, using ssh keys! if you use an ssh key, you won't need to log in every time when trying to move your files, and save a lot of time. This is how it is done. 
- Start by using the command *ssh keygen*
- Then enter this as  the file to save the key (/Users/joe/.ssh/id_rsa): /Users/joe/.ssh/id_rsa
- Third, create a passphrase, leave the spot blank if you do not want one. You will have to do it twice to confirm.
- Finally, test it by using the ssh cs15lwi22aa@ieng6.ucsd.edu command in terminal and seeing if it requires a password.
<br /> 
If it worked, it should look as follows
<br /> <br />
![image](https://user-images.githubusercontent.com/56976660/149582978-7dc1a909-517e-4101-9E29-5ba56715df6e.png)
<br /> <br />
If you are on windows, before you do these instructions, you must follow the instructions on this website [https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation)
