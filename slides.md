---
lineNumbers: true
transition: fade-out
---

# From Chaos to Consistency

Building Reliable Environments with Packer and Terraform

---
transition: slide-left
layout: image
image: ./images/chaos.jpg
---

# In the beginning... There was chaos

---
transition: slide-up
---

##  The Era of Inconsistency: Pre-Configuration Management 

- Little to no documentation

- No version control

- Hard to reproduce

- Automation ? Good luck with that

- How to scale ? Add more people to the team ?


---
transition: slide-left
layout: cover
class: text-center
---

# Where we do go from here ?


---
transition: slide-left
class: text-center
layout: image
image: ./images/solution.jpg
---

# 


---
transition: slide-left
layout: two-cols
---

# Elevator Pitch: Terraform

- Infrastructure as code tool that allows you to define and provision infrastructure in a declarative way

- Provides a common language for teams to communicate about infrastructure

- Allows you to manage infrastructure in a consistent way

- Allows you to version control your infrastructure

::right::
  
  ```hcl
  resource "aws_instance" "example" {
    ami           = "ami-0c55b159cbfafe1f0"
    instance_type = "t2.micro"
  }
  ``` 





---
transition: slide-up
layout: two-cols 
---

## Elevator Pitch: Packer

- Tool that allows you to create machine images for multiple platforms from a single source configuration

- Allows you to build machine images consistently across multiple platforms

::right::

```json 
{
  "builders": [{
    "type": "amazon-ebs",
    "region": "us-west-2",
    "instance_type": "t2.micro",
    "source_ami": "ami-0c55b159cbfafe1f0",
    "ssh_username": "ubuntu",
    "ami_name": "my-ubuntu-20.04-{{timestamp}}"
  }],
  "provisioners": [{
    "type": "shell",
    "script": "path/to/provisioning-script.sh"
  }]
}

```

---
transition: slide-right 
layout: cover
class: text-center 
---

##  Terraform + Packer  = ✨ ? 



---
transition: slide-right
layout: image
image: ./images/well-yes.jpg  
---

##


---
transition: slide-down
---
## Going Beyond Adoption: Leveraging Packer and Terraform for Reliable Environments

- **Consistency** is the key to success

- Reduce the number of manual interventions

- build intuitive CI/CD pipelines

- **Automate** everything you can

- **Document** everything you can't automate

---
transition: slide-down
class: text-center
layout: cover
---

## Demo time !! 

---
class: text-center
layout: cover
---

## Thank you ! 


---
transition: slide-left
---

## Links 

- @ 0xgreat 
- @ s1ntaxe770r

code available at at https://github.com/umegbewe/







