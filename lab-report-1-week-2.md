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
here is an example of what it should look like:
<br />   <br />
![image](https://user-images.githubusercontent.com/56976660/149567887-c8f77616-2a38-410b-8b56-d1322a517829.png)
