---
layout: post
title: Web Session Cookie Attacks
date: 2023-03-27 00:24
category: [Cybersecurity]
author: Konrad Lazarski
tags: [cybersecurity, web applications]
summary: 
---

## Introduction  
What prompted me to write this post was hearing about how Linus Tech Tips (a major technology YouTube channel) was compromised in March of 2023. Their channel was used to post crypto scam videos. Password and 2FA protections were bypassed since the bad actor targeted session tokens stored within a web browser. Methods of preventing this attack will also be discussed.

## Background
Let's start with a basic understanding of what a cookie is. It is a piece of data that is placed on your computer when you’re browsing the internet. These text files are automatically created by browsers and websites. Websites like Facebook or Amazon use a session cookie to store your login credentials. This provides you with a more seamless browsing experience since without it you would have to log into a site every time you reopened your web browser.

## The Vulnerability 
Session Hijacking is a technique hackers use to steal session IDs to gain access to private systems and personal accounts without even having to enter in a username and password. Adversaries can send emails with attachments that on the surface seem harmless pdf files. However once a unsuspecting user clicks on the attachment a script runs in the background that grabs the session cookies from their web browser. All the adversary has to do is copy the values of the cookies from the victim's computer onto their computer and gain access to the victim's account. 

## Video Explanation 
<iframe width="560" height="315" src="https://www.youtube.com/embed/Yeik-Ks-q8U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>