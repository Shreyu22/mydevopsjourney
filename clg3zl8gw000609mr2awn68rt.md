---
title: "Docker for DevOps Engineers"
datePublished: Wed Apr 05 2023 17:52:19 GMT+0000 (Coordinated Universal Time)
cuid: clg3zl8gw000609mr2awn68rt
slug: docker-for-devops-engineers
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1680717088906/e4e872b7-4212-4672-9e2e-787897d2c0a3.png
tags: devops, trainwithshubham, 90daysofdevopschallenge

---

#Day16 of #90DaysOfDevopsChallenge

**Docker** is an open-source platform for developing, packaging and deploying applications in a containerized environment. Containers are lightweight and portable virtual environments that can run on any system that supports Docker.

### ✅Use the `docker run` command to start a new container and interact with it through the command line. \[Hint: docker run hello-world\]

**Local system update:**

```python
sudo apt-get update
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680703061893/27459b8d-9aee-4240-9cbb-733508eefacb.png align="center")

**command to check the docker version**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680703112677/327a682f-0b1d-4a50-bddb-00551dffdf7f.png align="center")

**use the following command to start Docker**

```python
sudo usermod -aG docker $user 
systemctl restart docker 
```

**Note: If the permission denied error occurs, use the below command and enter the password.**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680713462290/2fb4ecb9-cd28-4fff-b732-03a39fd0a61a.png align="left")

**To check the docker status**

```python
systemctl status docker
```

**Use the pull command to download the image**

```python
docker pull python
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680713612658/11315e70-4126-45e6-a6db-7d1aaeed941b.png align="left")

**To check all the docker images :**

* ```python
    docker images
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680713736661/34ad243d-3239-4b50-b287-6471e3cec93a.png align="center")
    
    **Create a container from the above image:**
    
    * ```python
        docker run -it <image name> /bin/bash
        ```
        
    
    To start a new container and interact with it through the command line, you can use the following command:
    

```python
    docker run -td --name <cantainer name> -p 80:80 <image name>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680715455026/f363c85e-84dc-45dd-b56e-f0b0936055fe.png align="center")

**To see all the containers:**

```python
docker ps -a
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680714272898/7a6f8330-eb01-44dd-9ab2-623496b2f305.png align="center")

### ✅Use the `docker inspect` command to view detailed information about a container or image.

```python
docker inspect <container name>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680714674634/0dcb9f9f-48c0-48b0-8e5c-e0f2ffbd8efc.png align="left")

### ✅Use the `docker port` command to list the port mappings for a container

```python
docker port <container name >
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680715535104/1db1895a-ea31-4628-9795-e96488942ea2.png align="center")

### ✅Use the `docker stats` command to view resource usage statistics for one or more containers.

```python
docker stats <container name>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680715793515/19c355b1-ed24-4faa-b8df-fd25f45a7dd2.png align="center")

### ✅Use the `docker top` command to view the processes running inside a container

```python
docker top <container name or id>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680715916892/a7f4f131-d04d-49a3-a8d4-e9ce55f1bc42.png align="center")

### ✅Use the `docker save` command to save an image to a tar archive

```python
docker save -o <image>.tar <image name>
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680716464105/9065d9c1-7d0d-497d-b11c-1b934e4a11f7.png align="center")

### ✅Use the `docker load` command to load an image from a tar archive

```python
docker load  -i  <image.tar> 
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680716584300/38e55582-d4a5-4ee5-9ec1-4c2fdd77ac70.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680716623907/88452190-4b37-4544-aecb-31eb65d749df.png align="center")

Thank you!!