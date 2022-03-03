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
	 

