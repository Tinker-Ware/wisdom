---
resource: true
categories: [Configs]
title: Recomended mix of Conigurations
---


Suggestions
===

This repository include information about the best way to keep errors away.


# About Roles

## Ghost

Create your server with more than 512 mb RAM memory.
`npm install` normally takes at least 500mb RAM, creating issues
and unfinished tasks if the server doesn't have enough memory.



# Local envs

There are plenty reasons why we recommend virtual machines specially for local environments.
Here the important ones:
   1. Portability.
      - What if my application is built to run on Debian but yours is built to run on CentOS? With container based virtualization we have to be put on different nodes. With VMs, we can share a node.
      

