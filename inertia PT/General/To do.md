# proposal
- [x] Simulation checken
- [ ] simulationen auf CPU02 checken, wenn fertig auf /data kopieren
- [ ] für 1:3 ratio neues Jupiter Python Script anlegen 
- [ ] 1:3 pe 30 112k m 0.02 auf cluster abbrechen und mit 128 kernen auf cpu02 laufen lassen
	- [ ] vergleichen mit 1:10
- [ ] bevor ich dann von dem Kram etwas auswerte schreibe ich das ~={DeepSkyBlue}scheiß Proposal fertig=~ und bereite den ~={purple}schmutzigen talk=~ vor 
- [ ] wenn mache ich die Auswertung und die abp Simulationen nebenbei 
- [ ] algo anpassen und vergleichen, aufräumen, insbesondere auf GitHub hochgeladen 
- [ ] com Methode machen 
	- [ ] dafür all die Funktionen wieder verwenden 
	- [ ] aber eine neue saubere evaluate funktion
	- [ ] und saubere eval frame funktion schreiben 
	- [ ] schiebe com wie in maggi auf $x=\frac{L_{x}3}{4}$ dort die fest die zwei dense boxen und entsprechend auf$x=\frac{L_{x} }{4}$ die zwei dilute boxen
- [ ] Vergleich 3.5k
	- [ ] pe 30 und pe 35 
	- [ ] 1:3, 1:5, 1:10
	- [ ] m 0.04 und m 0.02 bzw m 0.01
	- [ ] erkläre, dass box Ratio 1:3 das bessere ist. Statistik subbox Größe. Warum wir aber 1:5 gewählt haben (mandal2019) und dann 1:10 gegangen sind. Den klaren Vergleich dass 1:3 doch besser für MIPS ist, hatten wir nicht. Ist aber auch einleuchtend. Denn für die System size ist ja durch die kleinste Ausdehnung in eine Richtung gegeben und das ist nunmal die y Richtung. Und mit 1:10 bzw. 1:5 erhöht man die Einschränkung und damit die finite size Effekte
- [ ] cancel all pending simulations
	- [ ] instead simulate the masses 0.02 and 0.03 for all former data if this full connected mips is maintained even for 1:10 ratio
- [ ] wenn ich abp Simulationen mit script von Leif mache, dann auch im 1:3 ratio
- [ ] mache keine "near" abp Simulationen da die zu lange dauern wegen der extrem niedrigen step size
- [ ] Simulation mit PE 30 mit niedrigerer Masse 
	- [x] 0.02
	- ~={RedRed}⟹ Bingo!=~
	- [x] repeat with 1:10 ratio
- [ ] simulation mit PE 35 mit 
	- [x] 1:10 ratio
	- [x] 1:5 ratio
- [ ] Kästchen Methode mit com schreiben 
	- [ ] code so schreiben dass ich vieles von dem Code den ich habe weiter verwenden kann
	- [ ] modularer machen 
	- [ ] zb das Kästchen zeigen 
	- [ ] evaluate für com Methode 
- [ ] Ergebnisse mit meiner Methode vergleichen 
- [ ] PE 150 erwähnen, dass es hier MIPS sofort entsteht 
- [x] Simulation mit PE 50 mit 3.5k Teilchen 
- [x] Simulation mit PE 50 mit 7k Teilchen 
- [x] Simulation mit PE 40 mit 3.5k Teilchen 
- [x] Simulation mit PE 45 mit 3.5k Teilchen 
- [x] Simulation mit PE 40 mit 7k Teilchen 
- [x] Simulation mit PE 45 mit 7k Teilchen 
- [ ] Begründung für die starke Abhängigkeit des Bindercumlants von der system size bei den kleineren kästchen
	- [ ] ich denke es liegt daran, dass die statistik eine stark andere ist. je kleiner die system größe und je kleiner die kästchen, desto weniger teilchen sind in den kästchen und somit verändert das die statistik stark.
	- [ ] begründung dazu gabs in rovere1990 und binder1981
- [ ] warum benutzen manche $Q_{L}$ und nicht $\mathcal{B}$?
- [ ] RESULTS OF THE ORIGINAL SUBSYSTEM METHOD lesen
- [ ] siebert2018 + SI - nicht alle systemgrößen verwendbar
- [ ] prepare back up slides for questions 
	- [ ] one for the reasoning why to avoid interfaces is important 
		- [ ] picture of the local density distribution 
		- [ ] picture of the density distribution of the block density 
		- [ ] the not crossing of Q of ising model
		- [ ] comparison of the crossing of abp between block density distribution and modified Block-Distribution 
- [ ] ask nandita for help for wrapping things up or how much to say to certain things 
- talk
	- backup folien
	- stark reduzieren
	- wo setze ich den fokus?
		- auf die problematik der ursprünglichen methode eingehen
		- warum so viel wert auf das Auslassen der Grenzflächen gelegt wurde
		- erklären warum ich diese nicht verwenden konnte
		- local density distribution zeigen, dass ich das nicht einfach fitten kann, mit der distribution von rovere1990 *The gas-liquid transition of the two-dimensional Lennard-Jones fluid* vergleichen.
		- meine methode gut erklären
- [x] leif nach abp fragen
	- [ ] hab ich bekommen -> Simulationen starten 
