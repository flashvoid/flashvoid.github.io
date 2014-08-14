---
layout: post
title: "OHAI vs ec2 VPC bug"
date: 2014-08-14 08:07:48 +0000
comments: true
categories: [ aws, ec2, vpc, chef, ohai ]
---

Now, I hit that [bug](https://tickets.opscode.com/browse/OHAI-310) twice already. It take some effort to pull the solution out from a head.



solution: use ohai hints
```bash
touch /etc/chef/ohai/hints/ec2.json
```
