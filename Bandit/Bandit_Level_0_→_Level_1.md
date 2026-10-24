# **Lab Report: OverTheWire \- Bandit Level 0 → Level 1**

* **Datum:** 24 oktober 2026  
* **Doel:** Verbinding maken met een externe Linux-omgeving via SSH, navigeren door mappen en bestandsinhoud extraheren met basiscommando's.  
* **Geteste CompTIA Linux+ Concepten:**  
  * Externe authenticatie en Secure Shell (SSH) protocollen.  
  * Bestandsstructuur en permissie-inspectie (ls, ls \-la).  
  * Standaard bestandslezen (cat).  
  * Text-filtering en pipelining (grep).

### **1\. Uitgevoerde Stappen & Commando's**

1. **Authenticatie en Verbinding:** Er is verbinding gemaakt met de OverTheWire trainingsserver via SSH op poort 2220 met de gebruikersnaam bandit0:  
   Bash  
   ssh bandit0@bandit.labs.overthewire.org \-p 2220

2. **Reconnaissance & Analyse:** Na succesvolle inlog is de mapstructuur geanalyseerd. Met het commando ls \-la zijn zowel normale als verborgen bestanden en hun toegangsrechten bekeken:  
   Bash  
   ls \-la

   *Uitkomst:* Het bestand readme was zichtbaar met leesrechten voor de gebruiker.  
3. **Informatie-extractie:** De inhoud van het bestand readme is uitgelezen en gefilterd met behulp van een pipe (\|) en grep om direct het wachtwoord voor de volgende ronde te isoleren:  
   Bash  
   cat readme \| grep "The password you are looking for is:"

### **2\. Resultaat & Bewijs**

* **Verworven Credential (Level 1):** 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR  
* **Status:** Succesvol afgerond en gedocumenteerd.

Klaar voor de volgende uitdaging? Pak je terminal erbij, log uit met exit en log in op **Level 1** met:

Bash  
ssh bandit1@bandit.labs.overthewire.org \-p 2220

*(En vergeet niet de valstrik uit het vorige level te omzeilen als je daar het bestand met de naam \- tegenkomt: gebruik cat ./-\!)* Laat maar weten als je de vlag te pakken hebt\!