- [ ] talk fertig vorbereiten 
- [ ] talk text in PowerPoint Notizen notieren 
- [ ] Text für Überleitung/Entwicklung zu meiner methode fertig schreiben 
- [ ] Vortrag stark reduzieren 
- [ ] den Text den ich für den Talk aufgeschrieben habe fürs proposal verwenden 
- [ ] Florian meinte auch dass bei höhere pe ein Übergang 1. Ordnung wäre. Eigentlich logisch, daher gut dass ich nicht mit 150 pe simuliert habe. Mal schauen was da raus gekommen ist
- [ ] die mod methode was ich Benno erklärt habe fertig beschreiben - also mit deren Annahmen über die distributionen und dass deren Methode die Zwischenbereiche der regime nicht genauer betrachtet.
- [ ] deren Evaluation mit der originalen block density nicht rein nehmen 
- [ ] dann den Übergang zu meiner methode beschreiben und begründen.
- [ ] die snapshots aus dem report nehmen 
- [ ] die Beschreibung der Methode aus den Folien nehmen 
- [ ] die results rein  - dort auch die Begründung des fehlenden peaks in $\chi$ von Maggi rein 
- [ ] auch die masterplots 
- [ ] und was ich bisher bei den ABP hab
- [ ] dann das Problem beschreiben was ich als Missverständnis hatte, das Problem mit dem Ratio 
- [ ] Ausblick - Vergleich mit ABP und Simulationen mit anderem box Ratio, die ursprüngliche Methode verwenden und vergleichen sowie meine Anpassung an meinen algo erwähnen so dass die Platzierung noch besser wird.
- [ ] über die pdf schauen die ich Benno als Antwort geschickt hatte
- [ ] intro schreiben dazu die von der llm zusammengefassten Ergebnisse von lukas und Suvendu erwähnen 
- [ ] abstract
- [ ] Titel anpassen?
- [ ] angepasste Bedienungsanleitung für create sim anhängen! Da wurden ja ein paar Veränderungen gemacht zb auch heute mit den Skripten 
- [ ] Lukas Hecht active refigerator lesen/überfliegen und von llm zusammenfassen lassen
- [ ] mandal lesen und von llm zusammenfassen lassen -> was kam da bei seiner temperatur raus.
# unsortiert
- [ ] unbedingt konto und briefkasten checken
- [ ] um die Kiwis kümmern 
- [x] Bart und Nasenhaare schneiden 
- [ ] papa nachdem selfie stick fragen, den ihm arooj geschenkt hat
- [ ] Versuch dich mal an einer ~={LawnGreen}ganzen Aufnahme von so 70%=~. Lass Solo2 dann erstmal weg (spiel zu dem Punkt Rhythm oder so).
- [x] Kleiderschrank reparieren
- [ ] simulationen auf CPU02 checken, wenn fertig auf /data kopieren
- [ ] Pflänzchen umsetzen 
- [ ] 13.-21.6.2026 woche der bot. Gärten
- [x] im Sekretariat bot. Garten 
	- [x] Sonntagsdienst ~={RedRed} erst überlegen, wann ich nen Dienst machen möchte=~
		- Für die Sonntagsdienste können Sie sich für zwei Schichten eintragen (09:00–12:30 Uhr und 12:30–16:00 Uhr). An folgenden Terminen suchen wir aktuell noch Unterstützung: 10. Mai, 7. Juni, 5. Juli, 2. August, 6. September und 4. Oktober.
	- [ ] und Dienst zum Helfen 
- [x] pflanzen aus der Sonne stellen und eventuell Pflanzen ein packen mit zu den Eltern 
- [x] jamil mein bsc Zeugnis + cv schicken 
	- [x] kann sein dass er auch das Zeugnis braucht ⟹ einscannen
- [ ] Essen mit Kartoffeln machen 
- [ ] Handtücher Küche tauschen 
- [ ] Bettwäsche wechseln 
- [ ] alten Rosmarin klein schneiden 
- [ ] sobald ich den Vertrag unterschrieben habe, karte für psychedelic festival kaufen 
- [ ] Biomüll runter
- [ ] abp anstellen
- [ ] gießen
- [ ] spülkorb sauber machen
- [ ] schauen wie ich mein Tablet Update
- [ ] lernen schneller und kleiner an der Tafel zu schreiben
- [ ] sofa saugen 
- [ ] Wäsche zusammen legen 
- [ ] Mieterhöhung unterschreiben 
- [ ] und Papierkram
- [ ] Toilettendeckel tauschen 
- [x] bei Kinder Betreuung bewerben 
	- [ ] ⟹muss ich nicht mehr, ok vielleicht wäre das für die Sommerferien gut
- [ ] Email an Schulen gingen raus?
	- [ ] ⟹muss ich nicht mehr, 
- [x] nachricht von jamil lesen
- [x] ~={DeepSkyBlue}ADHS Event=~ im Mai anmelden
	- glaube nicht dass ich zum AOK ding möchte
- [ ] Wasserhahn Küche silkonölen
- [x] Pflanzen gießen 
- [x] Hantelbank fest Schrauben 
- [ ] simon nach seinen Folien fragen 
- [ ] Vorderrad Bremse checken/einstellen/tauschen 
- [ ] Klingel checken
- [ ] meditieren 
- [ ] Lisa mank SMS schreiben
	- nicht nötig, da ich jetzt an der BAS bin
- [ ] tägliches Mantra aufräumen 
- [ ] ~={Crimson}Wie schaffe ich es immer aroused zu sein?=~
	- [ ] Angst 
	- [ ] Sport 
	- [ ] guter Schlaf 
	- [ ] voll bei mir sein
	- [ ] nur eine Sache gleichzeitig 
	- [ ] kein Medienkonsum
	- [ ] Achtsamkeit 
	- [ ] Körperpflege 
	- [ ] frische Luft
	- [ ] mich und mein Leben im Griff haben
- [ ] mich mal nach nem anderen file Browser (handy) umschauen 
- [ ] ~={MediumSpringGreen}Nähgruppe/Club/Treff=~ suchen
- [ ] ~={DeepSkyBlue}Strickgruppe/Club/Treff=~ suchen
- [ ] ~={green}Sachen auf die ich Lust=~ habe, die mir Freude machen vom Zettel an der abschreiben in Therapie
- [ ] arthur fragen was er von asagraum hält
- [ ] Benq bildschirm austauschen.... ich vertrag den echt nicht...
	- [ ] warum hab ich da all die jahre eigentlich nicht auf mich und meinen körper gehört
	- [ ] ich hatte immer im Kopf stell dich nicht so an.... 
	- [ ] ⟹ wenn man immer unterdrückt, dass man Bedürfnisse hat und unter gewissen umständen nicht arbeiten kann, dann achtet man darauf einfach nicht und zwingt sich immer weiter darein. ich hab immer das Gefühl gehabt, dass ich mich nur anstelle.
	- [ ] deshalb konnte ich auch keine Entscheidungen treffen und mich nicht für mich einsetzen.
	- [ ] ich habe meinen körperlichen Signalen, meinem Befinden und meiner Wahrnehmung einfach nicht mehr getraut
	- [ ] ich hab mich dann nur noch fertig gemacht bzgl. meiner Entscheidungen
	- [ ] ich wurde aber auch nicht ernst genommen
	- [ ] Es wurde sich dann halt schon ziemlich lächerlich darüber gemacht, als es zum beispiel auch um das fahrrad ging. Arooj hat mich dann schon ernst genommen. aber war auch irgendwie herblassend zu mir
