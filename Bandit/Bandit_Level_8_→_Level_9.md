# **Lab Report: OverTheWire \- Bandit Level 8 tot Level 9**

* **Datum:** 25 oktober 2026  
* **Doel:** Het filteren van een unieke regel tekst die exact één keer voorkomt in een groot databestand.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het alfabetisch sorteren van gegevensstromen via de sort utility.  
  * Het filteren van duplicaten of unieke regels via de uniq utility met de \-u (unique) vlag.  
  * Het combineren van meerdere commando's in een keten middels pipes (\|).

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 8 is het bestand data.txt aangetroffen. De doelstelling vereiste het isoleren van de enige regel tekst in dit bestand die uniek is en niet voorkomt in de rest van de dataset.  
2. **Oplossingsstrategie:** Om te zorgen dat dubbele regels direct naast elkaar komen te staan zodat ze gegroepeerd kunnen worden, is de inhoud van het bestand eerst gesorteerd. Vervolgens is het resultaat doorgestuurd naar het uniq commando, waarbij specifiek gefilterd is op unieke regels.  
3. **Uitvoering:** Het volgende commando is opgesteld en uitgevoerd:  
4. Bash

sort data.txt \| uniq \-u

5.   
6. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 9):** UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR  
* **Status:** Succesvol voltooid en gedocumenteerd.

