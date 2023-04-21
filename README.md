# Functions-WU-Ticket-System
Custom Functions that I implemented in Whitworth University Ticket System to make solving tickets more efficient

## Deluge Scripting
All functions are coded in Deluge and is utilzied within the ManageEngine Service Desk Portal provided by Zoho Corporation

### addNote.dg
This functions is utilzied to add a note to a request. We use it as a kind of reminder for us if a requestor has not replied to a request for 2 days, a note is added that tells us to, Please send Follow up Reply

### addTask.dg
This function adds a task template to a request. We use this function as a way to add tasks for computer replacement requests. If Computer Replacement, is at all in the subject line of the request this funciton will initiate and add a task that has a checklist of things to do for a new computer replacement

### checkCMD.dg
This functions grabs a value from the request and uses that value to reply to the request. This value can be adjusted and changed accordingly by any technician. It is in the form of a drop down menu so allows you to select which reply you would want to reply with. Once it gets the reply that you want to reply with it will run the function and change status accordingly.

### updateStatus.dg
This function is used to change the status from a ticket onhold to open after two days. Once the ticket is changed back to open it will add a note to inform us to reply back to the email

### assignTech.dg
This function assigns a technician if they have replied to an email. The function does not run until a reply is received from any requestor. The technician that is directly assigned to the ticket is the technician that recently replied to the ticket. If someone is assigned it will not overwrite the technician. 
