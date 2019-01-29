---?image=assets/img/lego-blocks.jpg
@title[Immutable Infrastructure]

@snap[south-west h4-white]
@box[bg-orange text-white rounded demo-box-pad](How to create a system of Immutable Infrastructure)
@snapend

---?color=#7FDBFF
@title[Slides and Code]

## Slides

### https://gep13.me/ptslides

## Code

### https://gep13.me/ptcode

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Immutable Infrastructure?]

@snap[west h4-white]
#### Question
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Immutable Infrastructure )@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Immutable Infrastructure]

@snap[west h4-white]
#### Answer
@snapend

@snap[east span-70]
@quote[An immutable infrastructure is another infrastructure paradigm in which servers are never modified after they're deployed. If something needs to be updated, fixed, or modified in any way, new servers built from a common image with the appropriate changes are provisioned to replace the old ones. After they're validated, they're put into use and the old ones are decommissioned.](Digital Ocean Tutorial)

---

@quote[In the old way of doing things, we treat our servers like pets, for example Bob the mail server. If Bob goes down, it’s all hands on deck. The CEO can’t get his email and it’s the end of the world. In the new way, servers are numbered, like cattle in a herd. For example, www001 to www100. When one server goes down, it’s taken out back, shot, and replaced on the line.](Randy Bias)

@size[0.5em](http://cloudscaling.com/blog/cloud-computing/the-history-of-pets-vs-cattle/)

---

@quote[Snowflake servers are similar to pets. They are servers that are managed by hand, frequently updated and tweaked in place, leading to a unique environment.](Digital Ocean Tutorial)

@snap[south]
@size[0.5em](https://martinfowler.com/bliki/SnowflakeServer.html)
@snapend

---
@quote[Phoenix servers are similar to cattle. They are servers that are always built from scratch and are easy to recreate, or "rise from the ashes", through automated procedures.](Digital Ocean Tutorial)

@snap[south]
@size[0.5em](https://martinfowler.com/bliki/PhoenixServer.html)
@snapend

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What are the benefits Immutable Infrastructure?]

@snap[west h4-white]
#### Question
@snapend

@snap[east span-80]
#### What are the benefits of
## @css[text-gold text-bold](Immutable Infrastructure )@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Immutable Infrastructure]

@snap[west h4-white]
#### Answer
@snapend

@snap[east span-70]
@ul
- Fewer deployment failures
- No configuration drift
- Consistent staging environments
- Simple rollback and recovery processes
@ulend
@snapend

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Vagrant?]

@snap[west h4-white]
#### Question
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Vagrant)@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Vagrant]

@snap[west h4-white]
#### Answer
@snapend

@snap[east span-70]
![Vagrant Logo](assets/img/vagrant.png)

@quote[Vagrant is a tool for building and managing virtual machine environments in a single workflow.](Vagrant website)
@snapend

---?code=Vagrantfile&title=Example Vagrantfile
@title[Vagrantfile]

@[3-4](Base VM Setup)
@[22-27](VM Configuration)
@[32-36](Provisioning Scripts)

---?color=beige
@title[Demo - Packer]

## Demo

### Create Vagrant VM

+++?terminal=assets/sessions/vagrant-up.cast&color=#7FDBFF&font=small&title=vagrant up

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Packer?]

@snap[west h4-white]
#### Question
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Packer)@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Packer]

@snap[west h4-white]
#### Answer
@snapend

@snap[east span-70]
![Packer Logo](assets/img/packer.png)

@quote[Packer is an open source tool for creating identical machine images for multiple platforms from a single source configuration](Packer website)
@snapend

---?code=Demos/1/first_run.json&lang=json&title=Example Packer file
@title[Example Packer file]

@[2-6](Packer variables)
@[7-13](Packer Builder)
@[30-40](Inline PowerShell Provisioner)
@[44-53](PowerShell Script Provisioner)

+++?terminal=assets/sessions/packer-validate.cast&color=#7FDBFF&font=small&title=packer validate

---?color=beige
@title[Demo - Packer]

## Demo

### Run packer to generate Amazon AMI

+++?terminal=assets/sessions/packer-build-aws.cast&color=#7FDBFF&font=small&title=packer build - Windows on AWS

---?code=Demos/2/first_run.json&lang=json&title=Parallel packer build
@title[Parallel packer build]

