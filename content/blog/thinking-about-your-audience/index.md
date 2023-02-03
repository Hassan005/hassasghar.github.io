---
title: Outreachy | Week 4 & 5
# date: "2022-12-23T22:40:32.169Z"  
description: Thinking about your Audience Cont.
---

### Thinking about your Audience
As I come from a Computer Science background, most people in my community come from the same background. As this field is rapidly growing and evolving every single day, one has to keep him/her self updated wth what's happening around them. I am usually asked whom I am interning with? and my answer would be OpenStack Manila, as most of my friends are not aware of this, I would explain to them about OpenStack as an opensource cloud computing platform used to build private as well as public clouds and Manila is shared filesystems as a service.

# What is OpenStack?
 A suite of software tools called OpenStack is used to create and manage cloud computing systems for both public and private clouds. Many believe that OpenStack is the future of cloud computing since it is supported by some of the biggest names in software development and hosting as well as thousands of individual community members.
# What is Manila?
In OpenStack, we have a shared filesystem service called Manila. It works similarly to Cinder (block storage). With Manila, you can create a shared filesystem and perform management activities such as visibility, accessibility, and usage quota. Manila supports file sharing protocols such as NFS, CIFS, HDFS, and GlusterFS.
A shared filesystem also allows us to define security using the following:
**DNS IP of tenant network**
**Security service IP or hostname**
**Security**

# Problem Satement 
There are a few ways to consume Manila shared filesystems with their several features, being the Command Line Interface, the more graphical User Interface (the OpenStack Dashboard - "Horizon" plugin), and also the REST APIs directly. The Manila User Interface is currently falling behind the features offered by the Manila API. The idea of this project is to cover the gaps of the previous development cycles, where new features were added to the API, but not added to the User Interface, and add Unit Test coverage to such features.
Manila provides a way to provision remote, sharable file systems (shares) which can be accessed by multiple instances simultaneously and file systems can have access rules assigned to control read-write and read-only access to the file system 


# Required Skills
As far as I understand required skills for working on this project are python, Django framework understanding, Linux understanding, how to debug your problem, and mainly understanding OpenStack and its working and functionality of manila shared file system.


# My approach
As I started working on this project main hurdle I was facing initially was understanding OpenStack and it's shared file system upon which I had to work.
I have spent some initial days Understanding OpenStack and its components.
As its code is written in Django, understanding Django was the next hurdle I faced. After reproducing the bug and understanding visually on WebUI bug fix, I had to implement the solution in Manila UI.
My mentors have supported me through this whole learning process and helped me in debugging problems, providing code overviews, and helpful resources.

As I have discussed above, OpenStack is backed by a huge community and tech giants, developed and maintained by thousands of software engineers working across the globe for its better performance and scalability. So working on this project and collaborating with the OpenSource community is quite exciting to me. 

# What I learned
I am still in process of learning and I believe that with time it will get better. I have Learned OpenStack and its works through WebUI, I have played around with its different components mainly Manila shares. I have learned Django as its core part of a project.
As far as I think, the internship period is 3 months so you should have enough skills to get started, also as a part of your internship learning is also important so you learn a lot by implementing them.

I am very excited about this project with the support of my mentors and with giving time and effort I hope i would be able to achieve good results.

See you :)



