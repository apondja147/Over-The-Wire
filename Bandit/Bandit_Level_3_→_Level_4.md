# **Lab Report: OverTheWire \- Bandit Level 3 tot Level 4**

* **Datum:** 24 oktober 2026  
* **Doel:** Het identificeren en uitlezen van een verborgen bestand binnen een specifieke directory.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het opvragen van verborgen bestanden met behulp van de \-la optie in de list-directory (ls) utility.  
  * Navigatie binnen geneste directory-structuren (cd).  
  * Het correct benaderen van bestanden met afwijkende voorvoegsels en karakters.

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 3 is de aanwezige map inhere geidentificeerd. Na het betreden van deze map gaf een standaard ls commando geen resultaten, wat duidde op de aanwezigheid van bestanden met een afwijkend attribuut.  
2. **Probleemstelling:** Linux en Unix-achtige systemen verbergen bestanden en mappen waarvan de naam begint met een punt (.) standaard voor de gebruiker om overzicht te bewaren.  
3. **Oplossingsstrategie:** Om de verborgen bestanden zichtbaar te maken, is de ls utility gekoppeld aan de \-la vlag, waarbij \-l zorgt voor een gedetailleerde lijstweergave en \-a (*all*) de verborgen objecten toont.  
4. **Uitvoering:** Na het uitvoeren van het commando werd het verborgen bestand ...Hiding-From-You aangetroffen. Dit is uitgelezen via een relatieve padnotatie:  
5. Bash

cat ./...Hiding-From-You

6.   
7. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 4):** xzTXqlrDJQVVAzdv5chq1TQytTWufAMQ  
* **Status:** Succesvol voltooid en gedocumenteerd.