@[2-8](Packer variables)
@[10-27](Amazon EBS Builder)
@[28-35](DigitalOcean Builder)
@[37-46](Shell Provisioner)

---?color=beige
@title[Demo - Packer in Parallel]

## Demo

### Run packer in parallel

+++?terminal=assets/sessions/packer-build-parallel.cast&color=#7FDBFF&font=small&title=packer build - Linux on AWS and DigitalOcean

---?code=Demos/3/windows_10.json&lang=json&title=Virtualbox packer build
@title[Virtualbox packer build]

@[8-18](Floppy files)
@[19-26](Virtualbox provider)
@[47-54](Post-Processor)
@[103-114](Packer Variables)

---?color=beige
@title[Demo - Packer Virtualbox]

## Demo

### Generate Virtualbox box

+++?terminal=assets/sessions/packer-build-virtualbox.cast&color=#7FDBFF&font=small&title=packer build - virtualbox to vagrant

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Terraform?]

@snap[west h4-white]
#### Question
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Terraform)@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Terraform]

@snap[west h4-white]
#### Answer
@snapend

@snap[east span-70]

![Terraform Logo](assets/img/terraform.png)

@quote[Terraform is a tool for building, changing, and versioning infrastructure safely and efficiently.](Terraform website)
@snapend

---?code=Demos/4/variables.tf&title=Terraform Variables
@title[Terraform Variables]

---?code=Demos/4/example.tf&title=Example Terraform File
@title[Example Terraform file]

@[1-5](Provider definition)
@[7-14](Main resource definition)
@[16-18](IP Address resource)
@[20-22](Output variable)

---?color=beige
@title[Demo - Terraform Apply]

## Demo

### Running Terraform Apply

+++?terminal=assets/sessions/terraform-apply.cast&color=#7FDBFF&font=small&title=terraform apply

---?color=beige
@title[Demo - Terraform Destroy]

## Demo

### Running Terraform Destroy

+++?terminal=assets/sessions/terraform-destroy.cast&color=#7FDBFF&font=small&title=terraform destroy

---?color=beige
@title[Demo - Vagrant add]

## Demo

### Adding newly created box to vagrant

+++?terminal=assets/sessions/vagrant-box-add.cast&color=#7FDBFF&font=small&title=vagrant box add

+++?terminal=assets/sessions/vagrant-up-local.cast&color=#7FDBFF&font=small&title=vagrant up local

+++?terminal=assets/sessions/vagrant-destroy.cast&color=#7FDBFF&font=small&title=vagrant destroy

---?color=beige
@title[Demo - Bringing it all together]

## Demo

### Bringing it all together

---?color=#7FDBFF
@title[Who Am I? - Gary Ewan Park]

@snap[north-west]
Who am I?
@snapend

@snap[west span-65]
Senior Software Engineer @ Chocolatey Software
<br>
<br>
![Chocolatey](assets/img/chocolatey.png)
![MVP Logo](assets/img/mvp.jpg)
![Cake Build](assets/img/cake.png)
@snapend

@snap[east span-30]
![Gary Ewan Park](assets/img/gary-avatar.png)
<br>

Gary Ewan Park

@snapend

@snap[south-west bio-contact]
@fa[twitter twitter-blue]&nbsp;&nbsp;gep13&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@fa[github text-black]&nbsp;&nbsp;github.com/gep13&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@fa[home text-blue]&nbsp;&nbsp;gep13.co.uk&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@fa[envelope choco-blue]&nbsp;&nbsp;gep13@gep13.co.uk
@snapend

---?color=#7FDBFF

@title[Questions]
## Questions?

Feel free to get in touch after the talk.

Email: gep13@gep13.co.uk

Twitter: @gep13

Web: https://gep13.co.uk

---?color=#7FDBFF
@title[Resources]

## Resources

* [Introduction to Packer](https://www.packer.io/intro/index.html)
* [Introduction to Terraform](https://www.terraform.io/intro/index.html)
* [Introduction to Vagrant](https://www.vagrantup.com/intro/index.html)
* [Chocolatey Documentation](https://chocolatey.org/docs)
* [What is Immutable Infrastructure - Digital Ocean](https://www.digitalocean.com/community/tutorials/what-is-immutable-infrastructure)
