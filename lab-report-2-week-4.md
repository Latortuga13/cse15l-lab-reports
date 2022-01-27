# Lab Report 2 <br />
## Error 1
### The symptom<br/>
![image](https://user-images.githubusercontent.com/56976660/151304330-154e4cd4-1633-4edd-a36b-ee26227064e8.png)<br />
### The new test to check if it is fixed (in MarkdownParseTest)<br />
![image](https://user-images.githubusercontent.com/56976660/151301934-87594d00-d856-4922-8f6d-806b028e5cc4.png)
### The actual fix in MarkdownParse
![image](https://user-images.githubusercontent.com/56976660/151405280-4f319624-8e0e-4cbf-9fc9-c7e41df256ca.png)
### Summary
This error refers to the test3 file, where there are no brackets or parentheses in the text file. By adding some if statements referring to this problem, we are able to make a case for our program to deal with a text file with no parentheses or brackets.
## Error 2
### The symptom <br />
![image](https://user-images.githubusercontent.com/56976660/151410580-2d6de65d-bb95-46ea-bebb-911a65794b70.png)<br />
### The new test to check if it is fixed (in MarkdownParseTest)
![image](https://user-images.githubusercontent.com/56976660/151412154-754810ae-1dad-4703-bc10-9d4ed3a57a69.png)
### The actual fix in MarkdownParse
![image](https://user-images.githubusercontent.com/56976660/151405280-4f319624-8e0e-4cbf-9fc9-c7e41df256ca.png)<br />
### Summary
This error refers to the test5 file. In the test5 file, the test randomly puts stuff that is not links into brackets and parentheses. Markdown is only supposed to acquire links, so the code aquiring a link from a test file with no links is an error. Our if statements from test 3 correct this error.
## Error 3
### The symptom <br />
![image](https://user-images.githubusercontent.com/56976660/151411418-e63cfbca-a835-49ce-aca8-5693c0ea39ed.png)<br />
### The new test to check if it is fixed (in MarkdownParseTest)
![image](https://user-images.githubusercontent.com/56976660/151412243-457fc90b-dde2-4125-b06f-8f860c7c61e2.png)
### The actual fix in MarkdownParse
![image](https://user-images.githubusercontent.com/56976660/151405280-4f319624-8e0e-4cbf-9fc9-c7e41df256ca.png)<br />
### Summary
This error refers to test7 text file, which only has a closed parenthese and a open bracket. In our original code, the code hangs, as the exit condition of the while loop is never met. However, with the added if statements, and their break and continue commands, the code is able to return the correct value.

