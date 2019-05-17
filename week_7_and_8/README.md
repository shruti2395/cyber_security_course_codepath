# Week 7 and 8 - Wordpress Vulnerabilities

## Setup

Install Vagrant in Ubuntu

Setup Wordpress site using WPDistillery - Wordpress Version: 4.2

Kali Linux in Virtualbox

![kali wpscan](https://github.com/shruti2395/cyber_security_course/raw/master/week_7_and_8/kali_wpscan.gif "Running wpscan in Kali Linux")

> Objective: Find, analyze, recreate, and document **vulnerabilities** affecting an old version of WordPress

## Exploit 1. Stored XSS
  - [X] Summary: 
    - Vulnerability types: XSS
    Summary: 4.2 version of Wordpress is vulnerable to a stored XSS attack. An unauthenticated attacker can inject JavaScript code in       the Wordpress comments and JS code is executed when comment is viewed by anyone.

    - Tested in version:4.2
    - Fixed in version: 4.2.1
  - [X] GIF Walkthrough: 
  - [X] Steps to recreate: 
      - Add a new post with image which named as XSS alert
      - Add a comment to inject JS code, which should be more than 64 kb.
      - Click on the image, you will see an alert box. 
  - [X] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/changeset?sfp_email=&sfph_mail=&reponame=&new=32311%40branches%2F4.2&old=32300%40branches%2F4.2)

## Exploit 2. Vulnerability XSS
  - [X] Summary: Admin can run XSS on the page
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.6.1
  - [X] GIF Walkthrough: 
  - [X] Steps to recreate: 
     - Create new page
     - Add the code which triggers XSS alert on load: testing_xss <img src = "#" onerror="alert('xss')">
  
## Exploit 3. Vulnerability Name or ID : USER Enumeration
  - [X] Summary: This exploit allowes user to enumerate through different user names, I tested with multiple non-existing usernames, and        extisting usernames. Upon knowing the valid username or usernames, it is easier to perfrom bruteforce attack. 
    - Vulnerability types: User enumeration
    - Tested in version: 4.2

  - [X] GIF Walkthrough: 
  - [X] Steps to recreate:
    - Try with multiple user names with including the existing usernames
    - See how the response is differ from the non-existing user or existing user. 