- [x] bei den Faulbäumen vorbei gehen 
	- ⟹glaube die stehen am Weg hinter der Eissporthalle 
	- ⟹gibts keine Faulbäume ~={Crimson}⟹=~ das ist ein ~={Teal}gewöhnlicher Spindelstrauch=~
- [x] Erbsen kochen
	- ⟹keine grünen Erbsen mehr da 
	- ⤷ koche die letzten grünen Erbsen zusammen mit Kichererbsen
- [x] Email an Christian Morgenstern Schule schreiben 
	- war dort mir wurde gesagt ich soll eine Email schreiben
	- den Namen der Frau habe ich wieder vergessen mit der ich gesprochen habe
- [x] Email an ernst niebergall Schule
	- heute pädagogischer Tag
	- Frau mai auch eine Mail schreiben 
- [x] Tisch absenken 
- [ ] in vodafone konto einloggen
- [x] Lattenrost einstellen 
	- [x] Kameraaufnahme von unten, während ich drauf liege, um zusehen, was sich wie bewegt.
		- ⟹ sieht ganz gut aus
	- [x] ist jetzt besser, ohne Kamera. Hab die Halter größtenteils an die äußere Position gemacht 
- [ ] Steckdosenleiste unter dem Bett umsetzen 
- [ ] einkaufschip clip mit metallkleber kleben
- [ ] ~={Magenta}hessenbox=~ vom laptop entfernen
- [ ] check for new mac os update - the next newer than Sonoma
- [ ] Aritra fragen wie er genau alles in visual studio code eingerichtet hat
- [ ] emails aufräumen
	- [ ] jean-lueck
	- [ ] lukasludwigwalter
- [ ] ksk app contactless pay notification anstellen 
- [ ] nochmal über thunderbolt karte nachdenken
- [x] maus reparieren
	- Offenbar reicht es, wenn man ~={red}rein pustet=~ und damit die elektrischen Ladungen durch die Luftfeuchtigkeit reduziert
- [x] Termin mit seib glaszis ausmachen 
- [ ] Gyros+pita aus Gefriertruhe essen
- [x] was mit Gemüse und Tofu kochen
	- [ ] erst was mit den bohnen im Glas 
- [x] Bei Schulen vorbei schauen
- [ ] Konto checken
- [ ] Mischa wegen den Gehaltsabrechnungen Dez + Januar schreiben, sowie Februar. 
	- [ ] nochmal Vertrag wegen Kündigungsfrist und allgemein wegen Kündigungsfrist schauen
	- [ ] Schauen ob ich noch zugriff mit lueck.walter@gmail.com habe
	- [ ] Dann wegen den Stunden Seit 20.2. Da ich keinen Zugriff mehr auf Toggle hatte.
- [ ] Waschbecken Küche 
- [ ] nadines socken weiter
- [x] dpag Laptop aufräumen 
	- [ ] Zeug aus Obsidian raus machen was von mir ist
	- [x] Laptop zurück gebracht 
- [ ] mir überlegen was ich anders mache. Lehrer werde ich nicht
	- [ ] sind zu viele Namen 
	- [ ] zu viele Persönlichkeiten
	- [ ] ich möchte nicht die Aufsicht über so viele Leute haben 
	- [ ] zu viele Dinge gleichzeitig zu kontrollieren 
	- [ ] zu viele Sorgen 
	- [ ] dann fühle ich mich im Unterricht auch nicht
	- [ ] ich kann auch keinen jahrgangs gerechten Unterricht machen
	- [ ] und insbesondere nicht an dieser Schule
	- [ ] die Physikräume sind schrecklich 
	- [ ] ~={green}nicht so negativ in die Zukunft blicken, was ich nicht kann. Dazu neigt meine Persönlichkeit =~
	- [ ] ~={ForestGreen}auf die Vergangenheit positiv schauen, was ich alles geschafft habe=~.
	- [ ] ~={red}wie bringe ich Physik mit einfachen Mitteln bei=~
	- [ ] ~={Tomato}wie bringe ich Ordnung in mein Tafelbild=~
	- [ ] ~={Crimson}Ordnung in meine Gedanken und Worte bringen, weniger ist mehr=~ 
- [x] ~={Tomato}Antwort von ksk?=~
	- [x] habe bei Sparkasse angerufen. Kann ich selbst machen 
	- [x] ~={red}war ja schon zurück gebucht... Am 17.3=~
- [ ] Notizen zu "deine ~={ForestGreen}Gedanken=~ lügen" ab 2:05:47
- [ ] Teil bzgl weg zur Kästchen methode und von dort zu meiner methode fertig schreiben. Nochmal in report schauen was ich da schon geschrieben habe
- [ ] floyd rose stimmtutorial
- [ ] mgla anschauen
- [ ] vertrag nach Kündigungsfrist durch schauen
- [ ] was ist die mindst Kündigungsfrist in Deutschland 
- [ ] Laufen gehen
- [ ] Freddies Socken an der Spitze vernähen 
- [ ] Socken einpacken 
- [ ] Duolingo türkisch screenshots älter als 25-09-30 vom handy löschen
- [x] VSS Formular ausfüllen
	- [x] Versicherungszeiten AOK runterladen
	- [x] Studienbescheinigung
	- [x] brauche noch die vom nächsten Semester 
- [ ] Lebenslauf
	- [x] Arbeit am Staatstheater Darmstadt hinzufügen
	- [x] Wann habe ich im MPA gearbeitet
	- [x] Wann habe ich bei Birkl gearbeitet
	- [x] Von wann bis wann war ich genau Tutor
	- [x] wann war ich tutor für mathe für maschbauer 
	- [x] wann habe ich für mathis gearbeitet (21-23)
