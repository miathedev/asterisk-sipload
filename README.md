# Basic sipload asterisk config for humans

## Whats inside?

### Endpoints (phones)
In this config, there are 2 endpoints configured for your SIP phones

* 6001
  - pw: 6001pw

* 6002 
  - pw: 6002pw

### What to change
Pls change the 6001/6002 extensions pw under extensions.conf
Enter your sipload credentials in pjsip.conf

### I Want to add more Endpoints (phones)
Copyn paste eg all [6001] context stuff and rename your copy to eg. 6003.
Dont forget to change password.
You will have to add 6003 in extensions.conf to be available for incoming calls.

### Routes

* 200 - check voice mail
* XXXX (any digit X) internal calls.
* any other -> outgoing

### Grandstream DECT Base - mailbox
Menu -> Voice Mail -> Set Voice Mail -> Enter 200
Should work. Then new Voicemail messages appear on your phones screen.
Could work out of the box with any other dect phone
