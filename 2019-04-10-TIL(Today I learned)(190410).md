---
layout: post
title: "TIL(Today I learned)(190410)"
date: 2019-04-10
blog : true
author : Donghoon Song
summary : "Today I learned"
permalink : /TIL/:year/:month/:day/:title
comments: true
tag: TIL
---

### DHCP : Dynamic Host Configuration Protocol : dynamically get address from as server

→ plug-and-play
→ management하기 좋다.
   1. IP address
   2. netmask
   3. Domain Name Server

goal : allow host to dynamically obtain its IP address from network server when it joins network

- can renew its lease on address in use
- allows reuse of addresses (only hold address while connected/"on")
- support for mobile users who want to join network (more shortly)

DHCP overview :

- host broadcasts "DHCP discover" msg [optional]
- DHCP server responds with "DHCP offer" msg [optional]
- host requests IP address : "DHCP request" msg
- DHCP server sends address : "DHCP ack" msg