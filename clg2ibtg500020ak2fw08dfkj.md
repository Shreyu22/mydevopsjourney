---
title: "Python Libraries for DevOps -
#day15 of #90DaysOfDevopsChallenge"
datePublished: Tue Apr 04 2023 17:01:20 GMT+0000 (Coordinated Universal Time)
cuid: clg2ibtg500020ak2fw08dfkj
slug: python-libraries-for-devops-day15-of-90daysofdevopschallenge
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1680627605455/9e371f21-1c55-457f-9ecc-8dd7b01d11df.jpeg
tags: devops, 90daysofdevopschallenge

---

1. ### Create a Dictionary in Python and write it to a json File.
    
    ![Python](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4ii4_6NE2r_GhG6m_ZWtwwadDgOy46vp2lw&usqp=CAU align="center")
    
    **Step 1: create a file in the directory**
    
    Command : <mark>touch file_name.py</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680612287702/41bfa182-097d-473c-81e5-99fc5c9933bc.png align="left")
    
    Here I have written a file into it and will import it into JSON File :
    
    command : <mark>vim file_name.py </mark> to write into the file
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680614148813/a4f913b7-dccb-474a-9658-f1f32073087e.png align="center")
    
    **Step-2 Create a json file by running this python file and verify with the command "ls"**
    
    command : <mark>python3 file_name.py</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680614620143/c766462f-d9a4-49eb-9286-a81d4be0d219.png align="center")
    
    **Step-3 Verify it :**
    
    command : <mark>vi file_name.json</mark>
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680614768151/d48a62fa-e762-4946-90fe-4b24bc7eb565.png align="left")
    
2. ### Read a json file `services.json` kept in this folder and print the service names of every cloud service provider.
    

```plaintext
output

aws : ec2
azure : VM
gcp : compute engine

```

**Step-1 Create a file services.json and write the following code into it :**

```json
[
  {
    "name": "aws",
    "services": "ec2"
  },
  {
    "name": "azure",
    "services": "VM"
  },
  {
    "name": "gcp",
    "services": "compute engine"
  }
]
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680615338106/02107b2d-16fd-41ad-8e76-bf59054a17c4.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680615233952/6e057fbc-3125-4ca5-8ca7-153b2eaf982c.png align="center")

**Step-2 Create a new file named task2**[**.py**](http://services.py/) **and write the following code into it**

```json
import json

# Read the JSON data from the file
with open('services.json') as f:
    data = json.load(f)

# Print the service names for each cloud service provider
for provider in data:
    print(provider['name'], ':', provider['services'])
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680615890224/2fb252f9-94f1-4a6d-8f63-a202f2d66f29.png align="center")

**Step-3 Now run it with python, it will revert the content:**

command : <mark>python3 filename.py</mark>

Output :

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680616332630/ef23b7df-7be6-44b6-8603-c56f38508b4e.png align="left")

1. ### Read YAML file using python, file `service.yaml` and read the contents to convert yaml to json
    

**Step-1 Create a file service.yaml and add the following data into it :**

---

```yaml
---
services:
  debug: 'on'
  aws:
    name: EC2
    type: pay per hour
    instances: 500
    count: 500
  azure:
    name: VM
    type: pay per hour
    instances: 500
    count: 500
  gcp:
    name: Compute Engine
    type: pay per hour
    instances: 500
    count: 500
```

**Step-2 Create a file task3.py and add the following code into it :**

```python
import yaml 
import json 
with open('provider.json', 'r') as f:
    data = yaml.load(f, Loader=yaml.SafeLoader) 
with open('provider.json;, 'w') as f:
    json.dump(data, f, sort_keys=False)
  
  
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680627036308/8fd2876d-d3b4-4338-9303-cd642af3db1f.png align="center")

**Step-3 Run the python file using the below command and verify it using ls**

command : <mark>python3 file_name.py</mark>

<mark>ls file_name.json</mark>

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680627217554/d472b2f1-0e50-42bf-8a93-94bf3a4f045c.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1680627249931/75e035a4-6298-4219-a924-101476f648df.png align="center")

Thank you for your time!