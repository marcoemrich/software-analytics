# Big Data Meetup
Ort: Nürnberg, Hohfederstraße 40, Raum HQ.013  
Datum: Mittwoch, 07.03.2018  
Kurzlink zu dieser Seite: https://git.io/vALLM  
Meetup-Seite: https://www.meetup.com/de-DE/Nuernberg-Big-Data/events/247954125/

## Einleitung

Herzlich Willkommen auf der Begleitseite zum Big Data Meetup "Datenanalysen in der Softwareentwicklung mit Software Analytics"!

Hier findet ihr alle notwendigen Informationen, um im Mini-Workshop mitmachen zu können.

Gleich vorab: Wer sofort richtig loslegen möchte, kann sich gerne eine "lokale Umgebung" einrichten. Wer noch zögerlich ist, kann auch die Online-Testumgebung nutzen (welche aber vermutlich nicht so performant und zuverlässig sein wird).

## Hands-On 1: Git log Analyse

Hier geht es um den Einstieg in die Datenanalyse mit Python und Pandas mittels Daten aus dem Versionskontrollsystem Git. Wir wollen einige einfache Statistiken über ein Open-Source-Projekt erheben:

* In welcher Zeitzone leben die meisten Entwickler?
* Zu welchen Uhrzeiten arbeiten die Entwickler?
* An welchen Tagen wird am wenigsten Code committed?
* Wie verteilen sich die Commits über die Jahre?

Mit dem Ergebnis bekommen wir zahlreiche Einblicke in das Leben von Open-Source-Entwicklern.

### Einrichtung
#### Lokale Umgebung

Zur Offline-Nutzung auf dem eigenen Rechner kann die "Eierlegendewollmilchsau"-Python-Distribution Anaconda 5.0.1 (Version mit Python 3.6) installiert werden:

> https://www.anaconda.com/download/

Zum Starten 
* unter Windows die Verknüpfung "Jupyter Notebook" verwenden
* unter Linux den Befehl `~/anaconda3/bin/jupyter notebook` ausführen


#### Online-Testumgebung

Alternativ kann das Hands-On auch online mittels [https://mybinder.org/](mybinder.org) durchgeführt werden. Hier ist dann lediglich ein Laptop mit Browser und Internetzugang notwendig.

Zum Vorab-Test gibt es hier eine Online-Testumgebung:

> https://mybinder.org/v2/gh/feststelltaste/software-analytics/master?urlpath=tree%2Fcourses%2Fbig_data_meetup

Für das Meetup selbst wird es noch eine separate Online-Testumgebung geben.


### Dataset

Für beide Varianten ist hier die URL zum notwendigen Dataset (für Copy'n'Paste):

```
https://pastebin.com/raw/C40C9S82
```

_Zur Offline-Nutzung empfiehlt sich natürlich ein entsprechender Download vorab._

## Hands-On 2: Analyse wertloser Codeteile

Hier kombinieren wir das Datenanalysewerkzeug Pandas mit der Neo4j Graphdatenbank. Wir wollen in einer Java-Anwendung fachliche Module identifizieren, die

* nicht oder selten genutzt werden
* besonders viele Programmierfehler aufweisen

Mit dem Ergebnis können wir Wartungsarbeiten am bestehenden Softwaresystem nach den Geschäftszielen priorisieren.

### Einrichtung
#### Lokale Umgebung

Voraussetzung ist eine eingerichtete, lokale Umgebung vom 1. Hands-On. Zusätzlich wird noch folgendes benötigt:

##### Python-Neo4j-Adapter `py2neo`
Diese Bibliothek kann z. B über den "Anaconda Prompt" mit Hilfe des Python-Paketmanagers `pip` installiert werden:

```
pip install py2neo
```

##### Demo-Applikation "Spring Petclinic"
Dieses Open-Source-Projekt ist eine mit jQAssistant ausgestattete (und von mir bewusst verschlechterten) Java-Web-Applikation. Sie ist unter

> https://github.com/JavaOnAutobahn/spring-petclinic

zu finden. Die dortige Anleitung schildert die Installationsschritte:

> https://github.com/JavaOnAutobahn/spring-petclinic#refuctored-spring-petclinic-sample-application

_Zur Offline-Nutzung empfiehlt es sich, die Anwendung wie in der Anleitung beschrieben komplett zu bauen und auszuführen._

#### Online-Testumgebung

Zum Meetup wird eine gesonderte Neo4j-Instanz zur Verfügung stehen. Weitere Details zur Nutzung folgen beim Treffen.

### Dataset

Für beide Varianten ist hier die URL zu dem notwendigen Dataset (für Copy'n'Paste):

```
https://pastebin.com/raw/HdgNTGKX
```

_Zur Offline-Nutzung empfiehlt sich natürlich ein entsprechender Download vorab._



## Schlussbemerkung

Wer an den Themen Gefallen gefunden hat, findet auf meinem Blog https://www.feststelltaste.de noch zahlreiche andere Anwendungsfälle. Über ein Feedback zur Veranstaltung auf der Meetup-Seite oder per [Mail](mailto:meetup@markusharrer.de) freue ich mich sehr!  

  
Markus Harrer  
[@feststelltaste](https://www.twitter.com/feststelltaste)  
[markusharrer.de](http://www.markusharrer.de) 
