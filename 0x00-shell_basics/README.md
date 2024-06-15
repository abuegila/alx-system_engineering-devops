### 0. Print the Absolute Path of the Current Working Directory
- **File:** `0-current_working_directory`
- **Command:** `pwd` (print working directory)

### 1. List the Contents of the Current Directory
- **File:** `1-listit`
- **Command:** `ls` (list directory contents)

### 2. Change Directory to the User's Home Directory
- **File:** `2-bring_me_home`
- **Command:** `cd` (change directory)

### 3. List Directory Contents in Long Format
- **File:** `3-listfiles`
- **Command:** `ls -l` (list directory contents in long format)

### 4. List All Files, Including Hidden Files, in Long Format
- **File:** `4-listmorefiles`
- **Command:** `ls -la` (list directory contents in long format, including hidden files)

### 5. List Directory Contents with File Digits
- **File:** `5-listfilesdigitonly`
- **Command:** `ls -la`

### 6. Create a Directory in /tmp
- **File:** `6-firstdirectory`
- **Command:** `mkdir /tmp/my_first_directory`

### 7. Move a File to a Directory
- **File:** `7-movethatfile`
- **Command:** `mv /tmp/betty /tmp/my_first_directory/betty`

### 8. Delete a File
- **File:** `8-firstdelete`
- **Command:** `rm /tmp/my_first_directory/betty`

### 9. Delete a Directory
- **File:** `9-firstdirdeletion`
- **Command:** `rmdir /tmp/my_first_directory`

### 10. Change to the Previous Directory
- **File:** `10-back`
- **Command:** `cd -`

### 11. List All Files in Multiple Directories
- **File:** `11-lists`
- **Command:** `ls -la . .. /boot`

### 12. Print the Type of a File
- **File:** `12-file_type`
- **Command:** `file /tmp/iamafile`

### 13. Create a Symbolic Link
- **File:** `13-symbolic_link`
- **Command:** `ln -s /bin/ls __ls__`

### 14. Copy HTML Files to Parent Directory
- **File:** `14-copy_html`
- **Command:** `cp -u *.html ..`

### 15. Move Files Starting with an Uppercase Letter
- **File:** `100-lets_move`
- **Command:** `mv [[:upper:]]* /tmp/u`

### 16. Delete Files Ending with a Tilde (~)
- **File:** `101-clean_emacs`
- **Command:** `rm *~`

### 17. Create Nested Directories
- **File:** `102-tree`
- **Command:** `mkdir -p welcome/to/school`

### 18. List Files and Directories with Commas
- **File:** `103-commas`
- **Command:** `ls -map`

### 19. Create a Magic File for Custom File Detection
- **File:** `school.mgc`
- **Commands:**
  1. `0 string SCHOOL School data`
  2. `!:mime School`
  3. `file -C -m school.mgc`
