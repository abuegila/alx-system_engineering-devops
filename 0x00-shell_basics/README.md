# Shell Basics Project

## Overview

This project is part of the **alx-system_engineering-devops** repository. It focuses on understanding basic commands, navigation, and file management in a Unix-based system. Below are the tasks, their objectives, and the respective commands used to accomplish them.

## Tasks

**Note:** Always start your script files with `#!/bin/bash`. Make the script executable with `chmod u+x <filename>`.

### 0. Write a Script that Prints the Absolute Path Name of the Current Working Directory
- **File:** [0-current_working_directory](0-current_working_directory)
- **Command:** `pwd`

### 1. Display the Contents List of Your Current Directory
- **File:** [1-listit](1-listit)
- **Command:** `ls`

### 2. Write a Script that Changes the Working Directory to the User’s Home Directory
- **File:** [2-bring_me_home](2-bring_me_home)
- **Command:** `cd`

### 3. Display Current Directory Contents in a Long Format
- **File:** [3-listfiles](3-listfiles)
- **Command:** `ls -l`

### 4. Display Current Directory Contents, Including Hidden Files (Starting with .). Use the Long Format
- **File:** [4-listmorefiles](4-listmorefiles)
- **Command:** `ls -la`

### 5. Display Current Directory Contents, Including Hidden Files. Use Only the Long Format
- **File:** [5-listfilesdigitonly](5-listfilesdigitonly)
- **Command:** `ls -la`

### 6. Create a Script that Creates a Directory Named `my_first_directory` in the `/tmp/` Directory
- **File:** [6-firstdirectory](6-firstdirectory)
- **Command:** `mkdir /tmp/my_first_directory`

### 7. Move the File `betty` from `/tmp/` to `/tmp/my_first_directory`
- **File:** [7-movethatfile](7-movethatfile)
- **Command:** `mv /tmp/betty /tmp/my_first_directory/betty`

### 8. Delete the File `betty` in `/tmp/my_first_directory`
- **File:** [8-firstdelete](8-firstdelete)
- **Command:** `rm /tmp/my_first_directory/betty`

### 9. Delete the Directory `my_first_directory` That Is in the `/tmp` Directory
- **File:** [9-firstdirdeletion](9-firstdirdeletion)
- **Command:** `rmdir /tmp/my_first_directory`

### 10. Write a Script that Changes the Working Directory to the Previous One
- **File:** [10-back](10-back)
- **Command:** `cd -`

### 11. Write a Script that Lists All Files (Even Ones with Names Beginning with a Period Character, Which Are Normally Hidden) in the Current Directory and the Parent of the Working Directory and the `/boot` Directory (in This Order), in Long Format
- **File:** [11-lists](11-lists)
- **Command:** `ls -la . .. /boot`

### 12. Write a Script that Prints the Type of the File Named `iamafile`. The File `iamafile` Will Be in the `/tmp` Directory When We Will Run Your Script
- **File:** [12-file_type](12-file_type)
- **Command:** `file /tmp/iamafile`

### 13. Create a Symbolic Link to `/bin/ls`, Named `__ls__`. The Symbolic Link Should Be Created in the Current Working Directory
- **File:** [13-symbolic_link](13-symbolic_link)
- **Command:** `ln -s /bin/ls __ls__`

### 14. Create a Script that Copies All the HTML Files from the Current Working Directory to the Parent of the Working Directory, But Only Copy Files That Did Not Exist in the Parent of the Working Directory or Were Newer Than the Versions in the Parent of the Working Directory
- **File:** [14-copy_html](14-copy_html)
- **Command:** `cp -u *.html ..`

### 15. Create a Script that Moves All Files Beginning with an Uppercase Letter to the Directory `/tmp/u`. You Can Assume That the Directory `/tmp/u` Will Exist When We Will Run Your Script
- **File:** [100-lets_move](100-lets_move)
- **Command:** `mv [[:upper:]]* /tmp/u`

### 16. Create a Script that Deletes All Files in the Current Working Directory That End with the Character `~`
- **File:** [101-clean_emacs](101-clean_emacs)
- **Command:** `rm *~`

### 17. Create a Script that Creates the Directories `welcome/`, `welcome/to/`, and `welcome/to/school` in the Current Directory. You Are Only Allowed to Use Two Spaces (and Lines) in Your Script, Not More
- **File:** [102-tree](102-tree)
- **Command:** `mkdir -p welcome/to/school`

### 18. Write a Command that Lists All the Files and Directories of the Current Directory, Separated by Commas (`,`), and Hidden Directory Names (`..`) Should End with a Slash (`/`)
- **File:** [103-commas](103-commas)
- **Command:** `ls -map`

### 19. Create a Magic File `school.mgc` That Can Be Used with the Command `file` to Detect School Data Files. School Data Files Always Contain the String `SCHOOL` at Offset 0
- **File:** [school.mgc](school.mgc)
- **Input:**
  - `0 string SCHOOL School data`
  - `!:mime School`
- **Command:**
  - `file -C -m school.mgc`

## License

This project is licensed under the MIT License.

## Author

[Yusuf Abu Egila](https://github.com/abuegila)

## Repository Link

[alx-system_engineering-devops](https://github.com/abuegila/alx-system_engineering-devops/tree/master/0x00-shell_basics)
