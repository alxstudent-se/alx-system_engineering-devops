Create a script that switches the current user to the user betty.
0-iam_betty
#!/bin/bash
su betty

Write a script that prints the effective username of the current user.
1-who_am_i
#!/bin/bash
whoami

Write a script that prints all the groups the current user is part of.
2-groups
#!/bin/bash
groups

Write a script that changes the owner of the file hello to the user betty.
3-new_owner
#!/bin/bash
chown betty hello

Write a script that creates an empty file called hello.
4-empty
#!/bin/bash
touch hello

Write a script that adds execute permission to the owner of the file hello.
5-execute
#!/bin/bash
chmod u+x hello

Write a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file hello.
6-multiple_permissions
#!/bin/bash
chmod 754 hello

Write a script that adds execution permission to the owner, the group owner and the other users, to the file hello
7-everybody
#!/bin/bash
chmod ugo+x hello

Write a script that sets the permission to the file hello as follows:

Owner: no permission at all
Group: no permission at all
Other users: all the permissions
8-James_Bond
#!/bin/bash
chmod 007 hello

Write a script that sets the mode of the file hello to this:
9-John_Doe
#!/bin/bash
chmod 753 hello

Write a script that sets the mode of the file hello the same as olleh’s mode.
10-mirror_permissions
#!/bin/bash
chmod --reference=olleh hello

Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.
11-directories_permissions
#!/bin/bash
chmod -R +X .

Create a script that creates a directory called my_dir with permissions 751 in the working directory.
12-directory_permissions
#!/bin/bash
mkdir -m 751 my_dir

Write a script that changes the group owner to school for the file hello
13-change_group
#!/bin/bash
chgrp school hello

Write a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
100-change_owner_and_group
#!/bin/bash
chown vincent:staff *

Write a script that changes the owner and the group owner of _hello to vincent and staff respectively.
101-symbolic_link_permissions
#!/bin/bash
chown -h vincent:staff _hello

Write a script that changes the owner of the file hello to betty only if it is owned by the user guillaume.
102-if_only
#!/bin/bash
chown --from=guillaume betty hello

Write a script that will play the StarWars IV episode in the terminal.
103-Star_Wars
#!/bin/bash
telnet towel.blinkenlights.nl
