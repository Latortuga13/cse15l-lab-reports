# Lab Report 5
## How I found the tests with different results
![image](https://user-images.githubusercontent.com/56976660/157932381-52772c10-17cf-451d-838e-26415aa90b86.png)
<br />
This is the script that I used to iterate through all of the files with the trycommonmark file. I edited the trycommonmark by adding a new class link visitor to visit each link.
<br />
![image](https://user-images.githubusercontent.com/56976660/157934189-0e163c1c-f661-43aa-943f-dbf31552af23.png)
<br />
I then added the greater sign and a text file to add all the files into a seperate text file.
<br />
![image](https://user-images.githubusercontent.com/56976660/157936009-c1f1e011-2d6d-4732-812b-42d5e15c6db8.png)
<br />
This let me manually compare the two codes by comparing the different prints in each file.
## Test 1
![image](https://user-images.githubusercontent.com/56976660/157948042-8fc6a5fa-69de-48cb-a7d9-1b2b4d37ab1c.png)
<br />
![image](https://user-images.githubusercontent.com/56976660/157944666-f958e7ed-22d9-44f6-86db-20d81c4e755b.png)
<br />
![image](https://user-images.githubusercontent.com/56976660/157944935-ca3d6a0b-221b-4ebe-8481-0f286804b0e2.png)
<br />
The expected output from running test 494 is [\foo\)]. The issue in the given (commonmark) code is that it is only ensuring that open brackets, closing brackets, open parenthesis, and closing parenthesis are in the file. It is not checking that parenthesis and slashes can be inside of a link. Our code projects the expected output.
## Test 2
![image](https://user-images.githubusercontent.com/56976660/157948916-c3fdb2aa-5217-4d41-936f-8a8febe21c83.png)
<br />
![image](https://user-images.githubusercontent.com/56976660/157947585-c5a4fa21-5c7a-45b8-abd6-10011cbd2018.png)
<br />
![image](https://user-images.githubusercontent.com/56976660/157945692-953fe5d5-1426-42cd-9860-4e6d760abc18.png)
<br />
The expected output from running test 192 is an empty array. This is because test file 192 is not following the format of a file. Our code once again projects the expected output. The given code is incorrect because it doesn't return an empty array. I am assuming if there is a ctrl click option for the text, the commonmark code will think it is a link and puts in in.
