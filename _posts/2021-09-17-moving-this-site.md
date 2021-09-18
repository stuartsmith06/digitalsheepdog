---
layout: post
title: "Moving This Site"
author: "Stuart"
tags: Cloudflare
---

You may have heard over the past few months some of the "cancel culture" events news.  In particular, Amazon and the AWS platform made a decision to remove some conservative platforms such as Parler.  While I don't really want to get into the why's and wherefore's of the AWS decision, I emphatically disagree with the decision.  Regardless if you're conservative, liberal, or middle-of-the-road from a political perspective, everyone should disagree with this decision.  That being said, I have decided to move all the domain names and sites I have hosted on AWS elsewhere.   

This site now actually "lives" on GitHub and is front-ended with CloudFront DNS and CloudFront Pages!

This option of tech is completely free (with AWS I was paying a nominal charge for S3 storage, a CloudFront distribution, and TLS certificate), with the exception the domain registration.  The domain registration is actually cheaper ($8.00 with CloudFlare vs. $12.00 with AWS Route53), and arguably there are more security features with CloudFlare.  I'm also already using CloudFlare's DNS on my home network.
