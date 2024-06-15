# Shell Variables and Expansions Project

## Overview
This project is part of the `alx-system_engineering-devops` repository. It focuses on understanding and utilizing shell variables and expansions in Unix-based systems. Below are the tasks, their objectives, and the respective commands used to accomplish them.

## Tasks
Note: Always start your script files with `#!/bin/bash`. Make the script executable with `chmod u+x <filename>`.

0. Create a Script that Changes Your User ID to betty
   - **File**: `0-iam_betty`
   - **Command**: `su - betty`

1. Write a Script that Prints the Effective User ID of the Current User
   - **File**: `1-who_am_i`
   - **Command**: `id -u`

2. Write a Script that Prints All the Groups the Current User is Part Of
   - **File**: `2-groups`
   - **Command**: `groups`

3. Write a Script that Changes the Owner of the File hello to the User betty
   - **File**: `3-new_owner`
   - **Command**: `chown betty hello`

4. Write a Script that Creates an Empty File Called hello
   - **File**: `4-empty`
   - **Command**: `touch hello`

5. Write a Script that Adds Execute Permission to the Owner of the File hello
   - **File**: `5-execute`
   - **Command**: `chmod u+x hello`

6. Write a Script that Adds Execute Permission to the Owner and the Group Owner, and Read Permission to Other Users, to the File hello
   - **File**: `6-multiple_permissions`
   - **Command**: `chmod u+x,g+x,o+r hello`

7. Write a Script that Adds Execution Permission to the Owner, the Group Owner and the Other Users, to the File hello
   - **File**: `7-everybody`
   - **Command**: `chmod a+x hello`

8. Write a Script that Sets the Permission to the File hello as Follows:
   - **File**: `8-James_Bond`
   - **Command**: `chmod 007 hello`

9. Write a Script that Sets the Mode of the File hello to this:
   - **File**: `9-John_Doe`
   - **Command**: `chmod 753 hello`

10. Write a Script that Sets the Mode of the File hello the Same as olleh’s Mode
    - **File**: `10-mirror_permissions`
    - **Command**: `chmod --reference=olleh hello`

11. Create a Script that Adds Execute Permission to All Subdirectories of the Current Directory for the Owner, the Group Owner and All Other Users
    - **File**: `11-directories_permissions`
    - **Command**: `chmod -R a+X .`

12. Create a Script that Creates a Directory Called my_dir with Permissions 751 in the Working Directory
    - **File**: `12-directory_permissions`
    - **Command**: `mkdir -m 751 my_dir`

13. Write a Script that Changes the Group Owner to school for the File hello
    - **File**: `13-change_group`
    - **Command**: `chown :school hello`

14. Write a Script that Changes the Owner to vincent and the Group Owner to staff for All the Files and Directories in the Working Directory
    - **File**: `100-change_owner_and_group`
    - **Command**: `chown vincent:staff *`

15. Write a Script that Changes the Owner and the Group Owner of _hello to vincent and staff Respectively
    - **File**: `101-symbolic_link_permissions`
    - **Command**: `chown -h vincent:staff _hello`

16. Write a Script that Changes the Owner of the File hello to betty Only If It Is Owned by the User guillaume
    - **File**: `102-if_only`
    - **Command**: `chown --from=guillaume betty hello`

17. Write a Script that Will Play the StarWars IV Episode in the Terminal
    - **File**: `103-Star_Wars`
    - **Command**: `telnet towel.blinkenlights.nl`

## License
This project is licensed under the MIT License.

## Author
Yusuf Abu Egila

## Repository Link
[alx-system_engineering-devops](https://github.com/abuegila/alx-system_engineering-devops)
