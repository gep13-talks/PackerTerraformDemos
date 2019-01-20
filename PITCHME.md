---?image=assets/img/lego-blocks.jpg
@title[What is GitPitch?]

@snap[south-west h4-white]
#### How to create a system of Immutable Infrastructure
@snapend

@snap[north-east text-04 text-gray text-smallcaps]
Press F to view slideshow in fullscreen mode.
@snapend

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Vagrant?]

@snap[west h4-white]
#### Question.
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Vagrant)@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Vagrant]

@snap[west h4-white]
#### Answer.
@snapend

@snap[east span-70]
bob

---?code=Vagrantfile

@[3-4](Base VM Setup)
@[22-27](VM Configuration)
@[32-36](Provisioning Scripts)

---?terminal=assets/sessions/vagrant-up.cast&color=#7FDBFF&font=small&title=vagrant up

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Packer?]

@snap[west h4-white]
#### Question.
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Packer)@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Packer]

@snap[west h4-white]
#### Answer.
@snapend

@snap[east span-70]
bob

---?terminal=assets/sessions/packer-validate.cast&color=#7FDBFF&font=small&title=packer validate

---?code=Demos/1/first_run.json&lang=json

@[2-6](Packer variables)
@[7-13](Packer Builder)
@[30-40](Inline PowerShell Provisioner)
@[44-53](PowerShell Script Provisioner)


---?terminal=assets/sessions/packer-build-aws.cast&color=#7FDBFF&font=small&title=packer build - Windows on AWS

---?code=Demos/2/first_run.json&lang=json

@[2-8](Packer variables)
@[10-27](Amazon EBS Builder)
@[28-35](DigitalOcean Builder)
@[37-46](Shell Provisioner)

---?terminal=assets/sessions/packer-build-parallel.cast&color=#7FDBFF&font=small&title=packer build - Linux on AWS and DigitalOcean

---?code=Demos/3/windows_10.json&lang=json

@[8-26](Virtualbox ISO Builder)
@[47-54](Post-Processor)
@[103-114](Packer Variables)

---?terminal=assets/sessions/packer-build-virtualbox.cast&color=#7FDBFF&font=small&title=packer build - virtualbox to vagrant

---?image=assets/img/bg/black.jpg&position=left&size=35% 100%
@title[What is Terraform?]

@snap[west h4-white]
#### Question.
@snapend

@snap[east span-80]
#### What is
## @css[text-gold text-bold](Terraform)@fa[question]
@snapend

---?image=assets/img/bg/blue.jpg&position=left&size=35% 100%
@title[Terraform]

@snap[west h4-white]
#### Answer.
@snapend

@snap[east span-70]
bob

---?code=Demos/4/variables.tf

---?code=Demos/4/example.tf

@[1-5](Provider definition)
@[7-14](Main resource definition)
@[16-18](IP Address resource)
@[20-22](Output variable)

---?terminal=assets/sessions/terraform-apply.cast&color=#7FDBFF&font=small&title=terraform apply

---?terminal=assets/sessions/terraform-destroy.cast&color=#7FDBFF&font=small&title=terraform destroy

---

@title[Who Am I? - Gary Ewan Park]
@transition[none]

@snap[north-west]
@css[choco-blue](WHO AM I?)
@snapend

@snap[west span-65]
Senior Software Engineer @ Chocolatey Software
<br>
<br>
![MVP Logo](assets/img/mvp.jpg)
![Cake Build](assets/img/cake.png)
@snapend

@snap[east span-30]
![Gary Ewan Park](assets/img/gary-avatar.png)
<br>
@css[bio-name](Gary Ewan Park)
@snapend

@snap[south-west bio-contact]
@fa[twitter twitter-blue]&nbsp;&nbsp;gep13&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@fa[github text-black]&nbsp;&nbsp;github.com/gep13&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@fa[home text-blue]&nbsp;&nbsp;gep13.co.uk&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
@fa[envelope choco-blue]&nbsp;&nbsp;gary@chocolatey.io
@snapend

---

@title[Questions]
## Questions?

Feel free to get in touch after the talk.

Email: gep13gep13.co.uk

Twitter: @gep13

Web: https://gep13.co.uk

---

@title[Resources]
## Resources

* Chocolatey Documentation - https://chocolatey.org/docs
* Gitter Chat - https://gitter.im/chocolatey/choco
* Google Groups - https://groups.google.com/forum/#!forum/chocolatey
* Learning Resources - https://chocolatey.org/docs/resources
* How To Use Package Internalizer To Create Internal Package Source - https://chocolatey.org/docs/how-to-setup-internal-package-repository
