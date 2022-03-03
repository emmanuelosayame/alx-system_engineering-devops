0:  Script changes the user ID to betty. 
    su betty
	 

 1:   Print the effective user ID of current user. Other alternative is `whoami`
	 id -un
	 

2:   Prints all the groups the current user is part of.
	 id -Gn
	 

 3:  Changes the owner of the file `hello` to the user `betty`
	 chown betty hello
	 

 4:   Create an empty file called `hello`
	 touch hello
	 

 5:  Add execute permission to the owner of the file `hello`
	 chmod u+x hello
	 

 6:    Add execute permission to user and group owner, and read permission to others for file `hello`
	 chmod ug+x,o+r hello
	 

7:   Add execution permission to all for file `hello`.
	 chmod ugo+x hello
	 

 8:   Set permissions for file `hello` so owner and group don't have any permissions and other users have all permissions.
	 chmod 007 hello
	

 9:   Sets permissions so owner has all permissions, group has read and execute permissions and others have write and execute permissions.
	 chmod 753 hello
	 

 10: Copies the mode of file olleh to file hello.
	 chmod --reference=olleh hello

11:  Add execute permission to all subdirectories of the current directory for the everyone. Regular files should not be changed.

	 chmod -R +X .
	 
12:  Create a directory called `my_dir` with permissions 751 in the working directory. User has all read, write, and execute permissions. Group has read and execute permissions. Others have just execute permission.
	 mkdir -m 751 my_dir
	 

 13:  Change group owner to `school` for the file `hello`
	 chgrp school hello
	 
	 end of mandatory tasks
	 begging of advanced task
	 
100:  Change owner to `vincent` and the group owner to `staff` for all files and directories in current directory.
 chown vincent:staff *
	 

101:  Changes the owner and group owner of file `_hello` to `vincent` and `staff` respectively.
	 chown -h vincent:staff _hello
	 

102:  Changes owner of the file `hello` to `betty` only if it is currently owned by `guillaume`
	 chown --from=guillaume betty hello
	 

103:  Play the Star Wars IV episode in the terminal. This is a premade script provided online.
	URL: telnet towel.blinkenlights.nl


