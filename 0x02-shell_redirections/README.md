# 0x02-shell_redirections

This is a readme file for the 0x02-shell_redirections directory in the alx-system_engineering-devops repo.

The 0-hello_world file is a script that prints “Hello, World”, followed by a new line to the standard output.

The 1-confused_smiley file is a script that displays a confused smiley "(Ôo)'.

The 2-hellofile file is a script that displays the content of the /etc/passwd file.

The 3-twofiles file is a script that displays  the content of /etc/passwd and /etc/hosts

The 4-lastlines file is a script that displays the last 10 lines of /etc/passwd.

The 5-firstlines file is a script that displays the first 10 lines of /etc/passwd.

The 6-third_line file is a script that displays the third line of the file iacta. The file iacta will be in the working directory

The 7-filefile is a script that creates a file named exactly \*\\'"Holberton School"\'\\*$\?\*\*\*\*\*:) containing the text Holberton School ending by a new line.

The 8-cwd_state file is a script that writes into the file ls_cwd_content the result of the command ls -la. If the file ls_cwd_content already exists, it should be overwritten. If the file ls_cwd_content does not exist, create it.

The 9-duplicate_last_line file is a script that duplicates the last line of the file iacta.

The 10-no_more_js file is a script that deletes all the regular files (not the directories) with a .js extension that are present in the current directory and all its subfolders.

The 11-directories file is a script that counts the number of directories and sub-directories in the current directory. The current and parent directories should not be taken into account. Hidden directories should be counted.

The 12-newest_files file is a script that displays the 10 newest files in the current directory.
Requirements:
One file per line
Sorted from the newest to the oldest

The 13-unique file is script that takes a list of words as input and prints only words that appear exactly once.
Input format: One line, one word
Output format: One line, one word
Words should be sorted

The 14-findthatword file is script that displays lines containing the pattern “root” from the file /etc/passwd.

The 15-countthatword file is a script that displays the number of lines that contain the pattern “bin” in the file /etc/passwd.

The 16-whatsnext file is a script that displays lines containing the pattern “root” and 3 lines after them in the file /etc/passwd.

The 17-hidethisword file is a script that displays  all the lines in the file /etc/passwd that do not contain the pattern “bin”.

The 18-letteronly file is a script that displays all lines of the file /etc/ssh/sshd_config starting with a letter including capital letters as well.

The 19-AZ file is a script that displays all characters A and c from input to Z and e respectively.

The 20-hiago file is a script that removes all letters c and C from input.

The 21-reverse file is a script that reverses its input.

The 22-users_and_homes file is a script that displays all users and their home directories, sorted by users, based on the the /etc/passwd file.

The 100-empty_casks file is a script that finds all empty files and directories in the current directory and all sub-directories.
Only the names of the files and directories should be displayed (not the entire path
Hidden files should be listed
One file name per line
The listing should end with a new line

The 101-gifs file is a script that lists all the files with a .gif extension in the current directory and all its sub-directories.
Hidden files should be listed
Only regular files (not directories) should be listed
The names of the files should be displayed without their extensions
The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay)
One file name per line
The listing should end with a new line

The 103-the_biggest_fan file is a script that parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
Order by number of requests, most active host or IP at the top.