- [x] python auf cluster laufen lassen
	- ❌ wie mache ich das nochmal. Steht das in meinem Latex glossar
	- ❌ in meinem blauen notiz Buch 
	- ✅ oder in element im Chat mit arooj, Lukas Hecht und auf dem cluster
- [x] nach push und pull request bei kayro fragen
- [x] ärzte ohne grenzen kündigen
	- puuh gerade noch rechtzeitig.
	- [x] wird am 5.3. abgebucht, aber ich erhalte das geld zurück.
	- [x] <span style="font-size:100%;color:red;">regelmäßig konto checken</span>
- [ ] dpg kündigen
- [ ] jean-lueck aufräumen
- [x] konto checken
	- ich war heute 500€ im minus
- [ ] yoga
- [x] Camembert essen kochen
	- Camembert+Rotrinden Käse verwenden 
- [x] fragen was mit der Abrechnung vom September ist bzw schauen ob was kam 
- [ ] zip tight knoten lernen 
- [ ] tesaabroller schärfen
- [x] Ist geld vom november auf dem konto?
- [ ] Konto checken
	- [x] Gehaltsabrechnung checken und fragen was mit September ist
	- [x] Gehalt von November ist noch nicht da 25-12-21
		- 25-12-22 geld da
- [ ] Kühlschrank putzen und abtauen
- [ ] Zeug vor dem Bad wegräumen 

# tägliches

## Wohnbereich 
- [ ] Esstisch wischen 
- [ ] Sofa saugen 
- [ ] Boden saugen
- [ ] Boden wischen 
## Schlafbereich 
- [x] Bettwäsche wechseln 
- [x] Boden saugen 
- [x] Klamottenfach aufräumen 

## Küche
- [ ] Camembert Tomaten Essen machen 
- Arbeitsplatte
	- [x] saugen
	- [x] wischen 
- Kartoffeln
	- [x] waschen
	- [x] schälen
	- [x] schneiden
	- [x] frittieren
- Spülmaschine
	- [x] ausräumen
	- [x] anstellen 
	- [x] Regeneriersalz
	- [x] Klarspüler 
- [x] Erbsen kochen 
- [x] Erbsen in den Kühlschrank
- [x] Medikament bestellen 
- [x] Medikament abholen 
- [x] Avocado 🥑 essen
- [x] auberginen + tofu
-  Hülsenfrüchte Tofu
	- [ ] Hülsenfrüchte über Nacht einweichen 
	- [ ] erstes Wasser abgießen 
	- [ ] mixen und würzen
	- [ ] mit genug Wasser aufkochen 
	- [ ] etwas abkühlen lassen
	- [ ] in Dose füllen und in den Kühlschrank 
## Bad
- [x] Bart schneiden
- [x] Bart Halsregion rasieren
- [ ] saugen und wischen
- [ ] Toilette putzen
- [ ] Toilettendeckel/sitz tauschen 
- [x] Dusche schrubben 
## technisches
- Obsidian 
	- [x] text wrapper size in shortcut einbauen 
		-  <span style="color:red;font-size:120%">test</span>
		- <span style="color:green;font-size:130%;">test</span>
	- [x] quiet outline drag heading testen
	- [x] was macht autovervollständigung in der dataprotect knowledge base? 
		​⟹completr
	- [ ] remove .obsidian/app.json
	- [x] check the git version on mac, how it is installed and update it
	- [x] deinstall the old git version in windows 
		- <span style="color:gold">⟹nicht nötig</span>

## Wäsche, Kleidung und Stoffe
- [x] Bettwäsche wechseln
	- [x] Kopfkissen und Bettdecke 
	- [x] Spannbettlaken 
- [x] neuen Schlafanzug 
## sonstiges
- [x] Kartons wegräumen 
- [x] wann ist der Vortrag im hessischen Landesmuseum 
	- war ein toller Vortrag und ich habe Laura kennengelernt 
- [x] Konto checken 
	- <span style="color:red">⟹noch kein Geld von Oktober auf dem Konto</span> 
	- 21.11 immer noch kein Geld
	- 24.11 volles Geld erhalten 
- [x] staubsaugen 



# Masterarbeit
- [x] susceptibility 
	- [x] L extract
	- [x] berechnen 
	- [x] exportieren 
	- [x] exponent berechnen 
- [ ] Folien 
	- [ ] mit Ergebnissen fertig machen 
	- [ ] Benno schicken 
- [ ] proposal 
	- [ ] zinos proposal lesen 
	- [ ] proposal aufräumen 
	- [ ] Theorie 
- [ ] Code fertig aufräumen 

# Gesundheit
- [x] beim nächsten Arzt Besuch bei Herrn lojko die Patienten akte wieder mitnehmen 
## körperlich

## mental
- [x] Notizen zu *why you can't finish simple tasks* machen
- [x] Notizen zur Kommunikation Friedemann schulz von Thun 
# Arbeit
## Arbeitssuche 
- definitiv noch bei Aldi/Rewe vorbei schauen
- Kitas 
	- [x] Krabbelstube "kleine Entdecker*
	- [ ] quatschmacher 
		- waren nicht da
	- [x] internationale lern und Spielstube 
		- ska E-Mail Adresse Bewerbung schreiben 
		- bewerbungen@ska-darmstadt.de
	- [ ] flugis Abenteuerland 
		- flyer bekommen 
		- Bewerbung online (Nina Büttner)
		- ⤷steht auf Flyer 
- Schulen
	- [x] Lio 
		- herr Keller auf skifreizei bis Ende der Woche
		- Email schreiben: ich würde gerne auch etwas mehr arbeiten als beim letzten Mal
		- [x] Email geschrieben
	- [x] Ello
		- coors ist der zuständige 
		- [x] Email ans Sekretariat (Adresse auf der Website )
	- [x] Kyritzschule (y gesprochen als ü) Grundschule
		- mit Frau Jonas gesprochen 
		- warte bis 12:30 auf den stellv. Schulleiter 
		- sms von Lisa Mank (Konrektorin) und dann darauf reagieren.
		- habe dort jetzt bereits einen Termin zum Arbeiten
	- [ ] Mädchenschule ist wo?
	- [x] Christian-Morgenstern-Grundschule
		- habe meine Kontaktdaten hinterlassen für SSV
	- [x] Bernhard-Adelung-Schule (integrierte Gesamtschule)
		- Gespräch mit Jamil (auch Physiker)
		- SSV Daten hinterlassen
		- Möglichkeit auf TVH Vertrag (spätestens ab Sommer)
