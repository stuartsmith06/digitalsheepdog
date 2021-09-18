---
layout: post
title: "DNS: what it is and why you should change yours"
author: "Stuart"
tags: DNS
---

DNS, or Domain Name System (sometimes called Domain Name Service) is a system (or service) that translates easy to understand domain names into IP addresses.  An analogy for DNS is it's like the telephone book of the Internet (for those under 30 who don't know what a telephone book is, it's a big book that telephone companies used to publish that had a list of people, their home addresses, and telephone numbers).  

When you type a website address, called a "fully qualified domain name" or FQDN, into your web browser's address bar, your computer actually needs the web server's Internet Protocol (IP) address in order to connect to the website.  For example, the address for my site, digitalsheepdog.com has an IP address of 104.21.60.152.  When you type in "www.digitalsheepdog.com", your computer does a DNS <i>query</i> to get the IP address of my website.  It checks with a <i>DNS server</i> to get the IP address.

You can actually try this yourself.  If you're on a Windows computer open your command prompt, or on a Mac open terminal, then type "nslookup" and the name of any website.

What is important to know is you can actually change the DNS server your computer uses (or all the devices on your network use) to do DNS queries.  So why is this important?

<b>DNS and Security</b>

DNS is at the heart of all Internet activity, and it actually can play a critical part in the security of your entire home network.  DNS controls what websites users can get to from your network.  In particular you can block access to adult, pornographic, or any other types of sites you don't want children or others using your home network by simply using a DNS service that doesn't respond when a device does a DNS query for an objectional website.  You don't even need to install any filtering software on individual computers, phones, or tablets.  All you need to do is change your DNS server (more about this below).

Additionally, you can block malicious websites or significantly impact certain types of malicious software (malware) from infecting computers on your network.  Many types of malware have to connect back to a "command and control" server when they are doing their dirty deeds.  This is especially true for "ransomware" (more in this in a future post).  By blocking malware's ability to lookup the IP address of the website/server it's trying to connect to, you can prevent it from functioning and reduce the impact of malware infections.

So how do you do this?  Very simply, there are a few free DNS solutions that you can use.

CloudFlare is a security company that offers a free DNS service for families.  By simply changing your DNS server from the ones that your ISP provides to 1.1.1.3 (primary) and 1.0.0.3 (secondary), you can block a whole range of both malware and adult websites.  CloudFlare has an <a href="https://developers.cloudflare.com/1.1.1.1/1.1.1.1-for-families" target="_blank">article that details the service on their website</a>.

OpenDNS is another free DNS service provided by Cisco that is very similar to CloudFlare.  Their DNS servers are 208.67.222.222 and 208.67.220.220.  More information about this service is found on the [Open DNS website](https://www.opendns.com/setupguide/#familyshield).

In most cases, you'll want to change your DNS server on your router.  This will provide protects for your entire network, and all devices running on it.  But, if your router doesn't allow you to change the DNS server, you may have to do this individually on each device.

The Cloudflare and OpenDNS sites have details on how to do this on many different routers and also have instructions on how change the DNS settings on indvidual devices.  Tip:  If you're a parent of teenagers or pre-teens who have a phone or tablet, you may want to do this on your child's device in addition to your home router.  That way, they're protected when they're away from home.

Bottom line:  Using a free, secure, DNS service is a great way to keep objectionable websites off your devices and improve the security of your home network!
