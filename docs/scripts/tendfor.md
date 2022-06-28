---
title: english Tendfor Contact Centre
tags:
  - Contact Centre
  - english
  - MS Teams
---

# Tendfor Contact Centre

## Prerequisites
  - install Microsofts [Remote Desktop Experience](https://docs.microsoft.com/en-us/windows-server/remote/remote-desktop-services/clients/windowsdesktop#install-the-client) and use the following credentials to access the three independent machines,   
    please do _not setup_ MFA, and please skip setup if asked.
    - use "subscribe with URL": 
    ```
    https//rdweb.wvd.microsoft.com/api/arm/feeddiscovery
    ```
    - Admin: hans.ente@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone:  #{nttdemouserphone2}#
    - User: petra.ente@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone: #{nttdemouserphone1}#
    - User: nadine.maus@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone: #{nttdemouserphone3}#
 
   - WebUsers:   
    - sign in a private browser [webteams](https://teams.office.com)   
    - user bruno.ente@ddcoms.onmicrosoft.com Password: #{nttdemouserpw}#   
      Phone: no phone license but still an agent   
   - all  are in queue sales
      
## Please do NOT
  - delete or modify the clients, even if you can do so !!! We trust you !!

## Begin:
login in all cloud pcs and make sure all agents are online
open needed browser tabs to avoid login dialogues

## Demo: Experience Overview
  - Use hans.ente@ddcoms.onmicrosoft.com to show
    -  Agent Experience in Tendfor Client   
      -  show: dial out as
      -  show_ shortcuts
      -  show: devices
      -  show: roles
      -  show: search
    -  Agent Experience in MS Teams
    -  Agent Experience in WebClient (Browserbookmark)
    -  Attentant Experience in Tendfor Client
      -   demonstrate phonetic search
    - mobile experience (stream your mobile)

## Demo: Call Queue (in several experiences)
  - call #{nttdemouserphonequeue}#
  - talk about the possibility of configuring queues and prompts
    -   the demo is set to parallel ringing
  - take the call and demonstrate call forward to 2nd level
  - demonstrate with bruno.ente@ddcoms.onmicrosoft.com, user has no phone license but still is an agent

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
  - pin "Adoption Bot" to Menu, using the "..." Menu and a right-click
  - pin "Tendfor" to Menu, using the "..." Menu and a right-click

## Environment 
  - please find the Tendfor Portal as a bookmark in edge
  - please find the Tendfor Client installed (to demo power user environment)
