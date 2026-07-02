# Nutzungshinweise Zeugnisformulare Berufskollegs nach APO-BK

## Allgemeine Hinweise

### Lernfelder
Bei Zeugnissen mit Lernfeldern muss in SchILD unter *Fachklassen* im Feld *Lernfelder* eine rtf-Datei eingefügt (oder der Inhalt getippt) werden. Dieser Text erscheint genau so auf der Anlage bzw. (bei A3-Zeugnissen) auf der 
Zeugnisrückseite auf Seite 4.\
Gleichzeitig wird (wenn es einen Lernfeldeintrag dort gibt) eine entsprechende Fußnote mit Verweis auf die Anlage gesetzt.

### Reiter "BK-Abschluss"
Für alle Abschlusszeugnisse muss der Reiter „BK-Abschluss“ in SchILD verwendet werden. Die Noten werden von dort in die Reports übernommen.  
Die Durchschnittsnote des Abschlusses wird hier berechnet und kann dann auf dem Abschlusszeugnis ausgewiesen werden.

### Erworbene Abschlüsse
Erworbene Abschlüsse müssen auch auf dem Reiter *Akt. Halbjahr* im aktuellen Abschnitt eingetragen sein. In den meisten Fällen werden die erworbenen Abschlüsse durch den Berechnungsalgorithmus automatisch gesetzt.

### Fachbereich, Fachrichtung, Schwerpunkt, Berufsfeld
Im Katalog Fachklassen werden auch Fachbereich, Fachrichtung, Schwerpunkt und Berufsfeld eingetragen.\
Berufsebene 1: Fachbereich\
Berufsebene 2: Fachrichtung bzw. Berufsfeld\
Berufsebene 3: Schwerpunkt der Fachklasse\
Die dortigen Eintragungen werden auf die Zeugnisse übernommen.

### Fehlzeiten
Fehlzeiten werden auf den Reiter *Akt. Halbjahr* in Stunden erfasst und auf Halbjahres- und Jahreszeugnissen ausgewiesen.  

### Praktumszeiten
Die Praktikumszeit wird einmal pro Aufruf abgefragt und ist in der vorgegebenen Form (inklusive Angabe von Wochen oder „Tage pro Woche“) anzugeben. 
Wird kein Praktikum absolviert, ist „0“ einzutragen (damit kein Eintrag auf dem Zeugnis erfolgt).  
Die Praktikumszeit kann auch als Vermerk mit der Vermerkart *Praktikumsdauer* und einem Datum, das im entsprechenden Zeitabschnitt liegt, eintragen werden. 
Wird ein passender Eintrag gefunden, überschreibt dieser die Eingabe beim Aufruf.  
Beispiel für einen Vermerkeintrag:  
- 3 Tage pro Woche
- 5 Wochen

### Sprachniveaus
Die Ausgabe der Sprachniveaus auf AGZ und ASZ erfolgt durch Eintrag bei der Sprachenfolge unter Laufbahninfo.

### Zeugniskopf
Die rtm-Datei mit dem Schulkopf muss im Ordner *Subreports* zu finden sein.  
In Abschlusszeugnissen ist als festes Bild das Wappen des Landes NRW eingebaut. Dieses sollte durch das Wappen des Schulträgers ersetzt werden.

