---
title: Outreachy | Week 2
# date: "2022-12-16T23:46:37.121Z"
description: "Everybody struggles"
---

---
### "Everybody struggles"
 There is so much to write about this week. It was all about everybody struggles. Past 4 weeks I was not able to 
 give proper time to my internship due to some family problems. Thanks to my both mentors who helped me and encouraged me 
 to take breaks and spend time with family. Thanks to Outreachy organizers who were in contact with my mentors and helped me 
 to spend time comfortably. Outreachy organizers made sure that I am working comfortably and not getting burnout.

 So about this week, I had a bug assigned by my mentors to reproduce. 
 Bug title is "Set as Active" button shown for replicas in transitional states. It is a low-hanging-fruit bug that I needed to 
 reproduce in my environment.

**Weekly tasks**.

# Manila UI / Horizon code walkthrough 
 For understanding the Manila UI framework, my mentors had given me a brief introduction and provided a code walkthrough. 
 It was a brief introduction. Carloss has gone through briefly every module and component in OpenStack and how they are linked with each other. API calls, request, and response flow with Manila UI framework relevance which helped me to understand how to link them to the actual Manila UI. 

# First approarch was to understand the bug.
To understand the bug, I have gone through several documents and spent time reading them. My mentors have shared some of the resources
 which were also helpful. I studied about shares replication, and what types of replication types are supported for example 
 readable , writeable, and dr. Understanding active and non-active replication , as active refers to replication that can be accessed 
 to read and write records. Non-active replicas have only read access and can't be written into. Then I studied about promotion for replicas which helps in understanding the transitions of replicas.

# Reproducing the bug 
 As I had some understanding and written documents, how to approach to reproduce the bug. My mentors provided me with some resources and steps to start with. Firstly, I had checked in the backend side whether, the replication type is set Manila configurations file, after enabling the backend stanzas I had to restart manila services with the command:
 sudo systemctl restart devstack@m-*
 Then I started with the command line provided in Manila documentation, a link shared by Carloss, i followed it thoroughly to understand the flow.
 As the command line environment did not help much, I was facing some variable issues that were not loaded in my devstack environment.
 After searching online, and could not get proper help, I asked my mentors about my query. Carloss suggested to **source** the **decstack** openrc file which helped in removing the error.
 I started with exploring UI keeping in mind the workflow through the command line. I created the share type admin with the extra spec as replication_type, next type was to create a share with created share type.
 As I was instructed to create it from UI so I looked up the UI to create a share I was not able to find the option. So after help from my mentors, I was able to create a share. Now to reproduce a bug, I had a platform set in Manila UI and I had to create a shared replica and see if the set as the active button was displayed during the transition of the replica.
 Before that, I had to debug the issue which was not helping me to create a share with the low storage provided.
 I monitored after creating all the options provided so that I could see where the problem is. 
 After noticing the problem I was able to successfully create a share.
 Then I promoted the share by switching the replica to an active state and created a shred replica and during its transition, I was able to see the set as an active button.

# Open Infra Summit
My mentor Gautham also shared the Open Infra summit and its travel support program which helps financially to cover the stipend to attend the event. I am very much interested in events like these and I would love to attend if I could get an opportunity.

Bye see you with week 3rd Blog:)

