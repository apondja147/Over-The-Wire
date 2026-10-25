# **Lab Report: OverTheWire \- Bandit Level 5 tot Level 6**

* **Datum:** 25 oktober 2026  
* **Doel:** Het identificeren en extraheren van een bestand met specifieke grootte- en eigendomskenmerken binnen een geneste mappenstructuur.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het recursief lokaliseren van bestanden via de find utility op basis van byte-grootte (-size 1033c).  
  * Het navigeren door subdirectories en het uitlezen van bestandsinhoud via de cat utility.  
  * Het scheiden van binaire bestanden en leesbare ASCII-data binnen een Linux-omgeving.

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 5 is de map inhere onderzocht, waarin twintig geneste mappen (maybehere00 tot en met maybehere19) werden aangetroffen.  
2. **Oplossingsstrategie:** Om te voorkomen dat de gehele server werd doorzocht (wat resulteerde in permissiefouten), is de zoekopdracht beperkt tot de huidige map door gebruik te maken van de find utility in combinatie met een filter op bestandsgrootte (1033 bytes).  
3. **Uitvoering:** Het volgende commando is uitgevoerd om het doelbestand te isoleren:  
   Bash  
   find . \-size 1033c

   Dit leverde het pad ./maybehere07/.file2 op. Vervolgens is dit bestand uitgelezen met:  
   Bash  
   cat ./.file2

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 6):** P4eMMCwgzUFMyGY3NReZ84kHYjIaRZAG  
* **Status:** Succesvol voltooid en gedocumenteerd.

