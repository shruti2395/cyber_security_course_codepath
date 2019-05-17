# Week 9 Project: Pentesting Live Targets

## Overview:

Get hands-on experience with some of the most common security exploits through an applied hacking exercise.


For this assignment, you will atack three live targets, each of which is a slightly modified version of the same web application, Globitek. The three targets are therefore mostly identical. However, each target has been given a different color menu bar—blue, green, red—and each one has two different security vulnerabilities.


## Challenge Goals:

The following goals must be completed:

## 1. Username Enumeration: 
A careless developer mistake has created a username enumeration vulnerability. Determine which color has the vulnerability. You can use the existing username "jmonroe99" as a test. Next, figure out what mistake the developer made.

![Username Enumeration](https://github.com/shruti2395/cyber_security_course/raw/master/week_9/UserEnum.gif "Username Enumeration attack")

## 2. Insecure Direct Object Reference:
One of the three sites is missing code which would prevent some sensitive information from being made public. Determine which color has the vulnerability. Then, figure out what the other two sites did correctly to prevent the information leak.

![Insecure Direct Object Reference](https://github.com/shruti2395/cyber_security_course/raw/master/week_9/SQL%20Injection.gif "Insecure Direct Object Reference attack")

## 3. SQL Injection:
Most of the data input received by these websites is being sanitized properly. However, one of the three sites has one place where the input is not being sanitized before being used in an SQL query. Determine which color has the vulnerability.

![SQL Injection](https://github.com/shruti2395/cyber_security_course/raw/master/week_9/IDOR.gif "SQL Injection attack")
