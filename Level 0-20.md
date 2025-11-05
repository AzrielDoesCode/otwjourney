[[BANDIT]]


**LEVEL 0**  
Login to bandit labs using ssh as Bandit0 user by the code 
	`ssh bandit0@bandit.labs.overthewire.org -p 2220` 
Then use Nano Terminal Text reader to get the key by the command  
	`nano readme`
	ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If



**LEVEL 1** 
Access the server using SSH as Bandit1 similarly, this time using the code retrieved from the last level
Here the name of the file is "-" NOW here we will need to do smthn different to access as the file using NANO since the name consists of a symbol at the first character; modification reqd is { ./  }
such that
	`nano ./-`       (easier unified way to remember :p)
giving us
	263JGJPfgU6LtdEvgfWU1XP5yac29mFx

**LEVEL 2** 
	`nano ./--spaces in this filename--"
	(TIP : ./--sp   <TAB key)
	
	MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx

**LEVEL 3** 


to display all the files incl hidden
`ls -a` 


to display all the files incl hidden explicitly
`ls -la`

`nano ./...Hiding-From-You`
2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ


**LEVEL 4**
use FILE command to get details on the contents of all 8 files as follows
	`file ./*`
 then cat the file (-File07 here) to get the code 
 
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw


**LEVEL 5**
emphasize on the DU, FILE and FIND commands now

	`find . -type f -size 1033c ! -executable`
where;
- -type f → only files.

- -size 1033c → exactly 1033 bytes (c = bytes).

- ! -executable → exclude executables.

and you get the code!
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

**LEVEL 6**
Here also we will need to use FIND command this time exactly following the Info given directly while writiing the  command 

`find / -type f -user bandit7 -group bandit6 -size 33c`
- owned by user bandit7
- owned by group bandit6
- 33 bytes in size

find .
- The . refers to the current working directory.
- Example: If you’re in /home/dhruv/projects, then:
	`find . `
- will list everything under /home/dhruv/projects recursively.


find /
- The / refers to the root directory of the entire filesystem.
- Example:
	`find /`
- will traverse every directory on the system: /bin, /etc, /home, /var, /usr, etc.

morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

**LEVEL 7**
Here onwards we will have a new set of commmands to focus on 
man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

so here we use a combination of two of them,Strings and grep

`strings data.txt | grep "millionth"`

millionth	dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

**LEVEL 8**
 MAN or WHATIS commands

`sort data.txt`
`sort data.txt | uniq -c`

4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

**LEVEL 9**
`strings data.txt | grep "="` 

FB`=
c\5D=
========== the
?/=l
=Uc1
=vG*2P
========== password
k=ezG
E========== is
=%r_
.?=Dm
O&A=n
5========== FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
=*^Y
=L3jT
q<=,
'QHE=
+=NBf

**LEVEL 10**
