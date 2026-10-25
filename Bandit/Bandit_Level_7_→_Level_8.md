# **Lab Report: OverTheWire \- Bandit Level 7 tot Level 8**

* **Datum:** 25 oktober 2026  
* **Doel:** Het filteren van specifieke tekstregels uit een groot databestand op basis van een zoekwoord.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het doorsturen van bestandsinhoud via de pipe operator (\|).  
  * Het zoeken naar specifieke patronen binnen tekststromen met behulp van de grep utility.  
  * Het analyseren van gestructureerde output in de terminal.

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 7 is de inhoud van de home-map geïnspecteerd met ls, waarbij het bestand data.txt is aangetroffen. De doelstelling vereiste het vinden van het wachtwoord dat zich naast het zoekwoord millionth bevond.  
2. **Oplossingsstrategie:** Om te voorkomen dat het volledige bestand handmatig gelezen moest worden, is de inhoud van data.txt doorgestuurd via een pipe (\|) naar de grep utility om direct te filteren op de target string.  
3. **Uitvoering:** Het volgende commando is zelfstandig opgesteld en uitgevoerd:  
4. Bash

cat data.txt \| grep millionth

5.   
6. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 8):** VR1ljMayciFxbnUokuQmJfW6QC9VKtub  
* **Status:** Succesvol voltooid en gedocumenteerd.