-  Lebenslauf hinzufügen:
	- [ ] Arbeit an Schule
	- [ ] Arbeit bei DATAPROTECT 
	- [ ] Stärken 
- [ ] Bewerbung:
	- [ ] nterra
	- [ ] telespatio
	- [ ] Merck 
	- [ ] Landschaftsgartenbau 
	- [ ] kitas
	- [ ] Schulen 
	- [ ] Forst 
## Frisör Queueing System 
Ein queueing system für den Frisör
Scannst du qr Code
Dann bist du der nächste in der Reihenfolge.

Musst halt noch angeben was du möchtest. 

Augenbrauen etc.
Und dann kannst du halt auch wieder gehen wenn viel los ist. 

Es wird dir ungefähr die Zeit angezeigt bis du dran bist.
Und je nachdem was du brauchst musst du eben länger warten. 

Eventuell kannst du noch den jeweiligen Frisör buchen.

Also angeben ob du gerne einen bestimmten hättest.
Macht man halt ein Abo Modell und das wird durch den Frisör bezahlt.

Nicht viel 1-2€ pro Mitarbeiter pro Monat.
Dadurch steigert sich halt die Kundenzufriedenheit immens.

Da es kein Gerangel gibt "wer war zu erst" oder "oh jetzt habe ich so lange gewartet und komme trotzdem nicht dran" oder "oh mir wurde gesagt sie können nachher nochmal kommen und dann ist man aber aus der queue draußen"
So was geht auch für Nagelstudios oder massage Salons.

Die halt keine Termine machen
- [ ] Programmiersprache?
	- [ ] java
	- [ ] python 
- [ ] android studio 

Kotlin und Java für Android, Swift für iOS, während Frameworks wie Flutter (Dart) und React Native (JavaScript/TypeScript) Apps für beide Plattformen mit einer einzigen Codebasis ermöglichen. 
Native Entwicklung (Spezifisch für eine Plattform)
Android:
Kotlin: Googles bevorzugte, moderne Sprache für Android, prägnanter und sicherer als Java.
Java: Etabliert, vielseitig und stabil; eine solide Basis für viele Android-Apps.
iOS (Apple):
Swift: Apples moderne, leistungsstarke und sichere Sprache für alle Apple-Plattformen.
Objective-C: Der ältere Vorgänger von Swift, wird aber noch in älteren Projekten verwendet. 
Plattformübergreifende Entwicklung (Cross-Platform)
Flutter (Dart): Entwickelt von Google, ermöglicht schnelles Erstellen von Apps für Android, iOS, Web und Desktop mit einer einzigen Codebasis und bietet native Performance.
React Native (JavaScript/TypeScript): Ermöglicht die Entwicklung nativer Apps mit Webtechnologien.
C#/.NET (Xamarin): Ermöglicht die Entwicklung von Apps für verschiedene Betriebssysteme. 
Weitere Sprachen
Python: Einfach zu erlernen, ideal für schnelle Prototypen und einfache Apps (z.B. mit Kivy).
C++: Wird oft für performancekritische Teile, Spiele oder wenn native Performance über Plattformen hinweg benötigt wird, eingesetzt. 
Entscheidungshilfe:
Für große Reichweite (Android): Beginne mit Kotlin.
Für Apple-Nutzer: Swift ist der Standard.
Für beide Plattformen (mit weniger Code): Flutter (Dart) oder React Native (JavaScript) sind gute Optionen. 

## DATAPROTECT 

- [x] Support Chat bei coreview Wegen den report entries fragen 
- [x] coreview <span style="font-size:100%;color:red;">reports</span>
- [ ] Understanding data import lesen
- [ ] Mischa entlasten und nicht noch mehr Arbeit machen 
- [ ] mehr mit den Tasks arbeiten 
- [x] robert wegen pentesting schreiben 
- [x] coreview Training 
- [ ] occident secure score fertig testen
- [x] komax reports zum Vergleich neu
- [ ] MS Sentinel weiter verstehen
	- [ ] ausprobieren, was in le chat steht
- [x] security awareness
- [ ] custom action bauen:
	- [ ] auto Archive
	- [ ] remove cancel calendar entries from today on
- [ ] MS Sentinel einarbeiten
	- [ ] ein paar eingaben testen
- [ ] Call mit ninja one vereinbaren
	- [ ] für eine Einführung
- [ ] MS Secure score abschließen
	- [ ] welche policies nehmen wir und welche nicht?
	- [ ] alle gescheit testen
	- [ ] und die letzten nicht funktionierenden fixen
- [ ] <span style="font-size:100%;color:red;">prio</span> Research Exchange Hybrid abbauen
	- [ ] muss wirklich save sein, dass man das <span style="font-size:100%;color:red;">wegwerfen kann</span> 
	- [ ] geht um die Abschaltung von Zug
- [ ] Support anfragen an Coreview bzw. im Demo tenant testen:
	- [ ] license pool
	- [ ] audit add on
- [ ] LDAP ENCRYPT Mischa die version mit OMA URI schicken
	- [ ] in der VM testen
- [x] VM umstellen 
- [x] coreview reports
- [ ] power shell kurs für visual studio code
- [x] die<span style="font-size:100%;color:red;"> wichtigsten 5-10  </span> <span style="font-size:100%;color: lawngreen;">sinnvollen</span> policies auf gängigkeit überprüfen damit wir sie deployen können
- [ ] <span style="font-size:100%;color:red">mich gut in Coreview einarbeiten, da ich ab nächsten jahr mehr mit coreview zusammenarbeiten werde</span>
- [ ] bräuchten Soft fail bei den workflows
- [ ] if closes in den Workflows anschauen
- [ ] ms Security weiter machen 
- [x] Georgios nochmal schreiben
	- [ ] der antwortet nicht
