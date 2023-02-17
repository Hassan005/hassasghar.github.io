---
title: Outreachy | Week 6
# date: "2022-12-23T22:40:32.169Z"  
description: Modifying Expectations
---
## Modifying Expectations
 I would like to talk about my progress throughout my internship until now. We started with an understanding of the OpenStack manila interface, I already have set up my environment for OpenStack in a VM provided by my mentors. I installed OpenStack though 
 the dev stack by running a series of scripts. After successfully installing OpenStack, the shares tab was missing from the WebUI of OpenStack, my mentor helped me in debugging the issue so after re-running the script we were able to see the shares tab as
 well. We started with the bug fix after exploring the WebUI of Manila, first challenge was to reproduce the bug to fix that. It took some time to reproduce the bug as getting familiar with the environment and WebUI, finally, I
 was able to reproduce the actual bug from WebUI, and I have also tried reproducing the bug through the command line as well.

 After finally reproducing the bug, the next step was to fix the bug.
 I started with understanding the code part while correlating with the actual UI of OpenStack Manila. For me, working in this environment was a little bit difficult at the start as I had not worked on Django previously so understanding the whole code 
 which was being implemented in Django was a bit challenging at the start bug thanks to my mentors who helped me by going through
 the code walkthrough which helped me to understand the structure of the code.

 I tried playing with the environment to see how code responds in the environment.
 The first solution for a bug I implemented was **Time Delay** after the replica was being set as active so it could not appear 
 while Setting the button as Active for a replica. But when I shared the solution with my mentors, they suggested that it will
 work for dummy environments but not on actual drivers which might take more time than dummy drivers.
 Then I spend almost 3 to 4 days working for a solution that would work out for actual drivers too.
 I finally came up with a solution that worked and fixed the visibility of the Set as Active button during replication change or deleting any replica, I finally shared the solution and my mentors responded with positive feedback.

 My next step was to push the code on **Gerrit**, I was familiar with this before but again environment was new so I was facing some problems with pushing the code but my mentors helped me in debugging the environment. So finally I was able to push the code on **Gerrit** but I had some problems with my code, I added some extra imports and charter for a single line I added a condition that was exceding the maximum limit. So I have gone through the other part of the code as well to find a solution for this.
 I finally pushed the code on Gerrit with the disired changes with **release not** mentioned by my mentors. Finally, it was reviewed
 by my mentors and other open-source community members and feedback was positive.

 Now as far as think I might not be up to the timeline that was set before for this project but I am heading for it and hopefully 
 in 1 or 2 weeks I would be able to achieve that.

 :)
