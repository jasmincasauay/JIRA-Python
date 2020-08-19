# JIRA-Python
Bulk ticket creating/updating from information in a selected excel spreadsheet

!!!READ ME!!!

Set up:
In this folder there are two files. In order to set up and run the script the following must be done:
1.	Download and extract the .zip file
2.	Click and Run the ".exe" file

Procedure:
NOTE: When creating JIRA tickets, the corresponding excel file must be closed.
1.	A log in window will appear as soon as the script runs. The user is asked to provide his/her JIRA account username 
and password for security purposes and so that JIRA knows the reportee of the ticket(s) to be created.
2.	After the log in credentials are accepted, the script will now ask for the user to provide the excel spreadsheet
(accepts workbooks only in the form of .xlsx and .xlsm) where the data for JIRA ticket creation will be coming from.
Click Browse and choose the desired excel spreadsheet. Select the desired worksheet as well and Click OK
3.	The main GUI window will open containing all the information from the excel spreadsheet. Select the 
rows that you want to create a JIRA ticket for or update by selectiing the checkboxes on the left side of the window.
4.	Once the Selection is complete, click "Create JIRA Issue" or "Update Jira Issue" according to what the user 
wants to do. (Note: JIRA only created new issue(s) when the "Work Ticket" column is NOT populated. JIRA only updates the
selected issue(s) when the "Work Ticket" column IS populated.
5.	A dialog box will pop up when the action is successfull. The dialog box will also print the number of tickets 
created or updated.


Specs:
-	Created multiple JIRA tickets at a time
-	Prints the correspinding Work ticket number in the specific column as a hyperlink
-	Updates multiple JIRA tickets at a time
-	Asks for user's JIRA account username and password for security purposes
-	Establishes heirarchy in linking issues

Pyinstyaller:
1. Open command prompt
2. Got to directory where py script is located
3. Type this line "pyinstaller --onefile -w ./<pyscripttitle.py>
4. Creates one executable file <pyscripttitle.exe> in the "dist" folder
5. Follow set up procedures above
