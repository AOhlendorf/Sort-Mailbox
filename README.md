# Sort-Mailbox
Sort Exchange mailbox after migration from Lotus Notes

After a migration from Lotus Notes to MS Exchange, users may find a folder called "Unfiled" in their Exchange mailbox, containing a large number of mails. These mails have been filed in different folders while in Lotus Notes.
This script accesses the Notes mailbox, reads the folder structure and subject, sender, PosteDate of each mail.
Afterwards the script accesses the exchange mailbox, reads the content of the folder Unfiled and compares subject, sender, DateTimeReceived with the values in the Notes mail.
If an Exchange mail is found in the collection of Notes mails, the script tries to move this mail to the same folder as it has been in in Notes. Missing folders may be created, depending on a startup parameter.

Detailed description follows.... :)
