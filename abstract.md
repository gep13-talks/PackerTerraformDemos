How to create a system of Immutable Infrastructure

When applying updates or configuration to a server, it can be a lengthy and troublesome process, which may result in changes having to be reverted.
Switching to a system of Immutable Infrastructure means that new machines are provisioned and swapped out with existing machines, which can then be destroyed.
With this system, machine updates and configuration are done as part of the build process, rather than after the server has been provisioned.
This helps to reduce inconsistencies between servers, and as a result, improves the reliability of the deployment process.
In this talk, we will look at how we can use tools like Packer, Chocolatey and Terraform to help create a system for deploying Immutable Infrastructure.
