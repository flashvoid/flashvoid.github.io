---
layout: post
title: "AWSCLI filter by tag"
date: 2014-08-22 23:50:43 +0000
comments: true
categories: [ aws, awscli, examples ]
---

[AWS command line tool]("https://github.com/aws/aws-cli") really missing some good documentation on how to filter by tag

Filter by tag OR tag value
```bash
  aws ec2 describe-instances --filters Name=tag-value,Values=prod
  aws ec2 describe-instances --filters Name=tag-key,Values=environment
```

Filter by tag AND value
```bash
  aws ec2 describe-snapshots --filter Name=tag:Lineage,Values=syd-pg-prod
```
