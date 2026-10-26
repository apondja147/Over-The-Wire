# **Lab Report: OverTheWire \- Bandit Level 10 tot Level 11**

* **Datum:** 26 oktober 2026  
* **Doel:** Het decoderen van base64-gecodeerde gegevens in een tekstbestand om het volgende wachtwoord te achterhalen.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Het identificeren en decoderen van base64-formaten via de `base64` utility.  
  * Het toepassen van de decodeer-vlag (`-d` of `--decode`).  
  * Het verwerken van bestandsstromen binnen de command-line interface.

### **1\. Uitgevoerde Stappen en Analyse**

1. **Reconnaissance:** Na inloggen op Bandit Level 10 is het bestand `data.txt` aangetroffen, dat volgens de specificaties base64-gecodeerde data bevatte.  
2. **Oplossingsstrategie:** Om de gecodeerde tekst leesbaar te maken, is de `base64` utility ingezet in combinatie met de decodeer-optie om de datastroom terug te vertalen naar platte tekst.  
3. **Uitvoering:** Het volgende commando is zelfstandig opgesteld en uitgevoerd:

Bash  
base64 \-d data.txt

### **2\. Resultaat en Bewijs**

* **Verworven Wachtwoord (Level 11):** `pyF0Y6HwUsDj5rL9UvyhU7MCmv8VN5Ro`  
* **Status:** Succesvol voltooid en gedocumenteerd.