- [ ] zero Trust Assessment+maester.dev
	- [ ] zero trust assessment hat
	- [ ] nicht geklappt 
	- [x] maester dev hat geklappt 
- [x] mit einem älteren Checkpoint in der VM verbinden. ist es der richtige? Wie geht das?
- [x] Hybrid Connector 
	- [x] ⟹ <span style="color:gold">habe keinen Zugriff</span>
- [ ] heylogin 
	- [x] wie ich jemandem meinen "contact" senden kann damit dieser mir Passwörter geben kann
	- [ ] so bereit stellen damit es auf der Webseite gut aussieht 
- [ ] standard powershell tutorial + notizen machen
- [x] Pentesting Websiteeintrag <span style="color:red;font-size:120%;">Priorität</span>
- [x] demo tenant einrichten 
	- [x] pw in heylogin eintragen 
- [x] Outlook task planner zeug eintragen was mir Mischa aufgetragen und nicht selbst schon eingetragen hat 
- [ ] 
# Papierkram
- [ ] Lebenslauf / CV
	- [x] Arbeit am Staatstheater Darmstadt hinzufügen
	- [x] Wann habe ich im MPA gearbeitet
	- [x] Wann habe ich bei Birkl gearbeitet
	- [x] Von wann bis wann war ich genau Tutor
	- [x] wann war ich tutor für mathe für maschbauer 
	- [x] wann habe ich für mathis gearbeitet (21-23)
	- [ ] Zellenwartlehrgang einscannen
	- [ ] zweispaltig machen
	- [x] Wann war das Försterpraktikum genau?
	- [x] wann war mein Praktikum in der Revo Goldschmidt
- [ ] AOK
	- januar 258.28
	- Februar 346.76
	- Warum wurde der Betrag um fast 100€ erhöht und ich wurde darüber nicht informiert
	- 292.28, ist der angepasste betrag. deshalb wurde mir rückwirkend Geld abgebucht
	- habe weitere Email adresse eingetragen
	- <span style="font-size:100%;color:limegreen;">und eingestellt, dass ich Benachrichtigungen wieder per post erhalte</span>
- [ ] Rundfunkbeitrag 
- [x] Lohnabrechnungen für die AOK hochladen 
- Stromablesung 
	- [x] Termin 26-01-09
	- [x] online eintragen 
- [x] AOK KK Karte und Zeug einheften
- [x] Patientenakte abholen/besorgen
- [x] wbs legal einheften
- [x] Bauverein einheften 
- AOK verdienst melden 
	- haben sich gemeldet ich sollte die Gehaltsabrechnungen September und Oktober einreichen 
	- [x] Robert schreiben 
	- [x] BAT schreiben?
	- [x] Gehaltsabrechnungen an AOK weiterleiten
	- [ ] ist die auch korrekt?
	- [ ] ist ein Brief in der Post?
- [x] Patientenakte anschauen ⟹ wie viele Seiten sind das? Doppelseitig? Lohnt sich das zur Digitalisierung den Drucker zu kaufen? Alleine wie genervt ich von dem Drucker bin.. und wie viel nervige Zeit es kostet Sachen einzuscannen und dann ist das nicht gerade und schön. Auch das Scannen an den pc ist ne Katastrophe mit dem hp
- [x] Drucker in ebay Kleinanzeigen stellen 
	- gebe den Drucker Bilge 
- [x] alten Drucker abbauen 
- [x] neuen Drucker aufbauen 
 
# Ahl
- [ ] Maronen in den Wald setzen
- [ ] Gedanken machen welche heimischen Blüh Pflanzen ich auf die beiden Grasflächen im Hof anpflanze. ⟹robinga
- [x] Kartoffeln stecken 
- [ ] Teich planen 
- [x] Holz holen
- [x] Papa zeigen wie er gerade und ungerade Seiten eines scans merged
	- hat mit scan Gear viel besser geklappt als mit pdftk
# wenn ich lust und zeit habe
- [x] Fenster putzen 
- Carcassonne 
	- [ ] Eclipse Updaten
	- [ ] java updaten
	- [ ] funktioniert das Spiel noch? Testen 
	- [ ] klassenaufbau verstehen 
	- [ ] peer to peer host system 
	- [ ] karten erweitern 
- [ ] Schreibtischauflage
- [ ] Akustikgitarre Saiten wechseln
- [x] Sparkassen App+push tan
- [ ] maus reparieren 
	- geht momentan wieder
- [ ] Klodeckel
- [ ] Ackerbohnen säen
	- [ ] ahl
	- [x] Balkon 
- aus Destilliertem Wasserbehälter
	- [ ] Behälter für carnivoren 
		- ich hab diese Glaskaraffe 
	- [ ] aufhängbaren Behälter für Pflanzen 
	- [ ] Schaufel 
	- [ ] mini outdoor Gewächshaus 
- [ ] dusche dampfen
	- ⟹Dusche habe ich aber geschrubbt
- [x] Sauerteig auffrischen 
      <span style="font-size:100%;color:gold;">⟹Egal in irgendein Fladenbrot hauen und dann egal</span> Ist <span style="font-size:100%;color:red;">Ablenkung</span> Wenn ich leckeres Brot gehe, dann gehe ich zum Bäcker und stopfe mein Gehirn nicht mit unwichtigem Zeug voll
- Fermentieren
	- [ ] Knoblauch 
	- [ ] Gemüse 
- [x] Klarspüler clip zurecht schneiden/schleifen 
	- hat ganz gut geklappt mit der kleinen Akkuflex 

# Nähen, Malen, Basteln und Reparieren 
- [ ] Uhr reparieren 
- [ ] Chiphalter reparieren 
	- metall 2 Komponenten Kleber verwenden 
- [ ] neue Saiten auf Akustik 
	- [ ] Griffbrett säubern
	- [ ] Klinkenanschluss wieder anbringen 
		- [ ] dafür mutter und u scheibe suchen/besorgen 
- [x] flipflop reparieren 
	- ~~runde Scheibe durchbohren~~ ⟹ unnötig 
	- [x] oberen Teil 
		- [x] rest entfernen 
		- [x] durchbohren 
	- [x] gelbes seil durch und Knoten unten machen
		- habe weißes seil genommen
	- <span style="font-size:100%;color: limegreen;">⟹perfekt!</span>
