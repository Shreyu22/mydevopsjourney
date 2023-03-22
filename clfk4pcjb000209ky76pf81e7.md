---
title: "Shell Scripting"
datePublished: Wed Mar 22 2023 20:20:05 GMT+0000 (Coordinated Universal Time)
cuid: clfk4pcjb000209ky76pf81e7
slug: shell-scripting
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679516301702/4664b506-8c42-4ae5-88dd-f54bb1312f78.jpeg
tags: devops, devops-journey, trainwithshubham, cringe

---

<mark>#Day4 </mark> of <mark>#90DaysOfDevopsChallenge</mark>

### ✅What is Kernel?

The Linux kernel is the main component of a Linux operating system (OS) and is the core interface between a computer’s hardware and its processes. It communicates between the 2, managing resources as efficiently as possible.

### ✅What is Shell?

A shell is special user program which provide an interface to user to use operating system services. Shell accepts human readable commands from user and convert them into something which Kernel can understand. It is a command language interpreter that execute commands read from input devices such as keyboards or from files. The shell gets started when the user logs in or start the terminal.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679514750686/209e8a58-3c57-4c33-bcfa-7bfb2f5b419f.png align="center")

### ✅What is Linux Shell Scripting?

A shell script is a computer program designed to be run by a Linux shell, a command-line interpreter. The various dialects of shell scripts are considered to be scripting languages. Typical operations performed by shell scripts include file manipulation, program execution, and printing text.

### ✅What is `#!/bin/bash?` can we write `#!/bin/sh` as well?

**sh =&gt; Bourne Shell** sh used to be a shell called bourne shell back in 1977. sh is typically a minimalistic shell that lacks some of the advanced features of Bash.

**bash =&gt; Bourne Again Shell** Bash is an extended version of the Bourne shell (sh) and provides additional features such as command line editing, improved job control, and enhanced scripting capabilities.

bash and sh are two different shells with different features.

Both **#!/bin/bash** and **#!/bin/sh** are called shebangs and are used to specify the interpreter for a script in Unix-like operating systems.

**#!/bin/bash** specifies that the script should be interpreted by the Bash shell, which is a popular shell used in many Linux distributions.

**#!/bin/sh** specifies that the script should be interpreted by the default system shell, which may or may not be Bash. In many Unix-like systems, sh is a symbolic link to a specific shell, such as Bash or the original Bourne shell.

In summary, if you want to use Bash-specific features in your script, you should use #!/bin/bash. However, if your script only uses standard POSIX shell features, you can use #!/bin/sh for improved portability.

### ✅Write a Shell Script which prints `I will complete #90DaysOofDevOps challenge`

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679515303194/12f41de0-33bb-4bb1-a21e-eb62ce62fb65.png align="left")

Key Syntax for the execution access : <mark>chmod a+x filename.sh</mark>

### ✅Write a Shell Script to take user input, input from arguments and print the variables.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679515445145/a3ef850c-1d05-40f7-96a7-27072d583297.png align="left")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679515460970/f5ff14bf-069f-4eef-9b45-278bd0cd2c64.png align="left")

### ✅Write an Example of If else in Shell Scripting by comparing 2 numbers

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679515755520/7ce663b5-b559-4bff-95b7-685f2799e903.png align="left")

fi😃

#devops #trainwithshubham #90daysOfDevopschallenge