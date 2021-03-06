# HTTP Digest Bruteforce

## Description
Module performs bruteforce attack against HTTP Digest Auth service.

## Authors
* Marcin Bury <marcin.bury[at]reverse-shell.com> # routersploit module

## Usage
```
rsf > use creds/http_digest_bruteforce
rsf (HTTP Digest Bruteforce) > show options

Target options:

   Name       Current settings     Description
   ----       ----------------     -----------
   target                          Target IP address or file with target:port (file://)
   port       80                   Target port


Module options:

   Name                Current settings                                                               Description
   ----                ----------------                                                               -----------
   usernames           admin                                                                          Username or file with usernames (file://)
   passwords           file:///Users/lucyoa/git/routersploit/routersploit/wordlists/passwords.txt     Password or file with passwords (file://)
   threads             8                                                                              Numbers of threads
   stop_on_success     1                                                                              Stop on first valid authentication attempt
   path                /                                                                              URL Path
   verbosity           1                                                                              Display authentication attempts


rsf (HTTP Digest Bruteforce) > set target http://192.168.1.1
[+] {'target': 'http://192.168.1.1'}
rsf (HTTP Digest Bruteforce) > run
[*] Running module...
```
