# Gramps Web

### Open-Source-Genealogie im Netz

David Straub

7. Dezember 2023

Ahnenforscher-Stammtisch Unna (Zoom)




Gramps Desktop <-> Gramps Web

<div >
<img style="vertical-align: middle;" width="45%" src="images/gramps-screenshot.png">
<img style="vertical-align: middle;"  width="40%" src="images/grampsweb-screenshot.png">
</div>



## Über mich

- Aus Wendlingen am Neckar, jetzt München
- Ahnenforschung als Hobby seit der Schulzeit
- Gramps-Desktop-Nutzer seit ca. 15 Jahren
- Python-Entwickler seit 8 Jahren
- Erster Prototyp einer Gramps Web-App vor 4 Jahren
- Beruf: Physiker, Data Scientist



## Plan

- Motivation
- Kurzer Blick auf Gramps Desktop
- Gramps Web: Idee, Aufbau
- Ausführliche Tour durch Gramps Web
- Installationsoptionen
- Links



## Wozu ein Genealogie-System?

- Stammbdaum-Datenbank und -Visualisierung
- Vollständig digitalisierte und verknüpfte Quellen und Medien
- Vollständig digitale und verknüpfte Notizen


## Die Daten im Genealogiesystem sind das Vermächtnis des Ahnenforschers!


## Warum Open Source?

- Unser Vermächtnis soll auf genealogischen Zeitskalen zugänglich bleiben -> offene Formate, offene Datenstrukturen
- Unabhängigkeit von strategischen/wirtschaftlichen Entscheidungen einzelner Unternehmen (z.B. Causa FTM)



## Gramps Desktop: Fakten

- Seit 2004
- Frei & Open Source (GPL)
- Aktive internationale Entwicklergemeinde
- In über 40 Sprachen übersetzt
- Plattformübergreifend (Linux, Windows, Mac)
- In Python programmiert
- Offene Standards (XML, SQLite)
- GEDCOM-Import/Export


## Gramps Desktop: Demo



## Warum Gramps Web?

- Forschungsergebnisse in der Verwandtschaft kommunizieren?
- Zusammenarbeiten?
- Unterwegs auf Handy oder Tablet arbeiten?


## Gramps Web: Anforderungen

- Vollständiger Zugang zu allen Daten im Genealogiesystem
- Blogfunktion
- Kompatibel & synchronisierbar mit Gramps Desktop
- Einfacher Export
- Nur für ausgewählte Benutzer zugänglich
- Für manche Nutzer manche Daten unsichtbar machen
- Gemeinsames Bearbeiten
- Handy-/Tablet-freundlich


## Gramps Web: Architektur

![](images/Architektur.svg)


## Was Gramps Web *nicht* ist

- Keine eigene Datenquellen (Familysearch, Ancestry, MyHeritage, ...)
- Kein Abgleich mit Datenbanken anderer Nutzer
- Keine öffentliche Genealogie-Webseite (siehe Gramps-Addons)


## Gramps Web: Demo



## Sicherheit und Datenschutz

- Zugang ohne Account grundsätzlich nicht vorgesehen
- Abgestufte Berechtigungen
    - bearbeiten, hinzufügen, betrachten, betrachten außer "vertraulich markiert"
- Berechtigungen werden von Gramps auf Datenbank-Zugriffs-Ebene erzwungen
    - stark reduzierte Wahrscheinlichkeit von Datenlecks durch Bugs




## Installation

- Architektur erlaubt Features, die man sonst nur vom Desktop kennt (PDF-Berichte, Gesichtsdetektion, Texterkennung)
    - höhere Installationsanforderungen (als z.B. Webtrees)
- Drei Optionen:
    - Eigener Server (Raspberry Pi, virtueller Server o.ä.)
    - Docker-Hosting (z.B. Gramps Web DigitalOcean-App)
    - Vollständig gehosteter Dienst (Grampshub)



## Grampshub

- Hosting-Dienst für Gramps Web
- Seit Mitte 2023 von mir betrieben
- Abo-Modell (aber keine Abo-Falle)

![](images/grampshub-abos.png)


## Grampshub: Vorteile

- Keine Installation nötig
- Keine Serverkonfiguration nötig
- Automatische Updates
- Unterstützung des Gramps-Web-Hauptentwicklers&nbsp;🙂

Und wie überall bei Gramps Web: kein Provider-Lock-In &ndash; Vollständiger Export/Import _aller_ Daten mit 3 Klicks


## Grampshub: Nachteile

- Kein Befehlszeilen-Zugang auf den Server
    - Lokale Bearbeitung dank Sync-Addon möglich
- Begrenzte Personenzahl im Baum
    - Umzug zu anderem Server jederzeit möglich
- Keine eigene Domain (familieXYZ.de)



## Mehr Info

- Gramps Web Docs: https://www.grampsweb.org
    - Deutsch [via Google Translate](https://translate.google.com)
- Grampshub: https://www.grampshub.com
- Mein Blog: https://www.grampshub.com/blog
- Instagram: https://www.instagram.com/grampshub/


## Hilfe finden

- Compgen-Liste `gramps-l` (deutsch): https://discourse.genealogy.net/c/gramps-l/
- Gramps-Forum (englisch): https://gramps.discourse.group/c/gramps-web/
- Fehler melden:
    - Unterbau/Verarbeitung: https://github.com/gramps-project/gramps-webapi/issues
    - Benutzeroberfläche/Darstellung: https://github.com/gramps-project/Gramps.js/issues
