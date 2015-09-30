README: German/[English](README-English)
#Das Blutende Plakat

##Allgemein:
Das Blutende Plakat ist ein Plakat welches sich verändert, wenn in der Nähe SMS oder Telefonanrufe getätigt werden. Diese erhöten Strahlenwerte lösen aus, dass das Plakat zu bluten anfängt und dadurch ein Pictogramm Ablauf sichtbar wird.


++++ VIDEO ++++ Fehlt noch

++++ eventuell noch Video Funktionsablauf ++++

**1. Versuche Handystrahlung als Auslöser zu verwenden:**

- Anfangs hatte ich versucht mit kurzen Dipol Antennen die Handysignal(Elektromagnetische Wellen) aufzufangen und eine Kleine Spannung zu Induzieren. [Hier im Video ist das gut erklärt](http://www.ebay.de/itm/Flashlight-Handyanhanger-Spanien-Espana-Spain-Handyschmuck-Mobile-Phone-Charm-/261917061109?pt=LH_DefaultDomain_77&hash=item3cfb792ff5)  
(Imprinzip genau das was früher durch kleine Anhänger an Handys schon passiert ist. [Beispiel](http://www.ebay.de/itm/Flashlight-Handyanhanger-Spanien-Espana-Spain-Handyschmuck-Mobile-Phone-Charm-/261917061109?pt=LH_DefaultDomain_77&hash=item3cfb792ff5))  
- Durch intensiver suche bin ich dann auf ein Schaltung gestoßen welche genau dies mit Hilfe einer kleinen Verstärkerschaltung schaft.

!(Bilder der Verstärkerschaltung---Fehlt---)[]

**2. Induzierte Spannung soll Raspberry PI Pin HIGH schalten:**

- Dieses für mich gedanklich so einfache vorhaben wurde zur großen hürde. Kurzzeitig dachte ich es klappt. Aber schlussendlich hat dieses Vorhaben nie wirklich gut funktioniert und das Projekt ist mehr oder weniger daran gescheitert  


**3. Ideenfindung des Plakates und Umsetzung**

- Der Pictogramablauf soll durch das Blut sichtbar werden. Durch viele gespräeche mit Komilitonen kamm dann die Idee: eine Durchsichtige Folie mit weißem Aufdruck auf einer Weisen Platte anzubringen. Bei Auslösen des Plakatese sollte dann eine rote flüssigkeite die Weiße Platte kurzzeitig rot ferben und somit den Pictogramm ablauf sichtbar werden lassen. Mit Klebefolie für Fensterscheiben wurde die durchsichtigen Folie becklebt und dann mit Schrauben und Muttern (als abstandshalter) zusammen gefüght. 

!(Bild beklepte Folie und Platte---Fehlt---)[]

- nun hatte ich einen Zwischenraum in dem ich mit einer Pumpe, einem Schlauch und Auffangbehälter, das Rote Kunstblutbehälter immer wieder aufs neue fließen lassen konnte.

**4. Das Plakat bekommt einen Rahmen in dem alle Bauteile unterkommen:**

- Der Rahmen wurde aus einfachen Latten notdürfig zusammengeschraubt(das geht bestimmt mit entsprechenden Mitteln besser und Zeit besser) und alles dahinter verstaut. Oberhalb und Underhalb des Plakates ist der Rahmen größer um Technik und den Auffangbehälter zu befästigen.
- Die Flüssigkeit wurde dabei mit hilfe eines durchlöcherten Schlauches an die Oberekannte des Plakattes gepumpt.
- Der Raspberry pi und der Empfänger wurden ganz oben im Ramen verbaut, sodass diese Bauteile nicht nass werden können.

!(Bild Plakat Fertig von Hinten und Vorne ---Fehlt---)[]

###Benötigt:

[Raspberry Pi](https://www.tinkersoup.de/raspberry-pi/):

-	Raspberry Pi (Ich hatte einen Raspberry Pi 2 Modell B 1GB)
-	Micro SDHC Karte für Pi(für das Betriebsystem)  
-	USB Stromversorgung 5V (Handy Ladekabel bzw. Ladenetzteil)
-	Pi Cobbler (Adafruit Pi T-Cobbler Plus)
-	[Breadboard](http://www.exp-tech.de/komponenten-zubehoer/breadboards/breadboard-830-630-200) und [Jumper Wires](http://www.exp-tech.de/komponenten-zubehoer/kabel/75-pcs-breadboard-jumper-wires-with-m-m-connectors) 
-	HDMI Kabel (damit du auch deinen Pi direkt an Bildschirm anschliesen kannst und mit Maus und Tastatur ohne Umwege bedienen)  
-	Patchkabel (Empfehle aber Wifi Dongel. Damit kannst du dann auch ohne Kabel über deinen Laptop den Pi Bedienen)  



Empfänger und Verstärker:

-	[Cell Phone Signal Detector](https://www.seattleu.edu/scieng/ece/laboratory/cellphone/) (Das ne super ausführliche Anleitung dort findet ihr alles was man dafür benötigt.

Pumpe und Relais:

-	[Niedervolt-Tauchpumpe Barwig 0444 600 l/h 6 m](http://www.conrad.de/ce/de/product/539090/?gclid=CNnkzrqvkMgCFcFuGwod1a0L6Q&insert_kz=VQ&hk=SEM&WT.srch=1&WT.mc_id=google_pla&s_kwcid=AL!222!3!56269798017!!!g!!&ef_id=U5b7vwAABVnJvAd-:20150924190911:s)  
-	[Relais & Co ](http://www.glacialwanderer.com/hobbyrobotics/?p=9)(Damit kannst du die Pumpe Schalten. Die Anleitung ist fur Arduino funktionerit aber genausogut mit dem Pi)
-	Passender Schlauch für die Pumpe am besten direkt mit der Pumpe bei Conrad erfragen. (Durchlöchert habe ich die Pumpe dann mit einer Bormaschiene und Holzborer.

Plakat Rahmen und Auffangbehälter

-	Holzlatten (Baumarkt)
-	Luftabzugrohr (Mit Säge und Heißklebepistole zu behälter umgebauen)
-	Holzschrauben und Holzwinkel für den Rahmen
-	Gewindeschrauben mit Muttern und Beilagsschreiben



###Installation:

1. Am Besten Baut man den Cellephone detector als erstes und verbiendet diesen dann einen Pin des Pi(Bei mir ist das Projekt mehr oder weniger daran gescheitert).
3. Bekommt ihr das Signal des Cellephone detectors als HIGH auf euren PI, dann könnt ihr damit die Pumpe Schalten.  
(++++ Code fehlt noch +++++) 
4.	Nun müsst ihr das Piktogramm  
[Piktogramm - Schwarz](Pictures/Pictogram-black.ai)  
[Pictogramm - Weiß](Pictures/Pictogram-white.ai)  
![Piktogramme](Pictures/Pictogram.jpg) auf einem Plotter ausschneiden lassen und könnt damit die Durchsichtige Folie bekleben. (ACHTUNG SPIEGELVERKERT)
4. Verbindet die beklepte Folie mit Platte Dafür benötigt man die lange Gewindeschrauben mit der entsprechenden Anzahl an Muttern und Beilagsscheiben für den entsprechenden Abstand.  
(siehe Bild Allgemein 3. Ideenfindung des Plakates und Umsetzung)
5. Jetzt fehlt noch der Schlauch welchen ich mit einer Bohrmaschiene(Holzbohrer) an der entsprechenden Stelle durchbort hatte. Das ende wurde einfach umgeknickt.
![Bild durchborter und angebrachter Schlau](Pictures/Tube.jpg)
6. Den Auffangbehälter wurde aus einem Stück eckigem Dunstabzugs-Rohr gebaut(gedacht für einen Hert), welches ihr in einem Baumakrt findet. An dem Rohr wurde eine Seite abgesägt und damit die enden verklebt.
![Bild Auffangbehälter](Pictures/Rohr.jpg)
6. Nun alles zusammensetzten...


###Anwenden/Benutzen

- Pi Schaltung für die Cellephone detector und Pumpe  
(++++ Code fehlt noch +++++)


###Anmerkungen:
Die Verbindung zwischen Cellephone detector und Pi hat nicht wirklich klappt. Sollte dafür keine Lösung gefunden wurde ist es nicht zu empfehlen diese Plakat nachzubauen.

###Verwandte Arbeiten:
Inspiriert durch: [Blood in the Mobile](https://facebook.com/bloodinthemobile)

###Dank:
Dank geht an alle meine Kommilitonen des Eingabe Ausgabe Kurses des Sommersemester 2015. Gans besonders natürlich Fabiantheblind unseren JEDI Meister.

###Kontakt:
Falls etwas unklar ist und ihr Fragen habt schreibt mir einfach Johannes.Leick@gmx.de
Viel Spaß

##Public License
Copyright (C) 2015 Johannes Leick aka JohannesProximo Everyone is permitted to copy and distribute verbatim or modified copies of this license document, and changing it is allowed as long as the name is changed.
