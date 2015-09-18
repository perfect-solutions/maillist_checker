# maillist_checker
Checker for mail list. It uses SMTP-protocol and 550 response for check the email is alive

# Usage
This command must be run on the works SMTP-outgoing server.

Command usage:

    maillist_check (filename=maillist) (HELO domain=mx-1.example.com)
    
Command example:

    maillist_check ./users.txt smtp-o-1.example.com

"smtp-o-1.example.com" is valid HELO with PTR for current server.

# Example contents of users.txt

    test1@example.com
    test2@example.com
    test3@example.com
    test4@example.com

