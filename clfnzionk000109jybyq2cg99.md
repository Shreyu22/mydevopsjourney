---
title: "File Permissions and Access Control Lists"
datePublished: Sat Mar 25 2023 13:06:01 GMT+0000 (Coordinated Universal Time)
cuid: clfnzionk000109jybyq2cg99
slug: file-permissions-and-access-control-lists
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679749526352/cf71770f-7e85-448d-b232-92c365b37134.png

---

#day6 of #90DaysofDevopsChallenge

The concept of Linux File permission and ownership is important in Linux. Today, we will be working on Linux permissions and ownership and will perform tasks on both of them.

Let us start with the Permissions.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679747638010/dffe1894-633f-405b-a8c1-a7a8ffce993b.png align="left")

### ✔️Create a simple file and do `ls -ltr` to see the details of the files

Command : <mark>ls -ltr</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679746961976/316430bd-c797-49e8-bbd9-f28e197fe4e5.png align="center")

### ✔️Each of the three permissions are assigned to three defined categories of users.

### The categories are:

* **owner** - The owner of the file or application
    
* **<mark>"chown"</mark>** - used to change the ownership permission of a file or directory.
    
* **group** \- The group that owns the file or application.
    
* **<mark>"chgrp"</mark>** is used to change the group permission of a file or directory.
    
* others - All users with access to the system. (outside users are in a group)
    
* **<mark>"chmod"</mark>** is used to change the other users permissions of a file or directory.
    
* ### As a task, change the user permissions of the file and note the changes after `ls -ltr`
    
* ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679748229525/6fd7c512-1f08-4852-a38e-0b24ec36d01d.png align="center")
    

### ✔️What are File Permissions ?

* Linux is a multi-user operating system, so it has security to prevent people from accessing each other's confidential files.
    
* When you execute an “ls” command, you are not given any information about the security of the files, because by default “ls” only lists the names of files. You can get more information by using an “option” with the “ls” command. All options start with a ‘-‘. For example, to execute “ls” with the “long listing” option, you would type ls -l
    
    1. The first character will almost always be either a ‘-‘, which means it’s a file, or a ‘d’, which means it’s a directory.
        
    2. The next nine characters (rw-r–rwx) show the security and permissions from which -
        
        r = reading permissions
        
        w = writing permissions
        
        x = executable permissions
        
        ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679747830466/38803794-e9fb-4338-a72a-d7cb77e1439f.png align="center")
        

### Permissions with numeric and Symbols

For all access to owner, group and others use the command <mark>chmod 777 </mark> filename.txt

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679747918474/71a08fe1-a92a-461a-a4ef-90336bf401dd.png align="left")

### ✔️What is ACL?

Access control list provides an additional, more flexible permission mechanism for file systems. It is designed to assist with UNIX file permissions. ACL allows us to give permissions for any user or group to any disc resource.

**getfacl command**

The getfacl command is used to retrieve the ACLs of files and directories.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679685942652/1ba0ece9-870f-433a-bbbf-957547c30bb4.png?auto=compress,format&format=webp align="left")

**setfacl command**

The setfacl command in Linux is used to **set file access control lists**. A file’s ACL specifies the users and groups that are allowed to access the file, and the permissions that they have.

The setfacl command can be used to add, remove, or modify a file’s ACL.

#trainwithshubham #devops