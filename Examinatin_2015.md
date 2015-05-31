## Pen testing examination  2015

## MS13961572

## K.M.D.S.B. Kulatunga

## Question 1

Map link - http://www.digitalattackmap.com/#anim=1&color=0&country=ALL&list=0&time=16065&view=map

1.) Date - December 27 2013

2.)

1. Source- USA ;Destination -USA
2. Duration - 9 mins
3. Attack was pulled of using IP fragmentation and bandwidth utilization. Attack was targeted on NatWest online banking.This attack was primarily targeted on SSH port on the hosted servers. Bank has different servers running on different operating systems at the initial part it was unclear about the attack but in the analysis they came to know that port 22 is used on all the servers. As a primary action they changed SSH port to non standard port so that attack can be mitigated.

3.) 
1.  USA
2.  China
3.  North Korea

	
## Question 2

#Wargames - Leviathan

**Level- 0**
User-name: leviathan0

Password: leviathan0

**Commands**

1. ls-al
2. cd .backup
3. ls-al
4. catbookmarks.html| grep password

**Level- 1**
User-name: leviathan1

Password: rioGegei8m

**Commands**

1. ls-al
2. ./check
3. enter password love
4. ltrace ./check
5. now you see that password is sex 
6. ./check enter password sex

**Level- 2**
User-name: leviathan2

Password: ougahZi8Ta

**Commands**

1. ls-al
2. ./check
3. printfile
4. mkdir /tmp/leviathan_22 && touch /tmp/leviathan_12/file\ tmp.txt
5. cd /tmp/leviatham_12
6. ls-al
7. ltrace ~/printfile "file tmp.txt"
8. ln -s /etc/leviathan_pass/leviathan3 /tmp/leviathan_12/file
9. ~/printfile "file"
10. ~/printfile "file tmp.txt"

**Level- 3**

User-name: leviathan3

Password: Ahdiemoo1j

**Commands**

1. ls-al
2. ./level3
3. enter default text to the password.
4. strings ./level3
5. snlprintf is quite interesting so that we use it as the password
6. after entering snlprintf you get a shell prompt
7. issue a whoami you will see that it is leviathan4 
8. go to the /etc/leviathan_pass/leviathan4

**Level- 4**

User-name: leviathan4

Password: vuH0coox6m

**Commands**

1. ls-al
2. cd ./trash
3. ls-al
4. ./bin
5. you will get a set of binaries. This could be our password and we have to find a way to convert this binary to ASCII


**Level- 5**

User-name: leviathan5

Password: Tith4cokei

**Commands**

1. ls-al
2. ./leviathan5
3. ln-s /etc/leviathan_pass/leviathan6 /tmp/file.log
4. ./leviathan5
5. boom you get the password.

**Level- 6**

User-name: leviathan6

Password: UgaoFee4li

**Commands**

1.  need to brute force it
2.  for i in {0000..9999}; do ./leviathan6 $i; echo $i; done
3.  at end of the loop
4.  cat /etc/leviathan_pass/leviathan7

**Level- 7**

User-name: leviathan7

Password: ahy7MaeBo9


## Question 3

A.)

1. the /etc/passwd file?
	1. is a tool that is used to change the user password in UNIX like environments.
	
	
2. the /etc/shadow file?
	1. contains the encrypted password and other details like account & password expiration times.


3. the setuid bit?
	1. set user id upon execution. these are access rights flags it contains the owner , group , user execution permissions.


4. chroot?
	1. is the command that changes apparent root directory

B.)
ls-lshow the files and directories with the permissions
lsattr lists file attributes

C.)

Android is one one of the most used mobile operating system.The problem with that is apps are not properly filtered. primary rule of security is to stick with least privileges for the application. But writer tend to collect more data on the users of the app. And some writers tend to create apps for privilege escalation purposes.As legitimate users we don't much care about the privileges requested by the application.This leads to a data leaks and privacy breaching.

D.) 

Access control lists provides an additional, flexible permission setting for file system. ACL allows you to give explicit allow or deny actions for any user or group to any system resource. 
In standard unix permission models, the ownership of the files is an important component. Access to the files  and read, write, execute permission depends on the permissions given by the owner.

E.)

1. Deleting Syslog entries
	1.you have to have root level permission to execute these commands quite effective method and some times these files are stored in a different logging servers. you have to have full access in to that server as well.
2. Altering account logs
	1. utmp, wtmp, and lastlog are the main targets of the attacker root level or credentials of a high level privileged user is required.

## Question 4

1. mov DWORD PTR [ebp-0x4], 0x8
	1. oves the memory address 0x8 into the location pointed to by EBP 
	2. like pushing a value onto the stack so we can work with it.
2. mov eax, DWORD PTR [ebp+0x8]
	1. moves value at epb+0x8 into EAX 
3. lea eax, [ecx + eax*1]
	1. the quantity ecx+eax*1 is placed in EAX
4. call _htons
	1. call _htons function
	2. call puts the address of the next instruction on the stack
	3. so the program can return to it
5. cmp [ebp+0x8], 0
	1. compare the values of the two operands ebp+0x8 and 0

## Question 5