### Zeugnisbemerkungen
Für die Zeugnisbemerkungen werden die üblichen Platzhalter durch die 
[ReplaceDefault-Funktion](https://schulverwaltungsinfos.nrw.de/svws/wiki/index.php?title=ReplaceDefault) 
ersetzt.  
Zusätzlich werden im Text geschlechtsspezifische Umwandlungen nach dem Muster der Bemerkungsfelder vorgenommen, d.h. aus &Text_männlich%Text_weiblich& wird in Abhängigkeit vom Geschlecht des Schülerdatensatzes die korrekte Form gewählt.

### Zeugnisunterschriften
Die Zeugnisse werden von der eingetragenen Abteilungsleitung unterschrieben. Sollte diese auch gleichzeitig die Klassenleitung sein, unterschreibt die stellvertretende Schulleitung.
Abgangszeugnisse (AGZ) und Abschlusszeugnisse (ASZ) werden von der Schulleitung unterschrieben.

### Optionale Angaben
Bei einigen Zeugnissen kann optional eine Aussage zu Schuljahr, Klasse und Jahrgang eingeblendet werden. 
Hierfür im *Detail.BeforePrint* an der markierten Stelle „ja“ eintragen.  

### Versionierung
Die Reports aller Anlagen enthalten im Namen eine Versionsnummer, um Änderungen nachvollziehen zu können. 

## Hinweise Anlage A

### Berufsschule (A01 - A04)

|Anlage|Report|
| :--- | :--- |
|Anlage A1.5: Zeugnis der Berufsschule|HJZ-20xx.x- BS(Anl A1.5).rtm <br> JAZ-20xx.x- BS(Anl A1.5).rtm|
|Anlage A1.6: Abschlusszeugnis der Berufsschule <br> Anlage 1.8: Abschlusszeugnis der Berufsschule mit MSA |ASZ-20xx.x- BS(A1.6+A1.8).rtm|
|Anlage A1.7: Abgangszeugnis der Berufsschule|AGZ-20xx.x- BS(Anl A1.7).rtm <br> ÜWZ-20xx.x- BS(Anl A1.7).rtm|
|Anlage A1.9: Abschlusszeugnis der Berufschule mit FHR|ASZ-20xx.x- mit FHR BS(A1.9).rtm|
|Anlage A1.10: Nichtzulassung zur FHR-Prüfung|Nichtzulassung FHR 20xx.x (Anl A1.10).rtm|
|Anlage A1.11: Nichtbestehen der FHR-Prüfung|Nichtbestehen FHR 20xx.x (Anl A1.11) ohne Auswahl.rtm <br> Nichtbestehen FHR 20xx.x (Anl A1.11).rtm|

#### Gewichtung der Fächer
Die Gewichtung der Fächer wird im Katalog *Fächer* bei jedem Unterrichtsfach unter *Sonstige Einstellungen* eingetragen.

#### Durchschnittsnoten
Die Durchschnittsnote für den Berufsschulabschluss wird automatisch auf *BK-Abschluss* berechnet, dabei werden die eingetragen Gewichtungen der Fächer berücksichtigt.  
Die Durchschnittsnote für die FHR wird ebenfalls auf *BK-Abschluss* berechnet (A02). 
Hierbei dürfen Sport und Relgion nicht berücksichtigt werden, diese Gewichtung muss entsprechend gliederungsbezogen bei den Fächern mit 0 bei Gewichtung allgemeinbildend eingetragen werden.
 
#### DQR-Niveau
Das DQR-Niveau des erreichten Abschlusses für die Berufsschule muss unter „Fachklassen“ eingetragen sein.

#### Anforderungen erfüllt/nicht erfüllt
In die Entscheidung *Anforderungen erfüllt/nicht erfüllt* werden die 5en und 6en eingezogen. Bei mindestens 2 mal 5 oder mindestens 1 mal 6 wird **anforderungen nicht erfüllt** ausgegeben. 
Die Fächer im Differenzierungsbereich werden nur mitgezählt, wenn die allgemeinbildende Gewichtung 1 ist (z.B. Mathematik für die FHR in A02).
Der Versetzungsvermerk wird bei der Berechnung der Versetzung automatisch gesetzt, kann aber manuell abgeändert werden:
* versetzt
* versetzt, Anforderungen nicht erfüllt

### Ausbildungsvorbereitung, Internationale Förderklassen

|Anlage/Hinweise|Report|
| :--- | :--- |
|Anlage A2.3: Zeugnisse der Ausbildungsvorbereitung (auch IFK)|HJZ-20xx.x-AV (Anl A2.3).rtm <br> ASZ-20xx.x-AV (Anl. 2.3).rtm <br> JAZ-20xx.x-AV (Anl A2.3).rtm <br>ÜWZ-20xx.x-AV (Anl A2.3).rtm <br> AGZ-20xx.x-AV (Anl A2.3).rtm|
|Anlage A2.4: Berechtigung zum Besuch des weiterführenden Bildungsganges|Bescheinigung 20xx.x Anl A2.4.rtm|
|Bescheinigung Vorklasse "Fit für mehr" |Bescheinigung FFM 20xx.x.rtm|
|Textzeugnisse für Schülerinnen und Schüler mit Förderschwerpunkt in der AV|Textzeugnis AGZ-20xx.x-AV (Anl A2.3).rtm <br> Textzeugnis HJZ-20xx.x-AV (Anl A2.3).rtm <br> Textzeugnis JAZ-20xx.x-AV (Anl A2.3).rtm|

#### Hinweis Schulpflicht in der Sekundarstufe II gemäß §38 Abs. 4 Schulgesetz NRW
Eine vorzeitige Erfüllung der Schulpflicht der SII (§38 Abs. 4 SchulG) wird auf Abgangszeugnissen vermerkt, wenn der Haken bei *Berufsschulpflicht erfüllt* auf *Individualdaten I* gesetzt ist. 


#### Internationale Förderklasse
In diesen Fachklassen wird Berufsebene 1 "Internationale Förderklasse" eingetragen. Berufsebene 2 und Berufsebene 3 bleiben leer.  
Für die Ausstellung der *Berechtigung zum Besuch des weitereführenden Bildungsganges* für IFK-Lernende wird bei jedem aufgerufenen Datensatz abgefragt, für welchen Bildungsgang die Berechtigung ausgestellt werden soll.

#### Bescheiniung "Fit für Mehr"
Die Lernenden erhalten eine Bescheinigung über den Besuch der Vorklasse "Fit für Mehr" zur Internationalen Förderklasse.  
Auf der Bescheinigung werden alle erteilten Fächer ohne Noten aufgelistet. Die Fächer müssen im *Akt. Halbjahr* unter *Leistungsdaten* zugewiesen sein.

#### Textzeugnisse
Für Lernende mit Förderschwerpunkt können Textzeugnisse erstellt werden.  
Die Texte je Fach werden als *Fachbezogene Leistungsentwicklung* bei den Leistungsdaten erfasst.


## Hinweise Anlage B
-	Zeugnisse nach Anlage B4: einjährige Bildungsgänge
-	Zeugnisse nach Anlage B5 bis B7: zweijährige Bildungsgänge

|Anlage/Hinweise|Report|
| :--- | :--- |
|Anlage B4: <br> Zeugnis der Berufsfachschule mit dem Nachweis <br> der beruflichen Kenntnis, Fähigkeiten, Fertigkeiten|HJZ-20xx.x-BFS (Anl B4).rtm <br>ASZ-20xx.x-BFS (Anl B4).rtm <br> JAZ-20xx.x-BFS (Anl B4).rtm <br> AGZ-20xx.x-BFS (Anl B4).rtm <br> ÜWZ-20xx.x-BFS (Anl B4).rtm |
|Anlage B5: <br> Zeugnis der Berufsfachschule mit einer <br> staatlich zu prüfenden Berufsausbildung|HJZ-20xx.x-2jBFS (Anl B5).rtm <br> JAZ-20xx.x-2jBFS (Anl B5).rtm <br> AGZ-20xx.x-2jBFS (Anl B5).rtm <br> ÜWZ-20xx.x-2jBFS (Anl B5).rtm|
|Anlage B6: <br> Abschlusszeugnis der Berufsfachschule|ASZ-20xx.x-2jBFS (Anl B6).rtm|
|Anlage B7:  <br> Berufsabschlusszeugnis der Berufsfachschule|ASZ-20xx.x-2jBFS (Anl B7) Kinderpflege.rtm <br> ASZ-20xx.x-2jBFS (Anl B7).rtm <br> ASZ-20xx.x-Externe (Anl B7).rtm|
|Anlage B8:  <br> Bescheinigung für den Antrag <br> Verkürzung der Ausbildung zur/zum <br> Pflegefachfrau/-mann|Bescheinigung Altenpflege 20xx.x (Anl B8).rtm|
|Anlage B9:  <br> Nichtbestehen der Berufsabschlussprüfung |Nichtbestehen BAB 20xx.x (Anl B9) ohne Auswahl.rtm <br> Nichtbestehen BAB 20xx.x (Anl B9).rtm|
|Anlage B10:  <br> Zertifikat Betreuungskraft nach § 43b SGB XI|Zertifikat Betreuungskraft 20xx.x (Anl B10).rtm|
|Anlage B11:  <br> Nichtzulassung zur Berufsabschlussprüfung|Nichtzulassung BAB 20xx.x (Anl B11).rtm|


#### Hinweis Schulpflicht in der Sekundarstufe II gemäß §38 Abs. 4 Schulgesetz NRW
Eine vorzeitige Erfüllung der Schulpflicht der SII (§38 Abs. 4 SchulG) wird auf Abgangszeugnissen vermerkt, wenn der Haken bei *Berufsschulpflicht erfüllt* auf *Individualdaten I* gesetzt ist. 

#### Berufsbezeichnung
Für die Formulare der 2-jährigen Berufsfachschule mit Berufsabschluss muss in der Fachklassentabelle die Berufsbezeichnung mit dem Zusatz „Staatlich geprüfter“ (männliche und weibliche Form) eingetragen sein.  
Diese ist Bestandteil der Bildungsgangsbezeichnung.

#### Abschlussarbeiten
Für die Abschlussarbeiten werden eigene Fächer angelegt (z.B. AA1, AA2) und der Fächergruppe *Abschlussarbeit* zugeordnet.
Die Themen der Arbeiten werden als *Fachbezogene Leistungsentwicklung (Memo)* erfasst.  
Die Eintragung kann auch über den Gruppenprozess *Details zu Fächern bei Schülern ändern" erfolgen.

#### Fachpraktische Anteile
Nicht ausreichende Leistungen in den praktischen Anteilen der Bereichsspezifischen Fächern müssen durch eine Fußnote gekennzeichnet werden.  
Die Fussnote wird gedruckt, wenn der Eintrag *Fachpraktische Anteile ausreichend* im *Akt. Halbjahr* Bereich *Allgemeine Angaben II* auf NEIN steht.

 
## Hinweise Anlage C

|Anlage/Formulare|Report| C1: Ass. + FHR|C2: Ass. |C3: schul. Teil FHR|FOS11/ <br> FOS12|FOS12B|
|:--- |:---|:---:|:---:|:---:|:---:|:---:|
|Anlage C5: <br> Abgangszeugnis|AGZ-20xx.x-Anl C (Anl C5).rtm <br> ÜWZ-20xx.x-Anl C (Anl C5).rtm|x|x|x|x|x|
|Anlage C6: <br> Halbjahres-, Versetzung- <br> und Jahreszeugnis|HJZ-20xx.x-Anl C(Anl C6).rtm <br> JAZ-20xx.x-Anl C(Anl C6).rtm|x|x|x|x|x|
|Anlage C7: <br> Zeugnis Fachhochschulreife <br> schulischer Teil|ASZ-20xx.x-Anl C FHR-Ass. und HBFS (Anl C7 und C8).rtm|x||x|||
|Anlage C8: <br> Fachhochschulreifezeugnis <br> Assistentinnen/Assistenten| siehe C7|x|||||
|Anlage C9: <br> Berufsabschlusszeugnis|ASZ-20xx.x-Anl C BAB-Assistenten (Anl C9).rtm|x|x|||||
|Anlage C10: <br> Fachhochschulreifezeugnis <br> der Fachoberschule|ASZ-20xx.x-Anl C FHR- FOS (Anl C10).rtm||||x|x|
|Anlage C11: <br> Nichtzulassung FHR|Nichtzulassung FHR 20xx.x (Anl C11) ohne Auswahl.rtm <br> Nichtzulassung FHR 20xx.x (Anl C11).rtm|x||x|x|x|
|Anlage C12: <br> Nichtbestehen FHR|Nichtbestehen FHR 20xx.x (Anl C12) ohne Auswahl.rtm <br> Nichtbestehen FHR 20xx.x (Anl C12).rtm|x||x|x|x|
|Anlage C13: <br> Nichtzulassung BAP|Nichtzulassung BAB 20xx.x (Anl C13) ohne Auswahl.rtm <br> Nichtzulassung BAB 20xx.x (Anl C13).rtm|x|x||||
|Anlage C14: <br> Nichbestehen BAP|Nichtbestehen BAB 20xx.x (Anl C14) ohne Auswahl.rtm <br> Nichtbestehen BAB 20xx.x (Anl C14).rtm|x|x||||
|Prüfungsliste|Pruefungsliste.rtm||||||
|Zulassungsbescheinigung FHR|Zulassung FHR 20xx.x.rtm||||||

#### Nichtzulassung/Nichtbestehen mit und ohne Auswahl
Die nicht ausreichenden Fächer werden automatisch aufgeführt.
- **mit Auswahl**: 
	* Es wird individuell abgefragt, ob eine Wiederholung möglich ist oder nicht.
	* Analog erfolgt beim Nichtbestehen eine Abfrage der Möglichkeit der Nachprüfung und der entsprechende Hinweis auf der Mitteilung.
- **ohne Auswahl**:
	* Lernende, die den aktuellen Lernabschnitt wiederholen (Haken bei Akt. Halbj.), bekommen automatisch den Hinweis auf das Überschreiten der Höchstverweildauer, die anderen den Hinweis auf die Möglichkeit der Wiederholung.
	* Bei C12 und C14 erfolgt ein Hinweis auf eine mögliche Nachprüfung, wenn entweder zweimal eine 5 vorhanden ist, oder im aktuellen Halbjahr ein Versetzungsvermerk „Nachprüfung möglich“ gesetzt wurde.
	* Für Fälle, die davon abweichen, müssen die Reports mit Auswahl verwendet werden.



## Hinweise Anlage D
siehe AnleitungBK-Zeugnisse-AnlD.pdf

## Hinweise Anlage E

Fachbereiche:  
A - Agrarwirtschaft  
G - Gestaltung  
E - Ernährung und Versorgungsmanagement  
I - Informatik  
S - Sozialwesen  
T - Technik  
W - Wirtschaft  


|Fachbereich| S | S |A, E, I, T, W|S|A|E|S|W|alle|
|:--- |:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|**Stunden**| 3.600 | 3.600 |2.400|1.800|1.200|1.200|1.200|1.200|600|
|**Fachrichtung**| Sozial-pädagogik | Heil-erziehungs-pflege|alle|Heil-pädagogik|Gartenbau, Land-wirtschaft|Groß-haushalt|Moto-pädie|Möbel-handel|Aufbau-bildungs-gänge|
|Abgangs-zeugnis| E6-1 | E6-2 |E6-3|E6-4|E6-5|E6-5|E6-6|E6-7|E6-8|
|Versetzungs-zeugnis| E4a-1 | E4a-2 |E4a-3|E4a-4||||||
|Versetzungs-zeugnis, Zulassung zum Praktikum| E5b-1 | E5b-2 ||||||||
|Zeugnisanlage mit Ergebnissen zu den Arbeiten| E5bz-1 | E5bz-2 ||||||||
|Nichtzulassung zum FS-Examen| E4b-1 | E4b-2 |E4b-3|E4b-4||||||
|Zulassung zum FS-Examen| E5c-1 | E5c-2 ||||||||
|Mitteilung Nichtzulassung| E4c-1 | E4c-2 |E4c-3|||||||
|Abschluss-zeugnis ohne FHR| E5-1 | E5-2 |E5-3|E5-4|E5-5|E5-5|E5-6|E5-7|E5-8|
|Abschluss-zeugnis mit FHR| E7-1 | E7-2 |E7-3|||||||
|Externen-prüfungs-zeugnis| E8-1 | E8-2 |E8-3|E8-4|E8-5|E8-5||||
|Zulassung Berufspraxis Externe| E8b-1 | E8b-2 ||||||||


#### Zeugnisreports
- AGZ-20xx.x-FS(Anl E6-1,2,3,4,5,6,7).rtm	
- AGZ-20xx.x-FS(Anl E6-8) Aufbaubildungsgang.rtm
- ASZ-20xx.x-FS Extern(Anl E8-3,4,5).rtm
- ASZ-20xx.x-FS Sozialwesen (Anl E5-1,2 und E7-1,2) mit und ohne FHR.rtm
- ASZ-20xx.x-FS Sozialwesen Extern(Anl E8-1,2).rtm
- ASZ-20xx.x-FS(Anl E5-3,4,5,6,7 und E7-3) mit und ohne FHR.rtm
- ASZ-20xx.x-FS(Anl E5-8) Aufbaubildungsgänge.rtm
- HJZ-20xx.x-FS (für Vollzeit).rtm
- JAZ-20xx.x-FS(Anl E4a) mit Versetzungsvermerk.rtm
- JAZ-20xx.x-FS(Anl E4b) Nichtzulassung Examen.rtm
- JAZ-20xx.x-FS(Anl E5c) Zulassung Examen.rtm
- Mitteilung Nichtzulassung 20xx.x- Fachschule (Anl E4c-3).rtm	
- Mitteilung Nichtzulassung 20xx.x- Fachschule Sozialwesen (Anl E4c-1,2).rtm
- Z-20xx.x-FS Sozialwesen Extern nach Theorieprüfung (Anl E8b-1,2).rtm
- Zeugnisanlage Sozialwesen 20xx.x (E5bz-1,2).rtm



#### Berufsbezeichnung
In der Fachklassentabelle muss die Berufsbezeichnung mit dem Zusatz „Staatlich geprüfter“ (männliche und weibliche Form) eingetragen sein.  
Diese ist Bestandteil der Bildungsgangsbezeichnung.

#### Abschlussarbeiten
Für die Abschlussarbeiten werden eigene Fächer angelegt (z.B. AA1, AA2, AA3) und der Fächergruppe *Abschlussarbeit* zugeordnet.
Die Themen der Arbeiten werden als *Fachbezogene Bemerkung (Memo)* erfasst.  
Die Eintragung kann auch über den Gruppenprozess *Details zu Fächern bei Schülern ändern" erfolgen.

#### Projektarbeit
Für die Projektarbeit wird ebenfalls ein eigenes Fach angelegt, das der Fächergruppe *Projektarbeit* zugeordnet wird. 
Das genaue Thema wird auch hier als *Fachbezogene Bemerkung* eingetragen.

#### Fachschule Sozialwesen
- In der Fachrichtung Sozialpädagogik werden die *Wahlfächer* der Fächergruppe *Wahlpflichtbereich* zugeordnet.
- Die Ergebnisse der Abschlussarbeiten am Ende des theoretischen Ausbildungsteils können durch die *Zeugnisanlage Sozialwesen* ausgewiesen werden. 
