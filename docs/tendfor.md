---
title: Demoscript Tendfor Contact Centre English
tags:
  - Contact Centre
  - english
  - MS Teams
---

# Demoscript English

## Prerequisites
  - install Microsofts Remote Desktop Experience and use the following logins to access the 3 independend machines,   
    please do _not setup_ MFA, please skip setup if asked.
    - use subscribe with URL: 
    ```
    https//rdweb.wvd.microsoft.com/api/arm/feeddiscovery
    ```
    - Admin: hans.ente@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone:  #{nttdemouserphone2}#
    - User: petra.ente@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone: #{nttdemouserphone1}#
    - User: nadine.maus@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone: #{nttdemouserphone3}#
    - all three are in queue sales
      
## Please do NOT
  - delete or modify the clients, even if you are able to do so !!! we trust you !!

## Begin:
log-in in all cloudpcs and make sure all agents are online
open needed browser tabs to avoid log-in dialogues

## Demo: Experience Overview
  - Use nadine.ente@ddcoms.onmicrosoft.com to show
    -  Agent Experience in MS Teams
    -  Agent Experience in Tendfor Client
    -  Agent Experience in WebClient (Browserbookmark)
    -  Attentant Experience in Tendfor Client
      -   demonstrate phonetic search
    - mobile experience (stream your mobile)

## Demo: Call Queue (in several experiences)
  - call #{nttdemouserphonequeue}#
  - talk about the possibility to configure queues and prompts
  - take call and demonstrate call forward to 2nd level

## Demo: Wallboard Experience
  [Wallboard for Sales Queue](https://tendforhosting.cloudspace.se/wb/1)   
  adust Browserzoom to show all panels
  
## Demo: Admin Experience
  - use hans.ente@ddcoms.onmicrosoft.com
  - show [statistics](https://tendforhosting.cloudspace.se/statistics/queue)   
    and describe how the statistic can be modified
  - show [Admin Interface](https://tendforhosting.cloudspace.se/admin)
    - go to "interaction queue" and describe "sales_queue"
    - go to SLA Profiles
    - go to Absence Codes
    - go to Event Handles
    - go to Wallboard
    - go to Auto Attendant 
    - go to Vistitor Flow


### Admin Hints   
  - please *skip* setting up MFA after login!!!
  - pin "Adoption Bot" to Menu, using the "..." Menu and a right click
  - pin "Tendfor" to Menu, using the "..." Menu and a right click

## Environment 
  - please find the Tendfor Portal as a bookmark in edge
  - please find the Tendfor Client installed (to demo poweruser environment)
