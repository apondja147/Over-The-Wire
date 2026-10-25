# **Lab Report: OverTheWire \- Bandit Level 6 tot Level 7**

* **Datum:** 25 oktober 2026  
* **Doel:** Het overkoepelend zoeken naar een bestand over de gehele server op basis van specifieke eigenschappen zoals eigenaar, groep en byte-grootte.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het recursief zoeken over het volledige bestandssysteem vanaf de root (/).  
  * Het filteren op bestandsrechten, eigenaars (\-user) en groepstoewijzingen (\-group).  
  * Het onderdrukken van onbevoegde foutmeldingen via standard error redirect (2\>/dev/null).

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** De doelstelling voor Level 6 vereiste het lokaliseren van een bestand ergens op de server dat eigendom is van gebruiker bandit7 en groep bandit6, met een exacte grootte van 33 bytes.  
2. **Oplossingsstrategie:** Omdat de locatie van het bestand onbekend was, is de find utility losgelaten op de absolute root (/). Om te voorkomen dat de uitvoer overspoeld raakte met Permission denied meldingen van systemen en mappen waar de gebruiker geen rechten toe heeft, zijn de foutmeldingen omgeleid naar de digitale vuilnisbak (2\>/dev/null).  
3. **Uitvoering:** Het volgende commando is uitgevoerd:  
4. Bash

find / \-user bandit7 \-group bandit6 \-size 33c 2\>/dev/null

5.   
6. Dit leverde direct het pad /var/lib/dpkg/info/bandit7.password op. Het bestand is vervolgens uitgelezen met:  
7. Bash

cat /var/lib/dpkg/info/bandit7.password

8.   
9. 

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 7):** Bmnvf82KzQlfXgAI2dlzYbrlu9r3E3  
* **Status:** Succesvol voltooid en gedocumenteerd

