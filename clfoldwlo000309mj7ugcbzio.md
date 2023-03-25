---
title: "Understanding package manager and systemctl"
datePublished: Sat Mar 25 2023 23:18:09 GMT+0000 (Coordinated Universal Time)
cuid: clfoldwlo000309mj7ugcbzio
slug: understanding-package-manager-and-systemctl
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1679786165438/6e9cc21b-49c8-499a-85dd-2761df5a46c7.jpeg
tags: docker, devops, jenkins, trainwithshubham

---

#Day7 of #90DaysOfDevopsChallenge

A package manager is a tool that allows users to install, remove, upgrade, configure and manage software packages on an operating system. The package manager can be a graphical application like a software center or a command line tool like apt-get or pacman.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679785849339/60b53d8d-78ba-4f69-b1e9-ed848cf07a32.png align="center")

### ✅What is a package?

A package is usually referred to an application but it could be a GUI application, command line tool or a software library (required by other software programs). A package is essentially an archive file containing the binary executable, configuration file and sometimes information about the dependencies.

### ✅Different kinds of package managers

Package Managers differ based on packaging system but same packaging system may have more than one package manager.

For example, RPM has Yum and DNF package managers. For DEB, you have apt-get, aptitude command line based package managers.

### ✔️Docker Installation - Complete Step by step Guide

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679785676686/12137c68-9c3b-4f10-ae0d-65abbd12281f.png align="center")

1. Remove any Docker files that are running in the system, using the following command:
    
    Command : <mark>sudo apt-get remove docker docker-engine docker.io</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679768786702/671cf6da-f015-4ee9-9dc9-c0c8244cb665.png align="center")
    
2. Check if the system is up-to-date using the following command:
    

Command : <mark>sudo apt-get update</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679767773589/5820ced5-f557-4aa3-8180-4acd9449e6ae.png align="center")

1. Docker Installation command : <mark>sudo apt install </mark> [<mark>docker.io</mark>](http://docker.io)
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679769051998/4f8b275f-29b7-498b-b36a-9b1b4018d189.png align="center")

You’ll then get a prompt asking you to choose between y/n - choose y.

1. Install all the dependency packages
    

Command: <mark>sudo snap install docker</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679769723814/af400555-a4bf-44bd-a918-1904be4e1205.png align="center")

5\. Before testing Docker, check the version installed using the following command: <mark>docker --version</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679769960455/1b4e31eb-5365-4625-bb80-17ab3d9daf4c.png align="center")

6\. Pull an image from the Docker hub

command : <mark>sudo docker run hello-world</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679770270465/17a976a9-4e3f-42fc-b127-d6d50a474c68.png align="center")

Here, hello-world is the docker image present on the Docker hub.

1. Check if the docker image has been pulled and is present in your system using the following command: <mark>sudo docker images</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679770355465/e16dd05f-3eab-47ad-91ef-8028ce7d1545.png align="center")
    
2. To display all the containers pulled
    
    command: <mark>sudo docker ps -a</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679770582060/fa4328eb-c0a3-4605-9e66-5030aaaa5709.png align="center")
    
3. To check for containers in a running state, use the following command:
    
    command : $ <mark>sudo docker ps</mark>
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679770625345/8339dbcc-530f-4fb3-b7cb-1d945e3e205b.png align="center")

***You’ve just successfully installed Docker on Ubuntu!***

### ✔️Jenkins Installation - Complete step by step Guide

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679782256267/0c9b58f3-ada6-40db-a6fe-bbdbe562ec37.png align="center")

1. Java Installation:
    

Commands : <mark>sudo apt-cache search openjdk</mark>

<mark>sudo apt-get install openjdk-11-jre -y</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679772597898/a79e6c0d-5f97-4558-a6b0-08a4d277e993.png align="center")

1. Check your java version by using the below command :
    

<mark>Java --version</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679772829140/236179bd-5429-4402-af45-f92425036874.png align="center")

1. add the repository key to the system:
    
    command : <mark>wget -q -O - </mark> [<mark>https://pkg.jenkins.io/debian-stable/jenkins.io.key</mark>](https://pkg.jenkins.io/debian-stable/jenkins.io.key) <mark>| sudo apt-key add -</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679771990047/5af35fc9-9850-41f7-9372-b073127ee9d5.png align="center")
    
2. After the key is added the system will return with `OK`.
    
    Next, let’s append the Debian package repository address to the server’s `sources.list`:
    
    command : <mark>sudo sh -c 'echo deb </mark> [<mark>http://pkg.jenkins.io/debian-stable</mark>](http://pkg.jenkins.io/debian-stable) <mark>binary/ &gt; /etc/apt/sources.list.d/jenkins.list'</mark>
    
3. ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679772016701/5a46debd-d166-4b76-87e4-76a5363545b2.png align="center")
    
    After both commands have been entered, we’ll run `update` so that `apt` will use the new repository.
    
    command : <mark>sudo apt update</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679771432349/8de67d6b-09f4-44eb-be98-e283f50b1b1e.png align="center")
    
