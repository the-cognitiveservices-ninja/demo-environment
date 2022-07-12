---
title: german virtual assistant (voice/chat)
tags:
  - virtual assistant
  - german
  - chat bot
  - voicebot
---

# Demoscript German
version: v0.6

!!! note "Note:"

    * please find links and phonenumbers on the [available demos table](https://www.nttdemo.de/scripts)

## background image
customer specific background: call/email holger.imbery@global.ntt

## Demo script
Bot:
Hallo! Ich bin ein virtueller Agent.   
Sie können mit mir wie mit einem Menschen sprechen   
Also, womit kann ich Ihnen heute helfen?   


### Usecase: Offene Rechnung/Gebührenbescheid
```available: chat & voice```

You: Ich kann meine Rechnung/Gebühren nicht begleichen   

Bot:
Sie können Ihre Ausstände nicht begleichen, dass ist prinzipiell kein Problem.   
Ich benötige einige Informationen von Ihnen. Wie ist Ihr Name bitte?   

You: *say your name*   

Bot:   
Danke! Und nun Ihre Kundennummer, bitte ?   

You: *say a number in digits 4 4 1 2 9 8*

Bot:   
Möchten Sie die Ausstände in Raten oder auf einmal zahlen?   

You: in Raten   

Bot:   
Zur Zeit ist leider kein Mitarbeiter in der Rechnungsstelle verfügbar.   
Können wir sie zurückrufen?   

You: Ja   

Bot:    
Wir benötigen Ihre Telefonnummer im internationalen Format, beginnen sie mit 49 für Deutschland.    
Bitte geben Sie mir Ihre Telefonnummer für den Rückruf   

You: *say your mobile number - or 49 151 123456*   

Bot:   
Können wir Sie morgen um 14:30 Uhr zurückrufen?   

You: nein   

Bot:   
Wir sind wochentags zwischen 8:30 Uhr und 16:30 Uhr erreichbar. Der Rückruf wird in einem Fenster
von 30 Minuten um Ihren Wunschtermin stattfinden. Wann können wir Sie zurückrufen?   

You:  *say nächsten Mittwoch, 9 Uhr 15*

Bot:   
Wir rufen Sie zum vereinbarten Zeitpunkt zurück.      

### Usecase: attendant aka IVR
```available: voice```

You:   
*Ich möchte mit dem Vertrieb sprechen* OR   
*Ich möchte mit der Ausländerbehörde sprechen*  OR   
*Ich möchte mit dem Gesundheitsamt sprechen*   


Bot:
Gerne   
Worüber möchten Sie sprechen ?   

You: *say your wish*

Bot:   
Geben Sie mir bitte Ihre Kundennummer?   

You: *say a number like 4 4 1 2 9 8*

Bot:   
*the bot will transfer the call to Holgers phonenumber, so give a hint, and he will pick up*   

Bot will create a Message with *customernumber* and *transferreason* in a MSTeams Channel.   
To show the message, you need to be in the ddcoms.onmicrosoft.com - Tenant   
[CallQueue Channel](https://teams.microsoft.com/l/channel/19%3a3aaf05d19a9f487db702586ce12977e6%40thread.tacv2/CallQueue?groupId=5c9297ab-bb81-48f5-869a-0bb06d597eb4&tenantId=81814973-9a47-4fb4-8feb-139dcaef5bc8)
 


### Usecase: FAQ - public sector
```available: chat ```

You:  
```
Was kostet ein Wunschkennzeichen?    
```

Bot: *bot gives a detailed answer*

You: *ask different - get the same or translated answer back*
```
wie kann ich ein Wunschkennzeichen bekommen
```
```
How much does a desired license plate cost?
```
```
Hoeveel kost een gewenst kenteken?
```
```
كم تبلغ تكلفة لوحة الترخيص المطلوبة؟
```
```
Combien coûte une plaque d’immatriculation souhaitée?
```

#### translation 
translation via cognitive services

   * language detection
   * language translation any to german
   * natural language understanding to catch the intent
   * lookup for answer
   * translating to source language

