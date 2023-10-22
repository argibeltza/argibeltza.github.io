---
layout: single
title: Pickle-Rick-CTF-Tryhackme Machine
excerpt: "This page will be the steps to follow to complete the tryhackme Pickle Rick CTF machine."
date: 2023-10-23
classes: wide
header:
  teaser: /assets/images/Rick/logo.png 
  teaser_home_page: true
  icon: /assets/images/thm.png
categories:
  - Tryhackme
tags:
  - CTF
  
---

This machine is easy to tryhackme in difficulty.

![](/assets/images/Rick/logo2.PNG)

## Step 1

To perform the scan we will need the **nmap** tool and the **IP of the machine to attack**.

![](/assets/images/Rick/R-1.PNG) 


## Step 2

We used **Gobuster** to discover hidden directories of the website.

![](/assets/images/Rick/R-2.PNG) 

It has found a directory called **Robots.txt** and **Login.php**.


## Step 3

We can find the user for the login in the **default page** (in **source view**).

![](/assets/images/Rick/R-3.1.PNG) 

And in the **Robots.txt** we can find the password for the login.

![](/assets/images/Rick/R-3.2.PNG)  

## Step 4

Once inside we can see a **command panel**, doing a **ls** we find the first ingredient.

![](/assets/images/Rick/R-4.PNG)  

To do this we will need to place the path name of the .txt **in the url.**

![](/assets/images/Rick/R-5.PNG)

## Step 5

Searching the machine we can find the **second ingredient** in **Rick's home**.

![](/assets/images/Rick/R-6.PNG)

With the **less command** we can view this file

![](/assets/images/Rick/R-6.1.PNG)

## Step 5

Doing **sudo -l** we find that it has **root permissions** **without** the need for any **password**.

![](/assets/images/Rick/R-7.PNG)

Looking in the **root directory** we find the last of all the ingredients.

![](/assets/images/Rick/R-7.1.PNG)

With the **less command** we can view this file.

![](/assets/images/Rick/R-7.2.PNG)


## Step 6

With this, we have completed the Rick's machine on TryHackMe.

![](/assets/images/Rick/R-8.PNG)

I hope it has been helpful to you :D. **Argibeltza 10/23/2023**
