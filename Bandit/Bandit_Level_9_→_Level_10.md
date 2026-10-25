# **Lab Report: OverTheWire \- Bandit Level 9 tot Level 10**

* **Datum:** 25 oktober 2026  
* **Doel:** Het extraheren en filteren van mens-leesbare tekststrings uit een binair bestand op basis van specifieke patroontekens.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het analyseren van binaire en gecompileerde bestanden via de `strings` utility.  
  * Het filteren van tekststromen met de `grep` utility op basis van specifieke karakterpatronen (`===`).  
  * Het combineren van data-extractie en filtering via de pipe operator (`|`).

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 9 is het bestand `data.txt` aangetroffen. Het direct uitlezen van dit bestand met de standaard `cat` utility resulteerde in onleesbare binaire uitvoer.  
2. **Oplossingsstrategie:** Aangezien het bestand niet uit platte tekst bestaat, is de `strings` utility ingezet om alle afdrukbare ASCII-reeksen te extraheren. Om te voorkomen dat het handmatig doorzoeken van de uitvoer te veel tijd kostte, is het resultaat via een pipe doorgestuurd naar `grep` om specifiek te filteren op regels met herhalende gelijktekens (`===`).  
3. **Uitvoering:** Het volgende commando is opgesteld en uitgevoerd:  
4. Bash

strings data.txt \| grep \===

5.   
6. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 10):** `B0s2khmbT9u@geKuOOvGW3JZKhndE3BG`  
* **Status:** Succesvol voltooid en gedocumenteerd.

