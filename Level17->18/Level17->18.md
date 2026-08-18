# Mission:
 The password is in passwords.new and is the only line that has been changed between passwords.old and passwords.new.

# Steps:

 ## Create sshkey.private
 First, i need to loginto bandit17 using sshkey.private. I will create a sshkey.private on my system(cause bandit16 doesn't have `.ssh`).
 
 I will create a sshkey.private first, then write the content.


 ```bash
 wofb@ubuntu1:~$ touch sshkey.private
 wofb@ubuntu1:~$ ls
 Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos  snap  sshkey.private
 wofb@ubuntu1:~$ cat > sshkey.private
-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAABlwAAAAdzc2gtcn
NhAAAAAwEAAQAAAYEAvdSaw8j1FQ2DjtbQPGiEVtqEG5kt3g71uDlixg42vRN2MvWRVnGQ

...
+MHK2KRq5Zd3YJd9Px6AF5iMbyiQYA69nsBumqt04Ihe8CFYHa9uG
KLE1QobuX5Wx6cWaOsc1j61vpaYDEwMUT8LeMFqKjN1rF1LMiNENBQhtd+ikJmYYwB01/5
Pfos/2C+rbNuHjAAAADnJ1ZHlAbG9jYWxob3N0AQIDBA==
-----END OPENSSH PRIVATE KEY-----
wofb@ubuntu1:~$ ls
Desktop  Documents  Downloads  Music  Pictures  Public  Templates  Videos  snap  sshkey.private
 ```


 ## Checking sshkey.private properties.
 ![Check](Check.png)

 ## Changing permission and login

 ```bash
 wofb@ubuntu1:~$ chmod 700 sshkey.private
 wofb@ubuntu1:~$ ssh bandit17@bandit.labs.overthewire.org -p 2220 -i sshkey.private
                         _                     _ _ _   
                        | |__   __ _ _ __   __| (_) |_ 
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_ 
                        |_.__/ \__,_|_| |_|\__,_|_|\__|
                                                       

                      This is an OverTheWire game server. 
            More information on http://www.overthewire.org/wargames

backend: gibson-1

      ,----..            ,----,          .---.
     /   /   \         ,/   .`|         /. ./|
    /   .     :      ,`   .'  :     .--'.  ' ;
   .   /   ;.  \   ;    ;     /    /__./ \ : |
  .   ;   /  ` ; .'___,/    ,' .--'.  '   \' .
  ;   |  ; \ ; | |    :     | /___/ \ |    ' '
  |   :  | ; | ' ;    |.';  ; ;   \  \;      :
  .   |  ' ' ' : `----'  |  |  \   ;  `      |
  '   ;  \; /  |     '   :  ;   .   \    .\  ;
   \   \  ',  /      |   |  '    \   \   ' \ |
    ;   :    /       '   :  |     :   '  |--"
     \   \ .'        ;   |.'       \   \ ;
  www. `---` ver     '---' he       '---" ire.org


  Welcome to OverTheWire!

  If you find any problems, please report them to the #wargames channel on
discord or IRC.

...
--[ More information ]--

  For more information regarding individual wargames, visit
  http://www.overthewire.org/wargames/

  For support, questions or comments, contact us on discord or IRC.

  Enjoy your stay!

 ```
 
 ## Diff
 Now, to find out the different between `passwords.old` and `passwords.new`, i will use `diff` command:

 ![Goal](Goal.png)

 As i know that the password is in `passwords.new`.

 The password: `OQxXZjELndr90zuhOTDYBEomI0SZITXI`.

