README: German
#Das Blutende Plakat

##Allgemein:
Das Blutende Plakat ist ein Plakat welches sich verändert, wenn in der Nähe SMS oder Telefonanrufe getätigt werden. Diese erhöten Strahlenwerte lösen aus, dass das Plakat anfängt zu bluten und dadurch eine ein Pictogramm Ablauf sichtbar wird.


**1. Versuche Handystrahlung als Auslöser zu verwenden:**
	
> 1. Anfangs hatte ich mit kurzen Dipol Antennen Versucht das Signal aufzufangen und eine Kleine Spannung zu Induzieren. [Hier im Video ist das gut erklärt](http://www.ebay.de/itm/Flashlight-Handyanhanger-Spanien-Espana-Spain-Handyschmuck-Mobile-Phone-Charm-/261917061109?pt=LH_DefaultDomain_77&hash=item3cfb792ff5)  
> (Imprinzip genau das was früher durch kleine Anhänger an Handys schon passiert ist. [Beispiel](http://www.ebay.de/itm/Flashlight-Handyanhanger-Spanien-Espana-Spain-Handyschmuck-Mobile-Phone-Charm-/261917061109?pt=LH_DefaultDomain_77&hash=item3cfb792ff5))  
> 2. Durch intensiver suche bin ich dann auf ein Schaltung gestoßen welche genau dies mit Hilfe einer kleinen Verstärkerschaltung schaft.

(Bilder der gezeichneten Algorithmen)[]!

**2. Induzierte Spannung soll Raspberry PI Pin HIGH schalten:**

> 1. Dieses für mich gedanklich so einfache vorhaben wurde zur großen hürde. Kurzzeitig dachte ich es klappt. Aber schlussendlich hat dies nie wirklich gut funktioniert und das Projekt ist mehr oder weniger daran gescheitert  


**3. Ideenfindung des Plakates und Umsetzung**

> 1. Der Pictogramablauf soll durch das Blut sichtbar werden. Durch viele gespräeche mit Komilitonen kamm dann die Idee eine Durchsichtige Folie mit weisem aufdruck auf einer Weisen Platte zu versehen. Bei Auslösen des Plakatese sollte dann eine rote flüssigkeite die Weiße Platte kurzzeitig rot ferben und somit den Pictogramm ablauf sichtbar werden lassen. Mit Plotter dicken durchsichtigen folie schrauben und Muttern als abstandshalter einer Pumpe, Raspberry PI, Relais und viel Schweiß konnte ich diese Idee umsetzen und auch ein Auffangbehälter unten anbringen welches die Flüssigkeit wieder auffing.

**4. Das Plakat bekommt einen Rahmen in dem alle Bauteile unterkommen:**

> 1. Der Rahmen wurde aus einfachen Latten notdürfig zusammengeschraubt(das geht bestimmt mit entsprechenden Mitteln besser) und alles dahinter verstaut. Oberhalb und Underhalb des Plakates wurde der Rahmen größer um Technick und den Auffangbehälter dahinter zu verstecken.
> 2. Die Flüssigkeit wurde dabei mit hilfe eines durchlöcherten Schlauches an die Oberekannte des Plakattes gepumpt.
> 3. Der Raspberry pi und der Empfänger wurden ganz oben im Ramen verbaut, sodass diese Bauteile nicht nass werden können.

###Benötigt:

[Raspberry Pi](https://www.tinkersoup.de/raspberry-pi/):

-	Raspberry Pi (Ich hatte einen Raspberry Pi 2 Modell B 1GB)
-	Micro SDHC Karte für Pi(für das Betriebsystem)  
-	USB Stromversorgung 5V (Handy Ladekabel bzw. Ladenetzteil)
-	Pi Cobbler (Adafruit Pi T-Cobbler Plus)  
-	HDMI Kabel (damit du auch deinen Pi direkt an Bildschirm anschliesen kannst und mit Maus und Tastatur ohne Umwege bedienen)  
-	Patchkabel (Empfehle aber Wifi Dongel. Damit kannst du dann auch über deinen Laptop den Pi Bedienen)  

Empfänger und Verstärker:

-	[Cell Phone Signal Detector](https://www.seattleu.edu/scieng/ece/laboratory/cellphone/) (Das ne super ausführliche Anleitung dort findet ihr alles was man dafür benötigt.

Pumpe und Relais:

-	[Niedervolt-Tauchpumpe Barwig 0444 600 l/h 6 m](http://www.conrad.de/ce/de/product/539090/?gclid=CNnkzrqvkMgCFcFuGwod1a0L6Q&insert_kz=VQ&hk=SEM&WT.srch=1&WT.mc_id=google_pla&s_kwcid=AL!222!3!56269798017!!!g!!&ef_id=U5b7vwAABVnJvAd-:20150924190911:s)  
-	[Relais & Co ](http://www.glacialwanderer.com/hobbyrobotics/?p=9)(Damit kannst du die Pumpe Schalten. Die Anleitung ist fur Arduino funktionerit aber genausogut mit dem Pi)
-	Passender Schlauch für die Pumpe am besten direkt mit der Pumpe bei Conrad fragen

Plakat Rahmen und Auffangbehälter

-	Holzlatten (Baumarkt)
-	Luftabzugrohr (Mit Säge und Heißklebepistole zu behälter umbauen)
-	Holzschrauben und Holzwinkel
-	Gewindeschrauben mit Muttern und Beilagschreiben



###Installation:

1. Am Besten Baut man den Cellephone detector als erstes und verbiendet diesen dann mit dem Pi wenn ihr das hinbekommen habt(das hab ich nicht wirklich hinbekommen).
2. Nun kommt die Schaltung mit der Pumpe dran, diese soll durch ein den Pi geschaltet werden.
3. Bekommt ihr das Signal des Cellephone detectors als HIGH auf euren PI, dann könnt ihr damit ie Pumpe Schalten.
4.	Nun müsst ihr euer Piktogramme auf einem Plotter drucken lassen und konnt damit die Durchsichtige Folie bekleben. ACHTUNG SPIEGELVERKERT
4. Nun könnt ihr das Plakat Bauen dafür benötigt man die Zweite Platte durch lange schrauben und der entsprechenden Anzahl an Muttern könnt ihr dies dann verbinden.
5. Jetzt fehlt noch der Schlauch welchen ich mit einer Bohrmaschiene an der entsprechenden stelle durchbort hatte und am ende umgeknickt. Den Auffangbehälter hatte ich aus einem Baumarkt genommen.
6. Dann kann man alles zusammenbauen...


###Anwenden/Benutzen

- Pi Schaltung für die Cellephone detector und Pumpe

###Anmerkungen:
Da die Verbindung zwischen Cellephone detector und Pi nicht wirklich klappt, sollte man solange man dafür keine Lösung gefunden hat dies nicht nachbauen.

###Verwandte Arbeiten:
Blood in the Mobile

###Dank:
Dank geht an alle meine Kommilitonen des Eingabe Ausgabe Kurses des Sommersemester 2015. Gans besonders natürlich Fabiantheblind unseren JEDI Meister.

###Kontakt:
Falls etwas unklar ist und ihr Fragen habt schreibt mir einfach Johannes.Leick@gmx.de
Viel Spaß

##Public License
Copyright (C) 2015 Johannes Leick aka JohannesProximo Everyone is permitted to copy and distribute verbatim or modified copies of this license document, and changing it is allowed as long as the name is changed.
