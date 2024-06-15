# Shell Variables Expansions Project

## Overview
This project is part of the alx-system_engineering-devops repository. It focuses on understanding and managing shell variables and expansions in a Unix-based system. The tasks include creating aliases, manipulating the `PATH`, and performing arithmetic operations with environment variables, among other activities. Each task is designed to deepen the understanding of shell scripting and the Unix environment.

## Tasks

### 0. Create a Script that Creates an Alias
**File:** 0-alias  
**Description:** This script creates an alias named `ls` with the value `rm *`, which redefines the `ls` command to remove all files in the current directory.  
**Command:** `alias ls='rm *'`

### 1. Print Hello User
**File:** 1-hello_you  
**Description:** This script prints `hello` followed by the current Linux user, using the `$USER` environment variable.  
**Command:** `echo "hello $USER"`

### 2. Add /action to PATH
**File:** 2-path  
**Description:** This script adds `/action` to the `PATH` environment variable, allowing the system to locate executables in the `/action` directory.  
**Command:** `export PATH=$PATH:/action`

### 3. Count Directories in PATH
**File:** 3-paths  
**Description:** This script counts the number of directories in the `PATH` variable, providing insight into how many directories are included in the system's executable search path.  
**Command:** `echo $PATH | tr ':' '\n' | wc -l`

### 4. List Environment Variables
**File:** 4-global_variables  
**Description:** This script lists all environment variables currently defined in the shell session, showing the variables that are available globally.  
**Command:** `printenv`

### 5. List Local Variables and Environment Variables
**File:** 5-local_variables  
**Description:** This script lists all local variables, environment variables, and shell functions, providing a comprehensive view of the shell's variable and function landscape.  
**Command:** `set`

### 6. Create a New Local Variable
**File:** 6-create_local_variable  
**Description:** This script creates a new local variable named `BEST` with the value `School`, demonstrating how to define local variables within a script.  
**Command:** `BEST='School'`

### 7. Create a New Global Variable
**File:** 7-create_global_variable  
**Description:** This script creates a new global variable named `BEST` with the value `School`, showing how to define environment variables that are accessible system-wide.  
**Command:** `export BEST='School'`

### 8. Print the Result of Addition
**File:** 8-true_knowledge  
**Description:** This script prints the result of adding 128 to the value stored in the environment variable `TRUEKNOWLEDGE`, performing arithmetic with environment variables.  
**Command:** `echo $((TRUEKNOWLEDGE + 128))`

### 9. Print the Result of Division
**File:** 9-divide_and_rule  
**Description:** This script prints the result of dividing the `POWER` environment variable by the `DIVIDE` environment variable, demonstrating division operations with environment variables.  
**Command:** `echo $((POWER / DIVIDE))`

### 10. Display the Result of Exponentiation
**File:** 10-love_exponent_breath  
**Description:** This script displays the result of raising the `BREATH` environment variable to the power of the `LOVE` environment variable, showing exponentiation with environment variables.  
**Command:** `echo $((BREATH ** LOVE))`

### 11. Convert Binary to Decimal
**File:** 11-binary_to_decimal  
**Description:** This script converts a number from base 2 (binary) to base 10 (decimal), demonstrating base conversion operations.  
**Command:** `echo $((2#<binary number>))`

### 12. Print Possible Combinations
**File:** 12-combinations  
**Description:** This script prints all possible combinations of two letters, excluding `oo`, using brace expansion and filtering.  
**Command:** `echo {a..z}{a..z} | grep -v "oo"`

### 13. Print a Number with Two Decimal Places
**File:** 13-print_float  
**Description:** This script prints a number stored in the environment variable `NUM` with two decimal places, showcasing formatting capabilities.  
**Command:** `printf "%.2f\n" $NUM`

### 14. Convert Decimal to Hexadecimal
**File:** 100-decimal_to_hexadecimal  
**Description:** This script converts a number from base 10 (decimal) to base 16 (hexadecimal), demonstrating base conversion to hexadecimal.  
**Command:** `printf '%x\n' <number>`

### 15. Encode and Decode Text Using ROT13
**File:** 101-rot13  
**Description:** This script encodes and decodes text using the ROT13 encryption, a simple substitution cipher that replaces a letter with the letter 13 letters after it in the alphabet.  
**Command:** `echo "<text>" | tr 'A-Za-z' 'N-ZA-Mn-za-m'`

### 16. Print Every Other Line from Input
**File:** 102-odd  
**Description:** This script prints every other line from the input, starting with the first line, demonstrating selective line printing.  
**Command:** `awk 'NR % 2 == 1'`

### 17. Add Two Numbers in Base bestchol
**File:** 103-water_and_str  
**Description:** This script adds the two numbers stored in the environment variables `WATER` and `STIR` and prints the result as a number in base `bestchol`, performing arithmetic in a custom base system.  
**Command:** `echo $((WATER + STIR)) | tr '0123456789' 'bestchol'`

## License
This project is licensed under the MIT License.

## Author
Yusuf Abu Egila

## Repository Link
[alx-system_engineering-devops](https://github.com/abuegila/alx-system_engineering-devops/tree/master/0x03-shell_variables_expansions)
