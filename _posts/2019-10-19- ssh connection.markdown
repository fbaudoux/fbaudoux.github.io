---
layout: post
title:  "Connexion via ssh"
date:   2019-10-19 22:24:34 +0200
categories: linux ssh
---

I want to connect as a particular user (let's say remoteUser for example) to a machine using ssh without typing any passport.  
I just have to :  
* copy the content of my local public key ( __~/.ssh/id_rsa.pub__)
* paste it into the authorized_keys file of remoteUser (__/home/remoteUser/.ssh/authorized_keys__) of the remote system.  

Then I can connect the remote system using : 
```
 ssh remoteUser@remoteMachineIp
```