- [ ] Winterschuhe braun sole kleben 
- [x] Loch im grünen Shirt flicken 
- [x] Handschuh flicken
- [x]  Aldi Tasche reparieren
- [ ] Leuchtstoffröhrenlampen 
	- [ ] Kabel für Lampe finden ⟹Lampe drehen 
	- [ ] Lampe vorne am Rand anbringen 
	- [x] hab sie mit Kabelbindern angebracht 
- [ ] das Problem mit der 90iger Universal Nadel raus finden.
	- mit den anderen Nadeln vergleichen Öse und Länge der Nadel ⟹ eventuell Länge abschleifen <br> ⟹hat geklappt <span style="font-size:100%;color:coral;">hab sie dann aber mit dem hammer zerstört als ich beim zweiten mal probiert habe die Öse mit einem Nagel etwas zu vergrößern. Sie ist dadurch gebrochen an der Öse. ich wusste es habe, es aber trotzdem gemacht, konnte es nicht lassen</span> <span style="font-size:100%;color:red;">ist aber nicht schlimm, ich habe daraus etwas gelernt</span> ich hatte dabei das erste Mal wieder das Gefühl "oh mein Gott ich habe etwas falsch gemacht und war kurz davor mich da weiter fertig und runter zu machen siehe PC etc." ⟹ der Fehler war nicht 100% bei mir und achtsam zu sein
	- ist die Nadel zentriert?
- [x] Schlafmaske reparieren 
- [x] Näh und Bastelecke einrichten 
	- <span style="font-size:100%;color:red;">yeahy</span> 🥳🎉
- [ ] Nähmaschine ersteinrichtung
	- [x] Auspacken und Aufstellen 
	- [x] Faden aufspulen
	- [x] erste test nähte
	- [x] Knopfautomatik 
- [ ] Monblume weiter malen
- [ ] Becorns basteln
- [x]  Schlafanzughose flicken
- [x] Jack Wolfskin Schuhe Schnürsenkel reparieren
- [x] graue hose Knopf reparieren 
# Pflanzen 
- [ ] salat aussäen
- [x] Bohnenkraut einpflanzen 
- [x] zitrusgewächse umpflanzen 
	- [x] limequat 
	- [x] Kumquat 
	- [x] calamondinorange
- [x] Sellerie einpflanzen 
- [x] Erdbeeren Pflegen
- [x] vogelmiere bei Pfefferminze entfernen 
- [x] kiwi aussäen 
	- [x] pikieren 
- [x] maracuja aussäen 
- [x] Löcher in Thunfischdosen bohren und einpflanzen:
	- [x] kiwi
		- angefangen 
	- [x] Apfelpflanzen 
	- [x] maracuja Pflanzen 
- [x] apfel Keimlinge umsetzen 
- [x] Basilikum säen
- [x] habanero Pflanze säen
- [x] loch für Bioabfall neben Oregano graben
- [ ] zitrone umsetzen 
- [x] Schnittlauch dahin wo Basilikum war
- [x] Melisse bei Erdbeeren entfernen 
	- [ ] dort nach physalis Pflanzen suchen
- [ ] root grow stimulants 
	- [ ] 350mg tablet aspirin in wasser 
		- die Stecklinge haben sich stark verfärbt, man sieht die Wirkung der Säure. Ob das gut ist🤷
		- sind verreckt 
	- [ ] honig in heißem Wasser verrühren ⟹nur rein dippen
	- [ ] 5 tropfen Apfelessig in auf eine halbe Tasse Wasser ⟹ nur dippen 
	- [ ] Bananenschalen (bio) wasser 24h einweichen 
- [x] carnivoren umsetzen 
# Musik
- [ ] Beltaine hohe Flöte üben 
- [ ] die dünneren jazz saiten auf die schwarze gitarre machen
- [ ] neue Saiten auf Akustik 
	- [ ] Griffbrett säubern
	- [ ] Klinkenanschluss wieder anbringen 
		- [ ] dafür mutter und u scheibe suchen/besorgen 
- [ ] füsilier alles üben
- [ ] fresh fur 
	- [ ] lead guitar 
	- [ ] gesang die töne in guitar pro versuchen zu treffen 
- [ ] Waffenbrüder Gitarre und Text
	- [ ] solo üben
	- [ ] Text stimme richtig üben
- [ ] fresh fur lead Gitarre
	- [ ] Anfang 
- [ ] the dream and the waking
	- [ ] lead vom Anfang auf 90% perfekt ⟹100%
	- [ ] main melody + text sync
	- [ ] Übergang main Melodie ⟹verse Melodie 
	- [ ] text sync Chorus vor zweiter main Melodie 
	- [ ] Übergang main Melodie ⟹"tremolo" picking (auf 100%)
	- [ ] Stakkato 
- [ ] soon departed auf +70% spielen 
- [ ] ride on spirit ⟹ solo üben
	- [x] mal damit angefangen 
- [ ] awakening:
	- [ ] Teil bis zur Melodie lernen
	- [ ] Alles bis dahin auf 60% perfektionieren und dann auf 70% hoch 
	- [ ] pull off hammer on tabbing solo anschauen <span style="color:red;font-size:100%;">Transition</span> + <span style="color:red;font-size:100%;">Solo A</span>
	- [ ] melodie solo anfang <span style="color:red;font-size:100%;">Solo B</span>
- [ ] mir die neuen Chor Stücke anschauen 
- [x] neue Boxen auf Sofa neben Router 
- [x] pod go neben sofa stellen und dort an den strom anschließen 
- [ ] mal ne flying V anschauen 
	- [ ] ESP SV-STD WH
# Lesen und Hören
- [ ] Universum in einem einzigen Atom 
- [ ] Einführung in die Charakterkunde 
# Filme, Serien und Dokus
- [x] <span style="color:gold">ghostbusters runterladen</span>
- [x] <span style="color:coral">paartherapie S3 runterladen</span>

# Alt
- [x] restliche Paprika ernten 
	- bis jetzt hängen noch ein paar draußen. 
	- bin gespannt wie sie die Kälte vertragen 
