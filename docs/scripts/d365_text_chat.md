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
  I need to replace my filter  

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
  Replace a filter  

* Bot:  
  Please wait, I connect you to a human colleague.  
  the bot connects you to a human for a live chat

## use case live chat - human to human interaction with livetranslation
!!! note "Case-Chaining"

    The case is chained to the previous case "human escalation". All the customer/bot entries are prerequisite for this use case too.



* You:  
  Guten Tag {$customer fullname$}, willkommen zu unser online Chat-Service.
Mein Name ist Mike und werde Sie unterstützen Ihr Anliegen zu lösen.
Unser intelligenter Freund - Virtual Bot - hat bisher folgende Informationen eingesammelt:<br>
Name: {$customer fullname$}<br>
Einwilligung zur Verarbeitung: True<br>

  Ist dies aus Ihrer Sicht korrekt?

* Customer:  
  Yes

* You:  
  Auf Basis der bisherigen Informationen fasse ich den Fall wie folgt zusammen:
Sie möchten mit uns über ein Problem mit Ihrer Smart Brew 1000 sprechen. Insbesondere benötigen Sie Hilfe beim Austausch eines Filters. Richtig?  

* Bot:  
  Yes, exactly


