### **Lab Report: OverTheWire \- Bandit Level 4 tot Level 5**

* **Datum:** 24 oktober 2026  
* **Doel:** Het identificeren van het enige mens-leesbare bestand uit een reeks bestanden met identieke groottes binnen een specifieke directory.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het analyseren van bestandsattributen en inhoudstypen.  
  * Het correct adresseren van bestanden die beginnen met speciale tekens (mintekens) via relatieve paden (./).  
  * Het toepassen van reconnaissance binnen geneste mappen.

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 4 is de map inhere betreden. Met het commando ls \-la is de inhoud geïnspecteerd, waarbij een reeks bestanden van file00 tot en met file09 werd aangetroffen die elk dezelfde grootte bleken te hebben.  
2. **Probleemstelling:** Het direct uitlezen van de bestanden faalde aanvankelijk doordat de bestandsnamen met een minteken begonnen, en omdat de meeste bestanden binaire data bevatten die niet direct leesbaar zijn in de terminal.  
3. **Oplossingsstrategie:** Door gebruik te maken van de eerdere lessen over bestandsnamen met mintekens is de relatieve padnotatie (./) toegepast in combinatie met de commando's om de bestanden stuk voor stuk te controleren op mens-leesbare ASCII-tekst.  
4. **Uitvoering:** Na het testen van de bestanden bleek file07 de juiste ASCII-inhoud te bevatten, welke is uitgelezen met:  
5. Bash

cat ./-file07

6.   
7. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 5):** 6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG  
* **Status:** Succesvol voltooid en gedocumenteerd.

