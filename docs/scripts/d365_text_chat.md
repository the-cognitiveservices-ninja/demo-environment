---
title: Dynamics 365 customer service textchat with human escalation
tags:
  - omnichannel contactcenter
  - Power Virtual Agents
  - Dynamics 365 customer service
  - text chat with human escalation
---

## Demo Script

Text Chat:  
[webchat](https://www.nttdemo.de/d365)

## Dialog

* You:  
  please enter the name "Claudia Mazzanti" in the name flield of the pre-conversation survey and tick the consent box

* Bot:  
  Welcome! I’m a virtual agent. You can chat with me like you would talk to a human.

### user case: simple question
* You:  
  When is the store open  

* Bot:  
  Our store hours are
  Monday-Friday 9am-5pm and
  Saturday 10am-2pm.
  Sunday, we are closed.

### use case feedback, Customer Satisfacion Survey
* You:  
  yes  
  5 star  
  yes  

### use case: Question with answer from D365 customer service knowledge base
* You:  
  Do I Need to Clean My Steam Wand After Every Use?

* Bot:  
  Please wait, I search for an answer.  

* Bot:  
 displays the content of the knowledgebase article

### use case feedback, Customer Satisfacion Survey
* You:  
  yes  
  5 star  
  yes  

### user case: question with power automate flow - simulation of a third party integration
you can go two times through the dialog, make sure you enter a city with a temperature above 25C and one with a temperature below 25C

* You:  
  What is the weather  

* Bot:  
  Of course, I can share the weather with you! Can you tell me the name of the region where you want to know the weather?  

* You:  
  Dakar (or another city) 

* Bot:  
  displays the temperature within a whole sentence

### use case feedback, Customer Satisfacion Survey

* You:  
  yes  
  5 star  
  yes  

### human escalation

* You:  
  I want to talk to a support agent  

* Bot:  
  Is your query product related?  

* You:  
  Yes  

* Bot:  
 Which product?  

* You:  
  smart brew 1000  

* Bot:  
  What is the topic?  

* You:  
  I want to install a water filter 

* Bot:  
  Please wait, I connect you to a human colleague.  
  the bot connects you to a human for a live chat

## use case live chat - human to human interaction with livetranslation
Agent: Hallo, wie kann ich Dir helfen  
User: I want to install a water filter?  

Agent in Copilot: How do i install a water filter  

Agent: Ich kann Dir eine Anleitung senden, ist das ok?  
User: Ok  

Agent "Press sent to Customer"  

User: Thank you, I will try.  
User closes  

Agent sees summary and creates case.  






