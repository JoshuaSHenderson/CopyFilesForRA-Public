# CopyFilesForD365-RA 
## Purpose 
This file does the following:
* Creates Log file
* Decides if the log file needs to be renamed
* Create Function "LogWrite"
  - This function appends what you wish to the log file
* Create Function "sendemail"
  - Uses on prem SMTP server to send emails when called upon, also adds the "Body" of email to log file
* Connects to cloud storage account
* Moves files from different folder on On-prem file share to Storage account 
  - on error
  -   Add line to log file
  -   Send email with error message
* Delete the orgin files after it has been verified that the file has been copied
* disconnects the mapped Cloud drive 


## To Do
* Create Public branch with all privledged information removed
