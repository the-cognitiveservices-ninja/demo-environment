---
title: Demoscript English
tags:
  - virtual assistant
  - english
  - chat bot
  - voicebot
---

# Demoscript English
version: v0.6

## background image
customer specific background: call/email holger.imbery@global.ntt

## Demo script
Bot:
Hi! I'm a virtual agent.   
You can talk to me like a human being.   
So, what can I help you with today?   


### Usecase: Outstandings
```available: chat & voice```

You:   
 - *I have issues with my payment* OR   
 - *i have outstandings*   


Bot:
You have problems paying your fees; in principle, this is not a problem.     
I need some information from you. What is your name, please?    

You: *say your name*   

Bot:   
Thank you! And your customer number, please?      

You: *say a number*

Bot:   
Do you want to pay in instalments or all at once?   

You: all at once   

Bot:   
Unfortunately, I can't connect you to the billing office at this time because all members of staff are busy.      
Can we fix a callback?   

You: Yes   

Bot:    
We need your phone number in international format, starting with 49 for Germany.   
Please give me the phone number for the callback?  

You: *say your mobile number - or 49 151 123456*   

Bot:   
Is it possible to call you back tomorrow at 2:30 pm?   

You: no   

Bot:   
We are available on weekdays between 8:30 am and 04:30 pm.   
When would it be possible for you to call you back?    

You:  *say next friday, 9 am*

Bot:   
We will call you back at the proposed time.      

### Usecase: attendant aka IVR
```available: voice```

You:   
*Í want to order* OR   
*I want to talk to a sales assistant*  OR   
*I want to talk to sales*   


Bot:
with pleasure      
What do you want to talk about?   

You: *say your wish*

Bot:   
Please give me your customer number?   
You: *say a number like 224454*

Bot:   
Bot:   
*the bot will transfer the call to Holgers phonenumber, so give a hint, and he will pick up*   

Bot will create a Message with *customernumber* and *transferreason* in a MSTeams Channel.   
To show the message, you need to be kocked in in the ddcoms.onmicrosoft.com - Tenant   
[CallQueue Channel](https://teams.microsoft.com/l/channel/19%3a3aaf05d19a9f487db702586ce12977e6%40thread.tacv2/CallQueue?groupId=5c9297ab-bb81-48f5-869a-0bb06d597eb4&tenantId=81814973-9a47-4fb4-8feb-139dcaef5bc8)  


### Usecase: FAQ 
```available: chat ```

You: where are your shares traded?       

Bot: *bot gives a detailed answer*

You: *ask different - get the same or translated answer back*
```
on which stock exchange are your shares
```
```
where are your shares listed
```
```
waar staan uw aandelen genoteerd?
```
```
ಯಾವ ಸ್ಟಾಕ್ ಎಕ್ಸ್ ಚೇಂಜ್ ನಲ್ಲಿ ನಿಮ್ಮ ಷೇರುಗಳಿವೆ
```
```
किस स्टॉक एक्सचेंज पर आपके शेयर हैं
```
```
ਤੁਹਾਡੇ ਸ਼ੇਅਰਾਂ ਦੀ ਸੂਚੀ ਕਿੱਥੇ ਹੈ
```
```
où vos actions sont-elles cotées
```

#### translation 
translation via cognitive services

   * language detection
   * language translation any to german
   * natural language understanding to catch the intent
   * lookup for answer
   * translating to source language