4. Finally, we’ll install Jenkins and its dependencies.
    
    commands : <mark>sudo apt install jenkins</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679772155901/e5ac06f6-c121-4323-a34b-0a6276ac6480.png align="center")
    
5. Let’s start Jenkins by using [`systemctl`](https://www.digitalocean.com/community/tutorials/how-to-use-systemctl-to-manage-systemd-services-and-units):
    
    command : <mark>sudo systemctl start jenkins</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679773314506/e38aff72-e87a-456b-9d20-9cadd1832c79.png align="center")
    
6. Since `systemctl` doesn’t display status output, we’ll use the `status` command to verify that Jenkins started successfully:
    

Command : <mark>sudo systemctl status jenkins</mark>

If everything went well, the beginning of the status output shows that the service is active and configured to start at boot:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679773574336/07699d9b-cf0d-48bf-8376-e015e3a9b289.png align="center")

1. Opening the Firewall
    
    command : <mark>sudo ufw allow 8080</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679774035813/966e6d64-c8d5-47c1-8cf2-390737c451d9.png align="left")
    
2. To check the status use the below command : <mark>sudo ufw status</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679774116390/76c453b3-5e37-43c7-a949-2f8f42710e70.png align="left")
    
3. If the status is inactive, as shown in the below screenshot, use the commands : <mark>sudo ufw allow OpenSSH</mark>
    
    <mark>sudo ufw enable</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679784275702/5dec9281-95d8-4443-af28-14808cd5784b.png align="center")
    
4. sudo ufw allow OpenSSH sudo ufw enableCheck `ufw`’s status to confirm the new rules:
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679774415472/106cf41f-bf28-4cd5-85bb-977babe376ae.png align="center")

## ✔️Setting Up Jenkins

To set up your installation, visit Jenkins on its default port, `8080`, using your server domain name or IP address: [`http://your_server_ip_or_domain:8080`](http://your_server_ip_or_domain:8080)

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679777453098/7808d536-71e4-4471-84bb-3b0619794466.png align="center")

In the terminal window, use the `cat` command to display the password:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679777643481/35989afc-5bdb-4118-9018-aeadaf4fc82a.png align="center")

We’ll click the **Install suggested plugins** option, which will immediately begin the installation process.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679777764617/fefdb2ae-498d-4589-9702-f150f150e9fb.png align="center")

When the installation is complete, you’ll be prompted to set up the first administrative user. It’s possible to skip this step and continue as `admin` using the initial password we used above, but we’ll take a moment to create the user.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679777938600/b6ea3927-f3e5-49ee-a703-8e0f9d09af59.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679777958855/8454659a-4eda-4f7d-84a0-de1164ce26ea.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679778010457/c394dd13-49db-4a22-838f-e4902d967969.png align="center")

### ✔️check the status of docker service in your system (make sure you completed above tasks, else docker won't be installed)

Command : <mark>systemctl status docker</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679778504253/70693e65-c32b-42ad-ae9c-f7be77619016.png align="center")

To stop the Docker service, you can use the following command in the terminal:

command : <mark>sudo systemctl stop docker</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679778742024/1ca5321a-5304-4334-8b12-6756622d27d0.png align="center")

This will stop the Docker service immediately. If you want to prevent the service from starting automatically at boot, you can also disable it using the following command: <mark>sudo systemctl disable docker</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679784798958/c6c7339e-be71-437d-84ea-3dbc062dd42b.png align="center")

### ✔️Stop the service jenkins and post before and after screenshots

To check the status

command : <mark>sudo systemctl status jenkins</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679779110767/ef1e9167-fb70-42aa-9564-2a768216db9a.png align="center")

To stop the Jenkins service, you can use the following command in the terminal: <mark>sudo systemctl stop jenkins</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679780458473/3f86bcbe-321f-4b5f-93b1-617ed7697214.png align="center")

### ✔️Read about the commands systemctl vs service

**💡systemctl :**

The systemctl command **manages both system and service configurations, enabling administrators to manage the OS and control the status of services**. Further, systemctl is useful for troubleshooting and basic performance tuning.

Example: <mark>systemctl status docker</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679779647320/bbf35890-5cec-4e28-860b-565507198bcc.png align="center")

**💡Service :**

The service command **starts, stop and restart a daemon or services by calling the script**. Usually all scripts are stored in /etc/init. d directory. It runs a script in as predictable environment as possible.

Example : <mark>service docker status</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1679780514536/b3561bd3-fef0-4c23-936f-e603b0646c20.png align="center")

**Conclusion : systemctl is basically a more powerful version of service**.

With service you can only do commands related to the service (i.e. status, reload, restart) whereas with systemctl you can use more advanced commands.