- [x] git am pc gescheit einrichten und Accounts trennen 
- [x] git in obsidian am Handy einrichten ==hat hoffentlich geklappt wir werden es sehen==
- [x] Wasserwaage auf rechten Bildschirm
- [x] git (richtige ssh keys) und Obsidian mit git am unirechner einrichten  
- [x] grünen Stift zum Schreiben bringen
- [x] carnivoren Wasser
- [x] stoffhandschuh flicken 
- [x] sparschäler kleben
- [x] passendes Gärkorbset suchen<br>⟹<span style="font-size:100%;color:gold;">ne unwichtig</span> <span style="font-size:100%;color:red;">Ablenkung</span>
- [x] duschen
- [x] um Teig kümmern
- [x] Wäsche zusammen legen
- [x] Tastatur wischen
- [x] Fladenbrot mit Sauerteig 
- [x] Erbsen kochen 
- [x] Sonnentau ausgraben und umsetzen 
- [x] Bettwäsche wechseln 
- [x] alten canon Drucker aus dem Handy entfernen 
- [x] Canon Drucker mit Laptop verbinden 
- [x] Essen
- [x] Spülmaschine
- [x] Krafttraining
- [x] Staubsaugen
- [x] Tastatur wischen
- [x] Bart
- [x] Zähne putzen
- [x] Duschen
- [x] Duolingo
- [x] Konto
	- ⟹noch kein Geld bekommen
- [x] Aldi
- [x] Sofa Decken
- [x] Zeug abheften
- [x] bei SHG anmelden 
- [x] Mischa Stunden schicken 
- [x] Tafel abschreiben 
- [x] adventssfeier checken 
      ⟹ war ich leider viiiiel zu spät die Mail war ja schon vom 25.10 und seitdem auch die Anmeldung offen... Es gab zu viele Anfragen. Aber naja mach dir nix draus Luk und katastrophiere nicht.😒
- [x] unter dem Bett aufräumen 
- [x] Nähmaschinenpreis checken
	- ⟹montag kaufen
	- ⟹<span style="font-size:100%;color:red;">gekauft yeah</span> 🥰🥰🥰🥰
- [x] Hülse auf boxen Bändel kleben 
- [x] Nähmaschine einrichten und Faden auffädeln 
- [x] Wiki Eintrag für glue 
- [x] mintfarbene Jogginghose flicken
- [x] gelben Pulli flicken
- [x] Dusche schrubben 
- [x] informieren wie man die android policies ändert
- [x] Weihnachtsmarkt Pilzgericht nach kochen 
- [x] Staubsaugen 
- [x] Sofa saugen
- [x] Küche aufräumen 
- [x] Bestellung auspacken 
	- [x] aux Kabel ausprobieren 
	- ⟹perfekt so ist es echt wunderbar. Dummerweise habe ich ausversehen zwei bestellt
- [x] Fritteuse 
	- [x] in Spülmaschine
	- [x] und weg packen 
- [x] Canon am Laptop installieren
- [x] Lotos set durchführen
- [x] oxana schreiben wegen Weihnachtsfeier 
	- [x] mache ich heute persönlich 
		- hab ich nicht geschafft 
	- hat sich erledigt, ich war nicht da
- [x] Küche aufräumen 
- [x] Glasmüll weg
	- ⟹war total voll, muss ich morgen nochmal probieren 
	- ⟹immer noch voll 12-09
	- ⟹12-13 weggebracht
- [x] aok neues Bild hochladen 
      ⟹habe das Bild vorher mit Gimp aufgehellt
      ![](Pasted%20image%2020251215173627.png)
- [x] Schnittlauch umsetzen 
	- nach drinnen nehmen
- [x] Schneidermatte + Rollschneider + Aux Kabel zusammen bestellen
- [x] Klapptisch von hinten als Nähtisch unter das Bett stellen
- [x] unter dem Bett aufräumen
- [x] Chilis schneiden
	- sind tot und stehen draußen 
	- hab jetzt die aus dem Büro
- [x] nochmal Pilzgericht machen
- [x] müll runter
	- [x] ⟹gelber Sack wäre noch frei
	- [x] Biomüll
- [x] erde umgraben
- [x] Klapptisch von hinten als nähtisch unter das Bett stellen 
- [x] Brokkoli verarbeiten 
- [x] Pesto wegräumen 
- [x] Bettwäsche wechseln 
- [x] Bettdecke waschen 
- [x] Kaffeemaschine entkalken 
- [x] Waschmaschinen Waschpulverfach reinigen 
- [x] Einkaufschiphalter fixen
- [x] pc uni checken
- [x] Kabel kaufen
	- ⟹war im Mediamarkt 😂 zu teuer
- [x] getrocknete chilis weg packen 
- [x] Kichererbsen tofu 
	- ⟹perfekt geworden 
- [x] Briefkasten checken
	- ⟹waren die Nadel zum Tinte befüllen drin
- In Kühlschrank
	- [x] Nudeln
	- [x] Erbsen
- [x] susceptibility
- [x] Kartons
- [x] Fotos vom alten Drucker
	- muss ich nicht, ich gebe ihn Bilge 
- [x] Essen Kochen
- [x] Meditation
- [x] E-Mail an Arooj entwerfen
	- ⟹hab ich mit angefangen und ein Google Doc erstellt
- [x] Klarspüler clip tauschen 
	- [x] Clip mit akkuflex anfertigen 
- [x] Paprika verarbeiten 
- [x] Nähmaschine im Aldi checken
- [x] Spazieren
- [x] weste waschen
- [x] hybrid connector
- [x] MFA für HRZ und PKM einrichten
- [x] müll runter 
- [x] ~={Crimson}AOK Zettel ausfüllen + hochladen=~ 
	- [x] ausfüllen 
	- [x] Studienbescheinigung runterladen
- [x] Zeug Angi vorbeibringen
	- [x] mit ihr Termin für 26-03-25 6:30 pm ausgemacht
- [x] aldi
	- [x] Milchmäuse oder so kaufen um einige davon mit dem Teller zurück zu geben
- [x] Wetterstation Batterien tauschen
- [x] job news letter deabonnieren