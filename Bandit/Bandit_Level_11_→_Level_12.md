# **Lab Report: OverTheWire \- Bandit Level 11 tot Level 12**

* **Datum:** 26 oktober 2026  
* **Doel:** Het ontcijferen van een ROT13-rotatie (verschuiving van 13 posities) in een tekstbestand om het volgende wachtwoord te achterhalen.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het vertalen en vervangen van specifieke karakters in tekststromen via de `tr` utility.  
  * Het toepassen van tekenreeksen en alfabetische bereiken (`A-Za-z` naar `N-ZA-Mn-za-m`).  
  * Het verwerken van standaardinvoer gekoppeld via de pipe operator (`|`).

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 11 is het bestand `data.txt` aangetroffen, waarvan alle letters over 13 posities waren geroteerd volgens het ROT13-principe.  
2. **Oplossingsstrategie:** Om de versleutelde rotatie ongedaan te maken, is de `tr` utility ingezet om de invoertekst te vertalen naar het originele alfabet door middel van een gerichte karakterwisseling.  
3. **Uitvoering:** Het volgende commando is zelfstandig opgesteld en uitgevoerd:

Bash  
cat data.txt \| tr 'A-Za-z' 'N-ZA-Mn-za-m'

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 12):** `GROozWP08QyN0mGrjUkID0WCYKzIqxrN`  
* **Status:** Succesvol voltooid en gedocumenteerd.

