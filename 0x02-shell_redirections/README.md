# Shell Redirections Project

## Overview

This project is part of the **alx-system_engineering-devops** repository. It contains scripts written in Bash that demonstrate various concepts related to shell redirections in Unix-based systems. Each script focuses on different aspects of shell redirections, including input redirection, output redirection, and redirection of standard input/output streams.

## Tasks

**Note:** Always start your script files with `#!/bin/bash`. Make the script executable with `chmod u+x <filename>`.

### 0. Hello World
- **File:** [0-hello_world](0-hello_world)
- **Command:** `echo "Hello, World"`

### 1. Confused Smiley
- **File:** [1-confused_smiley](1-confused_smiley)
- **Command:** `echo "(Ôo)'"`

### 2. Let's Display a File
- **File:** [2-hellofile](2-hellofile)
- **Command:** `cat /etc/passwd`

### 3. What About 2?
- **File:** [3-twofiles](3-twofiles)
- **Command:** `cat /etc/passwd /etc/hosts`

### 4. Last Lines of a File
- **File:** [4-lastlines](4-lastlines)
- **Command:** `tail /etc/passwd`

### 5. I'd Prefer the First Ones Actually
- **File:** [5-firstlines](5-firstlines)
- **Command:** `head /etc/passwd`

### 6. Line #2
- **File:** [6-third_line](6-third_line)
- **Command:** `sed -n '3p' iacta`

### 7. It Is a Good File That Cuts Iron Without Making a Noise
- **File:** [7-file](7-file)
- **Command:** `echo "Holberton School" > '\*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:)`

### 8. Save Current State of Directory
- **File:** [8-cwd_state](8-cwd_state)
- **Command:** `ls -la > ls_cwd_content`

### 9. Duplicate Last Line
- **File:** [9-duplicate_last_line](9-duplicate_last_line)
- **Command:** `tail -n 1 iacta >> iacta`

### 10. No More Javascript
- **File:** [10-no_more_js](10-no_more_js)
- **Command:** `find . -type f -name "*.js" -delete`

### 11. Don't Just Count Your Directories, Make Your Directories Count
- **File:** [11-directories](11-directories)
- **Command:** `find . -mindepth 1 -type d | wc -l`

### 12. Whats New
- **File:** [12-newest_files](12-newest_files)
- **Command:** `ls -t | head -n 10`

### 13. Being Unique is Better Than Being Perfect
- **File:** [13-unique](13-unique)
- **Command:** `sort | uniq -u`

### 14. It Must Be in That File
- **File:** [14-findthatword](14-findthatword)
- **Command:** `grep root /etc/passwd`

### 15. Count That Word
- **File:** [15-countthatword](15-countthatword)
- **Command:** `grep -c bin /etc/passwd`

### 16. What's Next?
- **File:** [16-whatsnext](16-whatsnext)
- **Command:** `grep -A 3 root /etc/passwd`

### 17. I Hate Bins
- **File:** [17-hidethisword](17-hidethisword)
- **Command:** `grep -v bin /etc/passwd`

### 18. Letters Only Please
- **File:** [18-letteronly](18-letteronly)
- **Command:** `grep '^[[:alpha:]]' /etc/ssh/sshd_config`

### 19. A to Z
- **File:** [19-AZ](19-AZ)
- **Command:** `tr Ac Ze`

### 20. Without C, You Would Live in Hiago
- **File:** [20-hiago](20-hiago)
- **Command:** `tr -d cC`

### 21. Reverse
- **File:** [21-reverse](21-reverse)
- **Command:** `rev`

### 22. DJ Cut Killer
- **File:** [22-users_and_homes](22-users_and_homes)
- **Command:** `awk -F: '{ print $1 ": " $6 }' /etc/passwd`

### 23. Empty Casks Make the Most Noise
- **File:** [100-empty_casks](100-empty_casks)
- **Command:** `find . -empty -type f -o -empty -type d`

### 24. GIFs
- **File:** [101-gifs](101-gifs)
- **Command:** `find . -type f -name "*.gif"`

### 25. Acrostic
- **File:** [102-acrostic](102-acrostic)
- **Command:** `cut -c 1 | tr -d '\n'`

### 26. The Biggest Fan
- **File:** [103-the_biggest_fan](103-the_biggest_fan)
- **Command:** `awk '{print $1}' | sort | uniq -c | sort -nr | head -n 11`

## License

This project is licensed under the MIT License.

## Author

[Yusuf Abu Egila](https://github.com/abuegila)

## Repository Link

[alx-system_engineering-devops](https://github.com/abuegila/alx-system_engineering-devops/tree/master/0x02-shell_redirections)
