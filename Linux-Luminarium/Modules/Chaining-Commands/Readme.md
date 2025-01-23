# Chaining with Semicolons
### Commands:
```
1) hacker@chaining~chaining-with-semicolons:~$ /challenge/pwn ; /challenge/college
```
### Flag: 
>pwn.college{g4jWdR7-NyxT03czF.VUz2Byd_LlwqTFmDdYNyufU0oX}

# Your First Shell Script
### Commands:
```
1) hacker@chaining~your-first-shell-script:~$ echo /challenge/pwn > x.sh && echo /challenge/college >> x.sh
2) hacker@chaining~your-first-shell-script:~$ bash x.sh
```
### Flag: 
>pwn.college{YBdR7cL-UF2XlwNyDd04oFjmVzWNd_yTfVczljoTYqx}
### Explanation:
Used redirection to store the output of `echo` command in a file named `x` with an extension `.sh` This extension is used for shell scripts. When the file is run using `bash`, it does not read the contents like that of a file but rather executes them as commands.

# Redirecting Script Ouptut
### Commands:
```
1) hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
```
### Flag:
>pwn.college{NlF_zYV0cTFUmqld4dRTBy7joXoF3.DYN7czl2UoWx}
### Explanation:
The output of `bash x.sh` is piped to the command `/challenge/solve` which gave the flag.

# Executable Shell Scripts
### Commands:
```
1) hacker@chaining~executable-shell-scripts:~$ echo /challenge/solve > y.sh
2) hacker@chaining~executable-shell-scripts:~$ ls -l
```
A list of files and directories under the home directory was displayed among which was

`-rw-r--r-- 1 hacker hacker   17 Oct 18 11:27  y.sh`
```
3) hacker@chaining~executable-shell-scripts:~$ chmod u+x y.sh
4) hacker@chaining~executable-shell-scripts:~$ ./y.sh
```
### Flag:
>pwn.college{FYzLdX.VNmR4qF7joTfTYowc2c-BU0YNW3d_ljzFoYX}
### Explanation:
Instead of using `bash` I made the file `y.sh` executable by changing the file permissions using `chmod` followed by executing it (since its in the current directory i.e. home directory, I used `./`)