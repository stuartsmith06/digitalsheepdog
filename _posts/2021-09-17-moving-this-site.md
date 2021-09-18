---
layout: post
title: "Moving This Site"
author: "Stuart"
tags: web-hosting
---

One doesn’t need to think very hard to come up with some examples of the “cancel culture” trend we’re seeing in the country these days.  At the beginning of 2020, Amazon caused a big dust up when the company made a decision to remove certain social media platforms from the AWS hosting service.  While I don’t really want to get into the why’s and wherefores’ of the AWS decision, I emphatically disagree with what they did.  Regardless if one’s political views, this action to “deplatform” someone (including another company) who doesn’t share your political views is troubling.  For this reason, and some more practical reasons, I have decided to move all the domain names and sites I have hosted on AWS to Cloudflare.   

This site now actually “lives” on GitHub and is front-ended with Cloudflare DNS and Cloudflare Pages!
This combination of hosting of websites is completely free.  With AWS, I was paying a nominal charge for S3 storage, paying a monthly charge for each CloudFront distribution, and an annual charge for each TLS certificate.  The domain name registration is also cheaper, only being $8.00 with Cloudflare vs. $12.00 with AWS Route53.  Arguably there are more security features with Cloudflare.  

Lastly, the deployment is a bit more straightforward, and works well with the Jekyll static content management system I’m using.  The overall design looks like this:

<img src="/images/blog_hosting.png">

…and how it works is this:

1.	Create content on my computer using Jekyll
2.	Push updates to a GitHub repo
3.	Cloudflare Pages automatically detects changes and deploys a new “build” based on the updates in the GitHub repo
4.	Cloudflare DNS has an alias to the Cloudflare Pages address for the FQDN of Digital Sheepdog

<p>I’m also already using Cloudflare’s DNS on my home network, so it was an easy transition to using their hosting service and DNS as well.</p>
