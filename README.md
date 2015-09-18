# maillist_checker
Checker for mail list. It uses SMTP-protocol and 550 response for check the email is alive

# Usage
This command must be run on the works SMTP-outgoing server.

Command usage:

    maillist_check (filename=maillist) (HELO domain=mx-1.example.com)
    
Usage example:

    maillist_check ./users.txt smtp-o-1.example.com > success.list
    grep -v -x -f success.list users.txt > badbox.list

"smtp-o-1.example.com" is valid HELO with PTR for current server.
To file "sucess.list" will be put existing boxes.
To file "badbox.list" will be put NOT existing boxes.

# Example contents of users.txt

    test1@example.com
    test2@example.com
    test3@example.com
    test4@example.com

