# **Lab Report: OverTheWire \- Bandit Level 1 tot Level 2**

* **Datum:** 24 oktober 2026  
* **Doel:** Het uitlezen van een bestand waarvan de naam identiek is aan een speciaal teken, waarbij wordt voorkomen dat de shell dit teken interpreteert als een commando-optie.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Omgaan met speciale karakters in bestandsnamen.  
  * Het gebruik van relatieve paden (./) om ambiguïteit in de command-line parser op te lossen.  
  * Bestandstoegangsrechten en eigendom binnen de Linux-directory.

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op de server is met het commando ls \-la de inhoud van de home-map geëvalueerd. Hierbij werd geconstateerd dat er een bestand aanwezig is met als naam een enkel minteken (\-).  
2. **Probleemstelling:** Het direct aanroepen van het commando cat \- faalt of resulteert in een hangende terminal, omdat de shell een enkel minteken interpreteert als het starten van een parameter of optie in plaats van een bestandsnaam.  
3. **Oplossingsstrategie:** Om de shell te dwingen het minteken als een fysiek bestand in de huidige map te beschouwen, dient het pad expliciet te worden meegegeven door middel van een relatieve padnotatie met een punt en een slash (./).  
4. **Uitvoering:** Het volgende commando is uitgevoerd om de inhoud correct te extraheren:  
5. Bash

cat ./-

6.   
7. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 2):** PK8FYLZg2hnHSZ83pLBL1iEPkdD3QToB  
* **Status:** Succesvol voltooid en gedocumenteerd.

