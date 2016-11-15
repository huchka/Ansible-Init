Initialization of ubuntu server.
jobs are
- update os
- install emacs
- copy public key to ssh folder

Usage:
$ ansible-playbook server.yml -i hosts --ask-pass --ask-become-pass --extra-vars "target=tom" --user huchka

Explanation:
-i : inventory file. all the hosts has to be written to hosts file
--ask-pass, -k : password for ssh conneciton
--ask-become-pass : password for root permission (just press enter key if it is same as ssh conneciton pass)
--extra-vars "target=tom" : choosing server(s) to initialize from hosts inventory file
--user huchka : ssh connection user name
