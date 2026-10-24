### **Lab Report: OverTheWire \- Bandit Level 2 tot Level 3**

* **Datum:** 24 oktober 2026  
* **Doel:** Het benaderen en uitlezen van een bestand met complexe spaties en streepjes in de bestandsnaam.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het automatisch aanvullen van bestandsnamen via Tab-completion (Tab toets).  
  * Escaping van speciale karakters en spaties binnen een bestandsstructuur.  
  * Het correct adresseren van bestanden in de huidige werkmap via relatieve padnotatie (./).

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na het inloggen op Bandit Level 2 is met ls \-la de inhoud van de home-map bekeken. Hier werd een bestand aangetroffen met de naam \--spaces in this filename--.  
2. **Probleemstelling:** Het rechtstreeks aanroepen van het bestand faalt vanwege de spaties (die door de shell als scheidingstekens worden gezien) en de dubbele mintekens vooraan (die door commando's worden aangezien voor opties of vlaggen).  
3. **Oplossingsstrategie:** In plaats van handmatig alle escape-tekens en aanhalingstekens te typen, is gebruikgemaakt van de automatische **Tab-completion** in de shell. Door de eerste letters te typen en op de Tab-toets te drukken, vult de terminal de benodigde backslashes (\\) automatisch in, gecombineerd met de relatieve padnotatie (./).  
4. **Uitvoering:** Het volgende commando is automatisch gegenereerd en uitgevoerd:  
5. Bash

cat ./'--spaces in this filename--'

6.   
7. (Zoals te zien in de terminal output leidde dit direct tot het uitlezen van de inhoud).

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 3):** 7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME  
* **Status:** Succesvol voltooid en gedocumenteerd.

