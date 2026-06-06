- [ ] Unterschrift 
- [ ] Datum eintragen 
- [ ] 1. neue erkenntnisse beschreiben unterschied zwischen den verschiedenen PE und box ratios
	- [ ] sagen dass das ein irrweg war, dass das box ratio es schlimmer gemacht hat, was auch logisch ist warum... Der Gedanke war die vertikale aufspaltung zu verringern, hat damit aber die horizontale aufspaltung verstärkt, das war damals ein Tipp von einem Doktorand aus der Arbeitsgruppe und um die in siebert erwähnte slab like structure ~={red}siebert2018 zitieren=~ nochmal zu verstärken
		- [ ] man zwingt das system sozusagen sich aufzuspalten
		- [ ] der grund dafür ist, dass die systemgröße durch die kleinste ausdehung in eine Richtung beschränkt wird und das ist nunmal die y-richtung -> größere Finite size effekte
	- [ ] dann aber den Übergang dazu warum die kästchen methode
	- [ ] wie diese funktioniert

- [ ] Entweder historisch vorgehen, das war unser vorgehen, deshalb sind wir dazu übergegangen das ratio so zu wählen und dann die Methode anzupassen. Schon bereits erwähnen, dass sich später herausgestellt hat, dass das unnötig ist, bzw. der falsche weg war. 
	- [ ] Oder erst die aktuellen erkenntnisse und dann erklären, was das vorherige vorgehen war
	- [ ] ich denke die Mischung: unser vorgehen, was wir vorgefunden haben, die gedanken waren, und dann schonmal ausblick dass sich das vorgehen als unnötig und kontraproduktiv herausgestellt hat. Verweiß auf die section danach in der die aktuellen erkenntnisse stehen
	- [ ] dort dann direkt erklären, was der grund dafür ist, dass das ratio kontraproduktiv ist
	- [ ] bezug auf das phase diagram nehmen, leicht höhere PE gleich besseres ergebnisse
	- [ ] geht aber auch mit der vorherigen PE mit niedrigerer masse

- [x] Lukas hechts skript und arbeit erwähnen

- [ ] Chapter simulations ~={Crimson}refer to it=~

- [ ] What is active matter?
- [ ] importance of universality classes for active matter
- [ ] read jones
	- [ ] Chapter 1 
	- [ ] Chapter 2 
		- [ ] 2.1
		- [ ] 2.2
- [x] Intro kapitel zu what is active matter fertig schreiben
	- [x] Definition rein
	- [ ] reviewen
- [ ] Kapitel bzgl der Entwicklung der Methode fertig schreiben
- [ ] Beispiele Active matter
	- [ ] Janus particles Vrugt2025
- [ ] Übergang: Entwicklung der Methode -> meine veränderte Methode:
	- [ ] erwähnen, welche Änderungen an den Simulationen es ermöglichen die modifizierte Methode doch anzuwenden
	- [ ] Bilder von Pe 35 bzw. Pe 40 zeigen für ratio 1:10? habe ich da überhaupt welche?
	- [ ] darüber schreiben, dass das ratio wichtig ist
	- [ ] Vergleich: Pe 30 ratio 1:10 zu 1:3 für verschiedene ~={orange}Seeds=~ und verschiedene ~={yellow}System size=~
		- [ ] schwierig bei PE 30 und 1:10 eine zusammenhängende dichte Phase zu bekommen. die Masse muss dafür sehr stark reduziert werden
	- [ ] Hier benennen, dass die Erkenntnis erst später kam
- [ ] meine veränderte Methode erklären und die aktuelle Problematik beleuchten
- [ ] Vergleich der Auswertung der Methoden ist geplant, daher wurde auch dringend versucht die Masse soweit abzusenken, dass eine zusammenhängende dichte Phase entsteht
- [ ] create sim vollständig beschreiben. Ergänzungen hinzufügen.
- [ ] Intro:
	- [ ] active matter: Buchkapitel + dessen Verlinkungen
		- [ ] active brownian particles + Vergleich zu Ornstein Uhlenbeck
		- [ ] Dry model
		- [ ] different regimes
		- [ ] MIPS
		- [ ] particles with inertia (kurz erkenntnisse aus papern)
			- [ ] mandal (worauf referiert er? wo fängt es an?)
				- [ ] Davon die erklärung zum Unterschied beim Verhalten insbesondere bei MIPS
				- [ ] Löwen2020 Seite 3 Bild zum Vergleich der Stöße 
			- [ ] Hecht, das MIPS Phasendiagramm zeigen und dessen Erkenntnis kurz zusammenfassen (zur not ChatGPT verwenden)
			- [ ] Su2021 zusammenfassen Erkenntnis über das verhalten der local density distribution
	- [ ] phase transition allgemein -> dazu cheung, schwabl, gros, täuber
		- [ ] schauen, was ich dazu schon im report versuch stehen habe
	- [ ] critical theorie: critical exponents: täuber: Buch + Mitschrift; Hermann; stanley1971
	- [ ] renormalization group
	- [ ] finite size scaling: hermann; täuber: Buch und meine Mitschrift zur VL; sutapa Roy Mitschrift
		- [ ] grund legender Effekt, tritt wann auf?
		- [ ] Observable im infinite system -> scaling function -> Observable im finite
		- [ ] Binder cumulant
		- [ ] wie bekommt man die exponenten
- ~={RedRed}das war es an Theorie, mehr ist nicht nötig=~

# guidlines
- follow the Talk red line
# current tasks
- [ ] simulationen checken
	- [ ] br10-pe30
		- [ ] 3.5k 
			- [ ] m=0.0001=10^-4
			      bleibt auch bei verlängerung auf die doppelte simulationszeit bei einer aufspaltung in größtenteils zwei bereiche, die sich aber schon sehr nahe kommen und auch ab und an verschmelzen
				- ⟹ m=10^-5 gestartet
				- [ ] m=10^-5 zweite simulation auf cpu2 mit seed 04000  gestartet
		- [ ] simulation br10-pe30 7k 
			- [ ] m=0.005 
				- sieht gut aus, ab frame 32, daher verlängert
			- m=0.0005 
				- perfekt
				- starte bei 3.5k daher mit m=1x10^-4 nen neuen seed, vielleicht reicht das bzw ist gut genug
		- [ ] simulation br10-pe30 14k 
			- [ ] m=0.005
				- gar nicht beendet....
			- [ ] m=0.01
				- dafür sieht das bereits sehr gut aus und ist durchgelaufen
				- es spaltet sich aber über die Zeit auf
		- [ ] simulation br10-pe30 28k
			- [ ] m=0.005
				- [ ] sieht gut aus, ist aber noch fragmentiert
				- [x] ⟹ m=0.0005 gestartet
		- [ ] simulation br10-pe30 56k
			- [x] m=0.005 ⟹ fragmentiert
		- [ ] simulation br10-pe30 128k
			- [x] m=0.005 ⟹ fragmentiert
	- [ ] br3-pe30
		- [ ] 112k
			- [ ] m=0.005 fragmentiert, wächst gegen Ende der Laufzeit zusammen
			- [x] ⟹verlängern
			- [x] seed 04000 starten
			- [ ] das verlängerte sieht gut aus, ich verlängere es nochmal ~={Gold}verdreifacht=~
		- [ ] 56k
			- [ ] m=0.005 fragmentiert, wächst gegen Ende der Laufzeit zusammen
			- [x] ⟹verlängern
				- [ ] Verlängerung ist ab 56 zusammen gewachsen
				- [ ] ⟹nochmal verlängern
			- [x] seed 04000 starten
				- [ ] bei diesem seed ist es schon von anfang an zusammen gewachsen
				- [ ] ⤷ starte seed 03000
		- [ ] 28k
			- [x] m=0.005 hängt bereits zu beginn wunderbar zusammen
				- [ ] ja ist perfekt ⟹ verdoppeln um mehr daten zu bekommen
				- [ ] seed 04000 ist auch perfekt ⟹ verlängere diese deshalb nochmal
		- [ ] 14k
			- [ ] m=0.005 hängt bereits zu beginn wunderbar zusammen
				- [ ] perfekt für beide seeds, daher beide simulationen verlängern
		- [ ] 7k
			- [ ] m=0.005 hängt bereits zu beginn wunderbar zusammen
			      neigt zur fragmentierung, sieht aber gut aus
				- [ ] gilt für beide seeds
				- [ ] also der 04000 er seed sieht super aus
				- [x] verdreifache deren trajektorie, damit ich mehr daten habe
		- [ ]  3.5k
			- [ ] m=0.005 hängt bereits zu beginn wunderbar zusammen
			      neigt zur fragmentierung, sieht aber gut aus
				- [ ] gilt für beide seeds
- [ ] gliederung
- [ ] Talk text 
	- [ ] ⟹ Gliederung 
	- [ ] ⟹ Einleitung
	- [ ] ⟹ stark kürzen für den Talk
- schreiben, dass ich im supplement von Siebert mit der original blockdensity methode es möglich war einen Schnittpunkt zufinden, die Genauigkeit ist nur schlechter ⟹ comparably large uncertainties ⟹ its results corroborate the estimate of the critical point in the manuscript (~={Tomato}corroborate =~ ~={LawnGreen} bestätigen, untermauern, bekräftigen=~)
- [ ] Hecht refigerator lesen
- [ ] Suvendus paper nochmal lesen
- [x] Siebert fertig lesen
	- [x] paper 
	- [x] SI
- [ ] Suvendus paper
- [ ] what is active matter lesen 
- [ ] Auswertungscode für original Kästchenmethode schreiben 

# important <span style="font-size:100%;color:tomato;">remarks</span>
- ich~={RedRed} will meine Arbeit Publikations fähig machen=~
- ~={Magenta}SI Siebert2018 Fig S4 b)=~ ⟹ mit Original subsystem Methode haben sie auch nen crossing point gefunden, der mit dem der abgeänderten Methode übereinstimmt. Der spread der intersections ist nur größer.
- ~={DeepSkyBlue}SI Siebert p2 Qualitative justification right side last paragraph:=~
	- "*For systems in the Ising universality class, critical correlations grow isotropically. Thus, the growth of the correlation length ξ is limited by the smaller linear dimension 2L in the chosen geometry.*" 
	- ~={Crimson}⤷ =~falls man davon ausgeht, dass das system zur ising universality class gehört
	- "*and when ξ is distinctly smaller than $2l$, the typical length scale $w$ of interfacial fluctuations in the  $d = 2$ Ising model is, from capillary wave theory and exact solutions: $w \propto \sqrt{ 2 l \xi }$, where the prefactor is of the order unity.*"
	- $w \propto \sqrt{ 2 l \xi }$ , where the prefactor is of the order unity
	- "This equation implies that for $ξ ≪ 2l$ the 'measurements' of the density in the subboxes cannot be affected by interfacial fluctuations, and it is reasonable to assume that the fluctuations in the liquid subboxes are independent from the fluctuations in the vapor subboxes."

> [!NOTE] "Order Unity" Regime
> The "Order Unity" Regime: Classical Capillary Wave Theory (CWT) applies to large wavelengths (small $q$). Microscopic CWT extends this to shorter wavelengths where the wavelength $\lambda$ is on the order of inter-atomic distances (or when wavevector $q \approx 2 \frac{\pi}{a_{0}}$, with being the particle size).
- Warum habe ich eigentlich keine PE von 200 oder 150 genommen???
  ![[../../Pasted image 20260420205452.png]]
- Es ist so oder so etwas unbegreiflich, warum wir keine höhere péclet Zahl zb. 150 verwendet haben, dann

# proposal tasks (moved)
- [x] Simulation checken
- [ ] simulation 1:10 pe 30 3500 m 0.005 verlängern, da es aussieht als könnte es nach 32kk steps stabil sein?
- [ ] Simulation 1:3 und 1:10 pe 32.5 112k
- [ ] `create-simulation_mod_p.sh -er -pr "equilibrateMaster_mod_p.in" "productionMaster_mod_p.in" "PE,30" 112000 "m" -4 .0005 .0005 .005 . 05000 -ts 4 -ss -cl -sc 64 -br 10 `
- [ ] überprüfen ob 28e30 irgendwann angefangen ist zu laufen, da 
      ![[../../Pasted image 20260428113150.png]]
      falls nicht:
      ` create-simulation_mod_p.sh -er -pr "equilibrateMaster_mod_p.in" "productionMaster_mod_p.in" "PE,30" 28000 "m" -3 .02 .03 .01 . 05000 -ts 4 -ss -cl -sc 32
`
- [ ] simulationen auf CPU02 checken, wenn fertig auf /data kopieren
- [ ] für 1:3 ratio neues Jupiter Python Script anlegen 
- [ ] 1:3 pe 30 112k m 0.02 auf cluster abbrechen und mit 128 kernen auf cpu02 laufen lassen
	- [ ] vergleichen mit 1:10
	- [ ] 1:3 sieht beim t=1kk noch aufgeteilt in zwei Bereiche aus, das ist ein gutes Zeichen, liegt also nicht unbedingt am ratio dass es aufgetrennt ist. bei N=3.5k  ist es direkt ein slab. Bei N=7k, quasi auch, über den zeitverlauf zerteilt es sich aber auch wieder, aber nur schwach. Das ist beruhigend. Es liegt also eher am jeweiligen run und es ist wahrscheinlich eine niedrigere masse notwendig. Die Zerteilung ist eventuell nur am anfang
	- [ ] 1:3 mit m=0.01 simulieren
- [x] alle 128k simulationen killen, da da ich 112k brauche...
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
# unsorted tasks
- [x] copy general plot to the non plot script
- [ ] wiki eintrag für jupyter on cluster verbessern
- [ ] set up visual studio code for amep auch am uni rechner
	- [ ] fix all branching 
	- [ ] and sort git hub
	- [ ] use llm to get the code sorted
	- [ ] and plan the coding
	- [ ] re-evaluating the concept with the std-dev around the peak
- [ ] wiki eintrag für create simulation programm
- [ ] fork von AMEP erstellen
- [ ] box algo code parallelize
- [ ] finish / reinvestigate approach of july 2025 where 
	- [ ] the peaks are filtered after the one-sided standard deviation of the  height of the highest peak inside the rectangle box (the center of the standard deviation isn't the average height but the peak or the second moment with $c=\text{peak}$)
	- [ ] and afterwards after the standard deviation of the x-position around the highest peak
	- [ ] and than the average of these peaks are calculated
	- [ ] this approach is independent of the size of the outer rectangle box
	- [ ] if the threshold for the peaks and pits are high, the total number of eval boxes are reduced, but not the quality of the placement is affected
	- [ ] but there must be still a filter for 
		- [ ] if the the eval square box is intersecting with the outer rectangle
		- [ ] if dense and dilute boxes are overlapping, the threshold value for the width of the outer rectangle box is reduced
			- [ ] or we are going back to the oldest approach that the rectangle box for the dilute phase is depending on the rectangle box of the dense phase. This avoids always the overlapping of the dilute and dense square boxes and also the overlapping of dense and dense and dilute and dilute boxes
			1. here the best approach is to use the stdv for the threshold for peak/pit
			2. the threshold is raised if the rectangle boxes are too narrow so that the square boxes aren't able fit in
			3. the threshold is lowered if there are to few square boxes. (which shouldn't be the case)
			- here is no quality management or overlapping / collision management necessary
- [ ] reset to the old algo from 1.1 or 2.2. and compare the behavior of the placement of 28k (snapshots)
- [x] 28k with new algo and stdHalf as start value from .07 to .09. compare the bindercumulant results
- [x] 3.5 k with stdhalf reevaluate 
	- looked quite good or?
- [x] check how the 3.5 k data looks like
- [ ] what can I change with the inner filter to get better results?
- [ ] auf alten algo zurück setzen 🤷
- [ ] if stddev is smaller than a certain value don't restrict to two pits 
	- [ ] found another solution
- [ ] migrate scripts on the cluster 
- [x] add a "post filter" for the pits and peaks
	- it should throw out all values within the standard dev
	- <span style="font-size:100%;color:red;">⟹seems to have nice results</span>
- [ ] To solve the problem that there are boxes in too narrow areas
	- [x] it must be necessary that there are at least two peaks / pits 
	- This filter I already have for the pits
	- [x] The actual square box must be inside the outer box
- [ ] For better results I switched from pit/peak height multiplier of stdDev/stdHalf to peakheightmul = 1.05 and pitheightmul = .95
      Comparisson:
	- stdHalf:
	  ![](box_sqSi23_frame_144000000.png)
	  ![](Pasted%20image%2020260222122153.png)
	  you see the magenta (dilute) square in the second row from above, which shouldn't be there
	- peakheightmul = 1.05 and pitheightmul = .95
	  ![](box_sqSi23_frame_144000000%201.png)
	  ![](Pasted%20image%2020260222122327.png)
	  here it is replaced by a green (dense) one
	  This is caused be the splitting of the horizontal density distribution with a lower threshold for the deviation from the mean value for the pit height and peak height.
	  ![](0.0_23.447361.png)
	  In comparison to a higher threshold (here the half of the standard deviation):
	  ![](0.0_23.447361%201.png)
- [x] create-sim auf general modifizieren 
- [ ] traj time step setzen mit `traj.dt=<dt>`
- [ ] create sim so modifizieren, dass restart etc mit -ow klar kommt
- [ ] Folien autor titel oben entfernen
- [ ] lammps skript anpassen
- [ ] simulationen für 
	- [ ] 14k
		- [ ] Pe=5,10,15,20,25,30,35
	- [ ] 28k
		- [ ] Pe=5,10,15,20,25,30,35
	- [ ] 56k
		- [ ] Pe=5,10,15,20,25,30,35
- [x] suvendu schreiben
- [x] Kayro nach ABP Daten fragen
- [x] Leif nach Lammps skript fragen
- [ ] Auswertung von $\nu$ überprüfen, eventuell Aritra fragen, ob ich nen fehler gemacht haben könnte.
	- [ ] ob er ideen im allgemeinen hat
- [ ] Proposal schreiben!
- [ ] Slides Numbering!
- [ ] Darstellungs/Auflösungsproblem bei plot mit den kleineren Kästchen klären
- [ ] use the model of hecht2021 ![](Pasted%20image%2020260116194755.png)
	- $$m  \frac{d\vec{v}_{i}}{dt} = -\gamma_{t}\vec{v}_{i}+\gamma_{t}v_{0}\hat{p}_{i}-\sum \limits^{N}_{\begin{matrix}j=1\\ j\ne i\end{matrix}}\nabla_{\vec{r}_{i}}u(r_{ij})+\sqrt{ 2k_{B}T_{b}\gamma_{t} }\vec{\xi_{i}}$$ 
	- $$
I \frac{d\omega_{i}}{dt} = - \gamma_{r}\omega_{i} + \sqrt{ 2k_{B}T_{b}\gamma_{r} }\eta_{i}
$$
- [x] understand the **time scales**
	- [x] three different regimes
- [ ] folie mit Suvendus Phasendiagramm vor den Binder cumulant Interpolations ⟹ werte raus schreiben 
- [x] what is my peclet number for my current simulations?
	 - [x] $Pe=\frac{v_{0}}{D_{r}\sigma}\propto \frac{\tau_{p}}{\tau_{c}\varphi}$ 
- [ ] Exponenten neu auswerten -> neu/getrennt abspeichern / backup der alten 
	- [ ] ⟹und gescheit in die Folien packen
- [ ] Quellen für Folien
- [ ] müsste noch den data collapse machen 😒
	- [ ] Folie für die Verteilung von $\rho$ um die Kurtigkeit zu meiner Verteilung zu zeigen, dass $0<\mathcal{B}<1$ für meine Verteilung ist.
	- [x] Verteilung aus alten skripten heraus gekramt und geplottet
	- [ ] es läuft noch eine ld auswertung für m0.05 s05000, 
- [x] Tu Design für Folien 
- [ ] Gescheiten Titel für die Thesis
- [ ] Thesis aufräumen/ neu erstellen
- [ ] Die Benennung "max" und "half" stört mich immer noch...
      ⟹ Aber das konsequent zu ändern 😵‍💫
	- [ ] $▢_{max}$ $\square_{max}$ 
	- [ ]  $▢_{half}$ $\square_{half}$ 
	- [ ] passe abgespeicherten dateinamen an für die plots, muss extra parameter werden
- [ ] Binder cumulant plots bzw überhaupt die x Achsenbeschriftung ... m ist ja falsch. das muss ja $M=\frac{\tau_{M}}{\tau_{R}}$ sein
- [ ] Feng2025 - Critical Motility-Induced Phase Separation in Three Dimensions is Consistent with Ising Universality
- [ ] Schreibe den Order parameter ab sofort als:
      $\mathcal{O}\equiv \left< \rho_{dense} \right>_{L} - \left< \rho_{dilute} \right>_{L}$ 

# old unsorted tasks
- [x] algo changes function and performance test
      ⟹little bugs: Naming of `peakPits` was wrong and the parameter `mainbox` was missing
      ⟹<span style="font-size:100%;color:red;">time reduction by almost a half</span>
      from:
      ![](Pasted%20image%2020251203111544.png)
      to:
      ![](Pasted%20image%2020251203111646.png)
      with the <span style="font-size:100%;color:red;">same result</span>!
	- [ ] longterm test for 112k 0.0680 "06000" max and half
		- [ ] <u>max:</u>
	      before:
	      ![](Pasted%20image%2020251203120842.png)
	      now: value slightly changed ⟹change at 5th digit.
	      ![](Pasted%20image%2020251203120657.png)
		- [ ] <u>half:</u>
		    before:
		    ![](Pasted%20image%2020251203112537.png)
		    now: value also slightly changed ⟹change at 5th digit.
		    here it actually took only the half of time
		    ![](Pasted%20image%2020251203220005.png)
	- [x] remove distData_evalbox before the while loop ⟹ not necessary since new_ysb_Dist is True before the while loop
	      ⟹function test valid! 
- [ ] Why are the values increasing for 112k and 224k for higher inertia? do I need to change something with the values? maybe test with smaller initial height ⟹halfstdDev
	  
- [ ] plot binder cumulant with the new evaluated data
- [ ] continue with slides
- [ ] reeval the exponents
- [ ] changed that `nbins` is dependend on the width of the simulation box factor `nbins=boxwidth*0.5` before 0.3 derived from 600 bins for 224k particles with width ~ 2000  

# <span style="font-size:100%;color:Crimson;">Thesis</span>
~={LimeGreen}Wie strukturiere ich die Arbeit, um diese These argumentativ bestmöglich zu untermauern?=~
~={DeepPink}Welche Gliederung eignet sich am besten dafür, um diese Forschungsfrage bestmöglich zu beantworten?=~

## info sammlung
- largest subfield of active matter is the study of medical applications ~={RoyalBlue}vrugt2025=~
- Feynman’s suggestion that patients may some day be able to “swallow the surgeon”, which takes the form of a microrobot performing a surgery or delivering drugs, and to the movie Fantastic Voyage that shows a miniature submarine traveling through the body ~={DeepSkyBlue}Vrugt2025=~
- medical applications, artificial active particles are often referred to as microrobots, microbots, nanorobots, or nanobots.  A major aim is to use them for targeted drug delivery
- 

## tasks
### general
- [ ] check the snapshots for m=0.05 for 112k 
- [ ] wie sehen die snapshots für 112k nach 10% aus?
- [ ] check if everywhere non-equilibrium is written
### seperate sections
#### history of evaluation methods
- [ ] exponent tabelle separat 
- [ ] was ich zum vergleich des CP zwischen alter und mod methode geschrieben habe, in den normalen text und bilder der beiden $Q_{L}$ nebeneinander
	- [ ] ⟹ es zeigt sich aber beim Lesen der SI, dass für die alte Methode wohl das maximum von $Q_{L}$ stark von der *overall packing fraction* abhängt. Aber wurde es getestet, ob das auch für die veränderte Methode gilt?
	- [ ] In der SI im Abschnitt ~={yellow}**QUALITATIVE JUSTIFICATION FOR CROSSING OF CUMULANTS**=~ wird nochmal stark die Wichtigkeit betont, dass die subboxen in der mitte der liquid phase sind.

1. ~~video zu wissenschaftliche Abschlussarbeiten schauen~~
2. Verlauf von vorherige Arbeiten zur Idee von meinem algo
	1. fast fertig
	2. tabelle mit allen exponenten die in den papern bestimmt wurden
3. inertia vorherige Arbeiten: (zu recent challenges)
	1. mandal
	2. hecht
	3. Su
	4. Feng
4. Gliederung
5. -> mein Algo
6. verwendete formeln + meine simulationen - aus dem report holen
7. meine aktuellen ergebnisse
8. problematik!
9. ausblick
10. theorie - wirklich auf die Arbeit zu geschnitten
	1. phase transition 
	2. what are critical exponents 
		- Für die Theorie dazu einfach nach den VL von ~={Magenta}Prof. Sutapa Roy =~richten [Link zur Playlist]( https://www.youtube.com/results?search_query=Dynamics+of+Confined+Fluids+close+to+Phase+Transitions+%7C+Prof+Sutapa+Roy+%7C+)
		- when are they relevant 
		- universality
		- renormalization group (nicht im Vortrag)
			- nochmal verstehen ⟹ den ~={DeepPink}abgetippten Wikiartikel=~ 
			- Kommen ~={RedRed}durch die RG=~ die Fixpunkte in das System oder sind die nicht schon da? 
			- ⤷ also der ~={Tomato}Fixpunkt um den Phase transition=~ point ist doch eigentlich immer da?
			- ⟹ Skaleninvarianz am phase transition point
			- ⤷ deshalb ~={LawnGreen}funktionieren=~ solche Sachen wie die Analyse des Binder Cumulant
		- 
	- lammps 
11. titel + abstract
12. create simulation programm in den anhang
13. quellen
14. zinos thesis lesen, um abzuchecken
15. -> arbeit aritra schicken
16. Vortrag
## talk

- fotos von
	- bakterien
	- flocks
	- janus particles
	- self-propelled medical micro robots

1. Thank you for having me. Sorry I have constant brain fog - my brain is so full and empty at the same time - these days so don't be mean about me, that I need to read what I want to say.
2. I often really don't know what is wrong with me.
	1. But that's wrong,
	2. The problem is i know what's wrong with me most of the time. 😅
	3. But it's too hard for me to explain in few words 
	4. I guess the easiest way to say what's wrong with me "that i try to explain what's wrong with me and why i so often can't"
3. At least I can say I am not healthy in many ways and I am recovering too slowly.
	1. But I am done with not meeting my obligations and test the patience of all again and again 
	2. I said that I will give my proposal defense talk today so I give some despite having not handed in I my proposal and despite I am even not finished with the preparation of this talk.
	3. I’ll take this time slot, and we’ll see what we can make of it.
	4. At least consider this as a wrap up of my "work" and than saying farewell.
4. One thing I can say that I have learned and I hope finally I have finally embodied somehow in my emotions and my existence.
	1. Don’t be driven by fear and anxiety; instead, be led by curiosity and fascination
	2. And bother too much about "how should I do this, this is to much I don't know where to start." 
	3. Just do it and start somewhere 
	4. And don't focus to much on things you believe you can't do.
5. So now to my actual talk 
	1. The topic of my work is: 
	2. Finite size scaling analysis of underdamped Brownian particles
6. 

7. What is active matter?
	1. Drei Zitate aus dem paper what is active matter 
	2. Active brownian particles 
8. Why interia? What's the matter with intertia?🤣
	1. Why not intertia?
		1. Overdamped equations are much easier?
		2. Where is the justification:
			1. We observe particles from several nm to several micrometer 
			2. Low Reynolds Number Regime: micrometer-sized particles in a liquid (colloids), the motion occurs at very low Reynolds numbers, where viscous forces (drag) dissipate energy much faster than the inertia can maintain motion.
			3. Time Scale Separation: Overdamping is justified when looking at long-time behavior, specifically for times $t \gg \frac{m}{\gamma}$(where $\gamma$ is the friction coefficient). The rapid inertial relaxation means that the particle reaches a diffusive regime almost immediately, rendering the acceleration irrelevant
		3. Applicable Scenarios: Microscale colloids in liquids, biological agents inside cells, and simulations where short-time ballistic behavior is not the focus.
	2. Why inertia?
		1. Failure Cases: Overdamping fails for macroscopic particles, microparticles in gases (low viscosity), or during the very early "ballistic" phase of a particle's motion where the trajectory is not yet dominated by collisions.
		2. Interesting cases: 
			1. Phase transitions
			2. Active Refrigerator 
9. What is critical phenomena and finite size scaling analysis ~={MediumTurquoise} Mal in die Folien von nico von letztem Jahr schauen=~
	1. What's a phase transition?
	2. A change in order parameter in dependency of a control parameter?
	3. What is an order parameter?
	4. Some usually extensive physical quantity. It depends on the system you want to describe and how you classify order in a phase transition.
		1. <u>Liquid gas transition</u>: the change in density in dependency of the temperature 
		2. <u>Ferromagnetism</u>: change of magnetization in dependency of temperature and an external field
		3. <u>MIPS in Active matter </u> the density distribution of the particles - the average density difference between the dense and the dilute phase, in dependency of  different parameters,
			1. the packing fraction, 
			2. for **abp** the activity strength or péclet number. 
			3. other particle models like AOUP, the persistence time of the self-propulsion speed is tuned.   
			4. On top of it you can apply various interactions 
			5. Or in my case turning the particles mass and therefore the inertia up from overdamped to underdamped regime.
		4. Phase transitions can be classified 
			1. Mainly in first and second order phase transition 
			2. First discontinuous change of the microscopic quantity 
			3. Second order continues change 
			4. <u>Ehrenfest</u>: order of the lowest derivative of the gibbs enthalpy G that has a discontinuity while crossing the coexistence curve
	5. Critical phenomena 
		1. As it names states it concerns about critical and therefore continuous phase transitions
		2. <u>Landau</u>: expansion of the free energy density near a continuous PT in terms of an order parameter
		3. what is happening in the vicinity of a continuous phase transition?
			2. small changes in values of external field lead to large changes in order parameter or there are large fluctuations associated with it 
			3. the correlation length $\xi$ - the length on which interactions correlate, the same yields for fluctuations - goes to infinity at the critical point point
			4. equilibrium: response and fluctuations are infinitely connected: fluctuation-dissipation theorem
			5. therefore other quantities like the susceptibility $\chi$ goes to infinity
			6. Description of these quantities by power law in terms of reduced control parameter $\tau=1-\frac{T}{T_{c}}$ 
			7. mean field theory crashes
			8. $\xi \propto |\tau|^{-\nu}$
			9. order parameter $\mathcal{O}=$$M_{S}\propto |\tau|^{\beta}$
			10. susceptibility $\chi \propto |\tau|^{\gamma}$
			11. other quantities like the specific heat $C$ or the compressibility $\kappa$
		4. there are mean field values for these exponents, but you never find them in experiments
			1. moreover fascinating it appeared universality of these exponents found in experiments and the scale invariance
			2. systems. with the same symmetry + same numbers of order paramter + interaction range ⟹same values for the exponents
			3. they are the same for physically complete different systems
			4. the exponents found for the Ising magnet and the liquid gas transition are the same
			5. also for the xy magnet model and a superfluid
	6. scaling theory
		1. generalization of the features near the CP
		2. depiction of the singular part of the free energy with a power law $$
f_{\text{sing}}(\tau,h)=|\tau|^{2-\alpha} \hat{f}_{\pm}\left( \frac{h}{|t|^{\beta \delta}} \right)
$$
		3. ⟹critical exponents are not independent -> scaling relations
	7. finite systems where you can't assume that they are thermodynamically large, like in our simulations
		1. the correlation length which is the indicator/reason of the singular behavior of other quantities, is limited by the systems minimal expanse $L$. At the CP the correlation length can be maximal equal to it $\xi \approx L$
		2. The singularities are rounded off -> this is described by scaling functions $\hat{f}\left( \frac{\xi}{L} \right)$ as function of the correlation length
		3. so quantities near a CP are displayed by a power law with its exponent multiplied by the scaling function $\mathcal{O}(\tau,L) = |\tau|^{-\zeta_{\mathcal{O}}}\hat{f}\left( \frac{\xi}{L} \right)$⟹$\mathcal{O}(\tau,L) = L^{-\zeta_{\mathcal{O}}/\nu}\tilde{f}\left( |\tau|\left( \frac{L}{\xi} \right)^{1/\nu} \right)$ 
10. Mention the behavior of $\chi$ in Maggi21
### text memory
- *For underdamped Brownian particles.*
  *Inertia is the control parameter.*
  *The measured quantity is the density fluctuation of the particles inside boxes placed at the peaks and pits of the horizontal density distribution of the simulation boxes*
### intro
- what is active matter?
	- descriptions von dem paper what's active matter - > anhand den verschiedenen Definitionen - non equilibrium 
	- verschiedenste Bilder 
		- flocking
		- Regime?
		- pattern building 
- einfachste Modelle 
	- abp / abp+?
	- Formeln immer trocken Modelle ⟹ fluid fließt in noise term und Reibung ein, sowie Interactions 
- overdamped normal Fall warum? (Auch in die Thesis )
	- regime? Ne 
	- Teilchen in der Regel klein und leicht im Vergleich zum ReibungsWiderstand 
- what is mips, how does it occurs in case of real basic active matter
- underdamped
	- als motivation/introduction
	- bisherige Forschung 
		- inertia vorherige Arbeiten: (zu recent challenges)
		- mandal
		- hecht
		- Su
		- Feng
	- Warum interessant? ~={RedRed}(Thesis)=~
	- was ist anders bei Mips Erklärung und Bild von suvendus paper
	- Kuriositäten ~={RedRed}(Thesis)=~
		- Kühlschrank ~={RedRed}(Thesis)=~
		- suvendus Erkenntnis mit der Temperatur ~={RedRed}(Thesis)=~
		- ~={Gold} nur=~  ~={RedRed}(Thesis)=~ paper mit den density distributions -> schulter ⟹habe ich ja auch gesehen 
- phase transition 
- what are critical exponents 
	- when are they relevant 
	- universality
	- renormalization group (nicht im Vortrag )
- lammps 
## to do
- [ ] ~={Magenta}explain the meaning of the binder cumulant as the deviation of the gaussian shape=~
- [ ] liste die paper bzgl. der universality class auf <span style="font-size:100%;color: limegreen;">einiges in Dittrich aufgelistet</span>
- [ ] vom siebert den einstieg in den box algo schreiben. bzw. unter <span style="font-size:100%;color: cyan;">Evaluation methods to determine critical points in non-equilibrium systems</span>
- [ ] Folien durch gehen und damit den groben fahrplan / struktur machen
- [ ] Den Weg vom der ursprünglichen Box eval methode zum Box algo beschreiben.
	- [ ] Erstes paper
		- [ ] warum haben die diesen eingeführt
		- [ ] was war die Idee 
		- [ ] was das Vorgehen 
		- [ ] was ist zu beachten und wichtig
	- [ ] box-algo
		- [ ] Warum waren die Veränderungen nötig
		- [ ] was war die problemstellung bei der ursprünglichen Methode? Also was hat nicht funktioniert?
		- [ ] Was ist die idee und wie funktioniert er?
			- [ ] im report schauen
			- [ ] in den Folien schauen
- [ ] Damit meine Arbeit beschreiben. strickt anhand der Folien
- [ ] Probleme des Algorithms beschreiben 
- [ ] Dann meine Introduction passend dazu schreiben
- [ ] Dann den theoretical background
- [ ] dann das create simulation program
- [ ] create simulation program auf dem cluster hochladen und beschreiben

## toc
- [ ] Motivation / Introduction
- [ ] basics / Phasetransition
- [ ] Recent challenges (current papers / researches)
	- [ ] what are the recent discoveries concerting the universality class
		- [ ] siebert
		- [ ] dittrich
		- [ ] maggi
		- [ ] Feng
	- [ ] inertia
		- [ ] mandal
		- [ ] hecht
		- [ ] Su2021
		- [ ] Feng2025
## general
- [ ] gescheiten Titel überlegen ⟹ criticality/universality of underdamped brownian particles non equilibrium 
- [x] Unterschrift und Datum ändern
- [ ] Date of submission
## outlook
- [ ] evaluating 112k and 224k with different box sizes
	- [ ] max
	- [ ] half
	- [ ] third
	- [ ] forth
	- [ ] fifth
	and compare the Binder cumulants since this is also a change of the probing system size.
- [ ] change the algo in ~={DeepPink}need to eliminate the phase contributions=~ to:
	- [ ] finish / reinvestigate approach of july 2025 where 
		- [ ] the peaks are filtered after the one-sided standard deviation of the  height of the highest peak inside the rectangle box (the center of the standard deviation isn't the average height but the peak or the second moment with $c=\text{peak}$)
		- [ ] and afterwards after the standard deviation of the x-position around the highest peak
		- [ ] and than the average of these peaks are calculated
		- [ ] this approach is independent of the size of the outer rectangle box
		- [ ] if the threshold for the peaks and pits are high, the total number of eval boxes are reduced, but not the quality of the placement is affected
		- [ ] but there must be still a filter for 
			- [ ] if the the eval square box is intersecting with the outer rectangle
			- [ ] if dense and dilute boxes are overlapping, the threshold value for the width of the outer rectangle box is reduced
				- [ ] or we are going back to the oldest approach that the rectangle box for the dilute phase is depending on the rectangle box of the dense phase. This avoids always the overlapping of the dilute and dense square boxes and also the overlapping of dense and dense and dilute and dilute boxes
				1. here the best approach is to use the stdv for the threshold for peak/pit
				2. the threshold is raised if the rectangle boxes are too narrow so that the square boxes aren't able fit in
				3. the threshold is lowered if there are to few square boxes. (which shouldn't be the case)
				- here is no quality management or overlapping / collision management necessary


# <span style="font-size:100%;color:LimeGreen;">Latex Formel Sammlung</span>
- $Q_L(T)=\frac{\Braket{\mathcal{O}_L^2}_L^2}{\Braket{\mathcal{O}_L^4}_L}$ 
- $\Braket{\dots}_L$ 
- $\mathcal{H}_{\text{Ising}}=-\sum_{l\ne l'}^{} J_{ll'} S_{l}S_{l'}-H\sum_{l}^{}S_{l}$ 
- $\mathcal{H}_{\text{Ising}}=-\sum\limits\limits_{l\ne l'}^{} J_{ll'} S_{l}S_{l'}-H\sum\limits_{l}^{}S_{l}$ 
- $\sum\limits_{i=1}^{N}$ 
- \href{https://journals.aps.org/pre/abstract/10.1103/PhysRevE.98.030601\#supplemental}{supplement material} 
- $p_{\text{subbox}}=L^{\beta/\nu} \hat{p}\left\{ \left( \rho-\rho_{\text{crit}} \right)L^{\beta/\nu},L^{1/\nu}\tau \right\}$ mit $\tau=1-\frac{T}{T_{c}}$
- $p_{\text{subbox}}^\text{liquid}(\rho)\propto \exp \left\{ -\left( \rho-\rho_{\text{liquid}}^\text{coex} \right)^{2}L^{2} / \left( 2k_{B}T\chi_{\text{eff}}^{L} \right) \right\}$
- $p_{\text{subbox}}^\text{vapor}(\rho)\propto \exp \left\{ -\left( \rho-\rho_{\text{vapor}}^\text{coex} \right)^{2}L^{2} / \left( 2k_{B}T\chi_{\text{eff}}^{L} \right) \right\}$
- packing fraction
	- $\varphi=N\pi\sigma^{2} / (4L_{x}L_{y})$
	- $\varphi=\frac{N\pi\sigma^{2}}{}$

# Masterplot
multiply the data of the observable (binder cumulant, order parameter,  susceptibility) with the scaling factors of the observable. $L^{\zeta_{\mathcal{O}}/\nu}$ 

> [!NOTE] Maggi21
> Using the finite-size scaling ansatz, we assume that a generic observable $\mathcal{O}$ near the critical point behaves as $$
\mathcal{O}=L^{\zeta_{\mathcal{O}}/\nu}\left[ F_{\mathcal{O}}\left( L \xi^{-1} \right) + O \left( L^{-\omega},\xi^{-\omega} \right)  \right] 
$$, where $\zeta_{\mathcal{O}}$ is the critical exponent associated with the observable $\mathcal{O}$, $F_{\mathcal{O}}$ is a universal finite-size scaling function and $\omega$ is the power of the (subleading) correction-to-scaling exponent.

![](Pasted%20image%2020260222131207.png)
- use the correct $M_{C}$ and correct exponents
- [x] automate show exponent value in masterplot 
	- [x] adjust masterplot template so that it reads the header from the csv file
	- [x] add the values used for the masterplots into the slides
- [x] masterplot below the general plots
- [ ] replot $\mathcal{B}$ of the "ABP" with the general plot template
- plot the orderparameter
	- [x] max
	- [x] half
- [x] add L to the ledgend
- plot bindercumulant
	- [x] max
	- [x] half
- plot $\chi$
	- [x] max
	- [x] half
# Important guidline to fokus on
- <span style="font-size:120%;color:red">Don't touch the box algo anymore!</span>
- <span style="font-size:120%;color:red">determine the Phase transition point</span>
	- use the latest data I have ⟹ of half avg and max avg
- <span style="font-size:120%;color:red">determine $\nu$ with the derivative of $\mathcal{B}$</span>
- [ ] Browser Uni aufräumen
- clean the proposal
- sort the introduction and theorie
- explain the algorithm at it's current state and it's flaws and also the ways to refine it
- [ ] clean the folder **sqaureboxEvaluation**
- [ ] renaming max to half and half to forth...
- make / clear snapshots with plots with the latest algo. ==am Windows PC==
	- **new folder**
	- **clear naming**
	- **neat** / **oversee-able**
	- 112k
		- [x] avg max
			<!-- - [ ] 0.06 -->
			- [x] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [x] 0.068
			<!-- - [ ] 0.069 -->
			- [x] 0.07
		- [x] avg half
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
	- 28k
		- [x] avg max
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
		- [x] avg half
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
	- 7k
		- [x] avg max
			<!-- - [ ] 0.06 -->
			- [ ]  0.065 
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
		- [x] avg half
			<!-- - [ ] 0.06 -->
			- [ ] 0.065
			<!-- - [ ] 0.067 -->
			<!-- - [ ] 0.0675 -->
			- [ ] 0.068
			<!-- - [ ] 0.069 -->
			- [ ] 0.07
	- Density distribution **exemplarisch** anhand von 112k für 
		- [ ] 0.065
		- [ ] 0.068
		- [ ] 0.07
- [x]  <span style="font-size:120%;color:orange">write down the scaling formula for the order parameter</span>
	- <span style="font-size:120%;color:orange">determine $\beta$</span>
- [x] git checkout to the ***last*** **phase-peak-pit-height-tune-algo**
- [ ] compare the box placement for stdDev and halfstdDev
- [ ] evaluate binder for 28k particles with halfstddev and compare the plot with stdDev
	
# Box Algo
ich frage mich, ob ich nicht, wenn ich die ~={yellow}kästchen kleiner=~ mache und mehr und ~={orange}mehr auf die peaks/pits=~ schiebe und den ~={LawnGreen}interfaces ausweiche=~, ob ich dann nicht den ~={DeepPink}fluktuationen ausweiche=~?
- [ ] ich muss definitiv die peaks filtern um die mitte des größten peaks. das würde die ergebnisse definitiv verbessern
- [ ] make an exception handling for the case if there are no dense/dilute boxes
- [ ] put the box evaluation on the cluster and evaluate the data there
- [ ] ask kayro for rights to push to upstream
- [x] kann den prozess beschleunigen, in dem ich das überprüfen der phase width aus filter new peak pit auslagere und distdata-evalbox, get_peak_pit, sowie filter peak_pit nur laufen lasse, wenn height_mul geändert wurde. 
      Hat geklappt und ist viel schneller / doppelt so schnell
## peak pit width tuning
- [x] did a new strange branch... from phase-peak tune...
- [x] need to branch it...
- did a combination of height and width mul variation in combination with an alternation in varying this value. Also increased the reduction of the width to get less loop breaks / faster results
- changed bins from 500 ⟹ 600 ⟹ $\text{nbins} = \text{boxwidth} \cdot 0.5$ (so it depends on the system size)
- atm the pit/peak height isn't altered (at least it has no direct effect) for overlapping boxes only if there are no dense/dilute boxes left, since the pit/peak height was altered indeed but the density distribution is not reevaluated because the boolean `new_ysb_Dist` isn't toggled True again. 
- [ ] the best result for placing the squares would be to average only over the peaks in the standard deviation range of the highest peak (part of the other branch)
## Evaluate
- [x] reeval at 224k seed 05000 m 0.067
- [x] Save the box size of the evaluated boxes

## finite-size-scaling_phase-peak-pit-height-tune-algo
new branch ⟹ fss_ppphta_ebox-fit-in-pp
- [ ] ==clean the code from old unused stuff== delete old code
	- [x] ==make a backup before cleaning==
	- [ ] filter_same_pits
	- [x] remove commented code in finite_size_scaling
	- [ ] remove keep_pbc in the middle
	- [ ] remove dist_pbc
	- [ ] substitute pbc everywhere
	- [ ] remove commented code from  `evaluate`
	- [ ] move the auxiliary functions out of the main code...
- [x] quality management with correct distance measurement
- [ ] filter_same_pits
	- [ ] check if distance between pits is wide enough that the evaluation box fits in
	      ![[Pasted image 20251024224645.png]]
	    It should lead to that in too "narrow" phases no evaluation squares are placed. But it does not provide that the box is complete inside the phase and also does not prevent overlapping with evaluation boxes in dilute phases, if they are placed at the boarder of a rectangle box.
	    Overlapping is only prevented, when the square is placed in the middle of a rectangle box.
- [ ] ==problem:== evaluating the particle number of split eval boxes ( those which overlap over the mainbox border)  ⟹ particles at vertical border between the left and the right split box are counted twice atm!
	- [x]  ⤷ Don't split squares in `subbox_to_square_withpeak_dilute_dense_new` split only, when  creating the plotting rectangles.
	- [ ] adjust `box_to_rectangle` / `box_to_rectangle_list` <span style="color:red"> needs another name ==not== rectangle</span>
	- [ ] adjust sorboxes ⟸ because there are no lists of squareboxes anymore
- [ ] add a dilute vs dense eval boxes counter to quality management

# Jupyter
- [ ] test new code / cleaned code, after square_box split was moved to  box_to_rectangle
- [ ] compare the densities / particle numbers of squarebox split and not split
- [ ] **Dict to csv**
    ```python
    import csv  
    
    cars = [     {"Brand": "Toyota", "Model": "Corolla", "Year": 2020},     {"Brand": "Honda", "Model": "Civic", "Year": 2019},     {"Brand": "Ford", "Model": "Focus", "Year": 2018} ]  
    
    # CSV file name 
    csv_filename = "cars.csv" 
    
     # Define the field names (headers) 
     fieldnames = ["Brand", "Model", "Year"]  
     
     # Writing to CSV 
     with open(csv_filename, mode='w', newline='') as file:   
			     writer = csv.DictWriter(file, fieldnames=fieldnames)
			     writer.writeheader()  # Write header row    
			     writer.writerows(cars)  # Write data rows   
    ``` 

- [ ] https://pandas.pydata.org/docs/reference/api/pandas.read_csv.html
	- [ ] https://pandas.pydata.org/docs/reference/api/pandas.unique.html
- [x] sort determine CP
## Juypter on cluster
the reason why it didn't find amep was that I choose the <span style="font-size:100%;color:red;">wrong folder depth</span>.
I choose `amep/amep`instead of `amep/`

### sbatch script
```bash
#!/bin/bash -l

#SBATCH --chdir /home/lwalter
#SBATCH --partition=standard
##SBATCH --partition=gpu
##SBATCH --nodelist=cpu11
#SBATCH --nodes=1
#SBATCH --ntasks=1
#SBATCH --cpus-per-task=1
#SBATCH --job-name="amep"

module load anaconda3

/home/lwalter/.conda/envs/phasetransition/bin/jupyter-notebook --no-browser --port=8081
```

![[Pasted image 20260303143705.png]]
![[Pasted image 20260303172550.png]]
![[Pasted image 20260303172607.png]]
`jupyter-lab --no-browser --port=portOut`
```bash
ssh -v -L portIn:cpuXX:portOut 192.168.211.2 -N
```
- `portIn` is the port received by the browser with `localhost:portIn` or `127.0.0.1:portIn`
- `portOut` is the port used to forward from the sending host 
```bash
ssh -v -L 8891:cpu11:8081 192.168.211.2 -N
```

`-v`is only for debugging, you can omit it.
## Connect to CPU2
You have to be logged-in to the cluster first.
```bash
ssh cpu02
```
Connect to Jupyter-lab via:
```bash
ssh -L 3733:127.0.0.1:8082 192.168.211.2 -N
```
The current working python environment is <span style="font-size:100%;color:red;">venv</span>
```bash 
source venv/bin/activate
```
Start juypter -lab
```bash
 jupyter-lab --no-browser --port=8082
```
# Evaluate
## Determine CP
linear approximation optimization with aritras interpolation method
- [x] Read Aritras Code and ask if something isn't clear
	- [x] "data_phase_transition_with_errors.csv" ⟹ how did he get the errors
	- [x] what are **unique L values** ⟹ a designated system size 
	      With the method `.unique()`you can filter rows for certain values.
	- [ ] Udl ⟹ is the Bindercumlant of mean largest cluster length $d_l$: $\mathcal{B}(d_l)$
	      In my case $d_l$ is $\rho$ of the evaluation boxes: $\mathcal{B}(\rho_\text{box})$
	- [ ] Udl_se means? ⟹ I guess it is the error
	- [x] What does `from scipy.interpolate import splrep, splev`?
		- [ ] splrep(_x_, _y_, _w=None_, _xb=None_, _xe=None_, _k=3_, _task=0_, _s=None_, _t=None_, _full_output=0_, _per=0_, _quiet=1_)[[source]](https://github.com/scipy/scipy/blob/v1.16.2/scipy/interpolate/_fitpack_py.py#L164-L305)
		      Find the B-spline representation of a 1-D curve.
		- [ ] splev(_x_, _tck_, _der=0_, _ext=0_)[[source]](https://github.com/scipy/scipy/blob/v1.16.2/scipy/interpolate/_fitpack_py.py#L308-L395)
		      Evaluate a B-spline or its derivatives.
	- [x] why `{py} subset_df = data_frame[data_frame['L'] == L_value]`
	      `{py} subset_df['Udl']` picks a column of a csv file
	- [ ] `{py} result = minimize(lambda params: objective(params, curves_data, curves_se_data), initial_guess, method='BFGS')` 
		- [ ] <u>BFGS</u> Minimization of scalar function of one or more variables using the BFGS algorithm.
		       https://docs.scipy.org/doc/scipy/reference/optimize.minimize-bfgs.html#optimize-minimize-bfgs
		       
		    n numerical optimization, the Broyden–Fletcher–Goldfarb–Shanno (BFGS) algorithm is **an iterative method for solving unconstrained nonlinear optimization problems**. Like the related Davidon–Fletcher–Powell method, BFGS determines the descent direction by preconditioning the gradient with curvature information.
		       https://en.wikipedia.org/wiki/Broyden%E2%80%93Fletcher%E2%80%93Goldfarb%E2%80%93Shanno_algorithm
Evaluate a B-spline or its derivatives.
`{cpp} printf("\nHello World!")`
Find the B-spline representation of a 1-D curve.
- [x] how do I export dicts to csv files
- [x] Export the data from
	- [x] binder_max_avg_dicts
	- [x]  binder_half_avg_dicts
	      `omit 3.5k and 7k `
- [ ] apply the optimization⟹decide by the optimization error which box size to choose
- [x] evaluate the derivative of the binder cumulant
## order parameter
- [x] determine order parameter $\Braket{\rho_\text{dense}}_{L}-\Braket{\rho_\text{dilute}}_{L}$ ==Feng2025==
      ![[Pasted image 20251103233523.png]]
- [ ] plot it
- [ ] write down the scaling function for the orderparameter
- [ ] determine $\beta$
## susceptibility
- [ ] determine the susceptibility $\chi$ ![[Pasted image 20251103233452.png]] $\chi \equiv \left( \frac{L^{3}}{v_{D}} \right) \frac{\Braket{\Delta \phi^{2}}_{L}}{\Braket{\phi}_{L}}$  <br> With $v_{D}\equiv\frac{\pi d^{3}_{hs}}{6}$ the volume of a single particle. With $d_{hs}=2^{1/6}\sigma$ $v_{\text{sphere}}=\frac{4}{3}\pi r^{3}=\frac{4}{3}\pi \left( \frac{d_{hs}}{2} \right)^{3}=\frac{4}{3 \cdot 8} \pi d_{hs}^{3}=\frac{\pi}{6}d_{hs}^{3}$   The susceptibility $\chi$ is maximal at the CP
      ![[Pasted image 20251103235225.png]]
- [ ] translate $\chi$ in $2D$ <br> $\chi \equiv \left( \frac{L^{2}}{v_{D}} \right) \frac{\Braket{\Delta \phi^{2}}_{L}}{\Braket{\phi}_{L}}$   With $v_{D}\equiv\frac{\pi d^{2}_{hs}}{4}$  the volume of a single particle. With $d_{hs}=2^{1/6}\sigma$  <span style="color:red;font-size:100%;">valid?</span> in 2D?<br>
- [ ] get $L$: in my case it is the length of the evaluation box.
	- [ ] need to retrieve it from calculate binder from sub box 
	- [ ] ==take care== $L$ is ==different== for *max* and *half*
	- [ ] create a column $L_{\text{evalbox}}$  
- [ ] plot $\chi$
- [ ] determine $\gamma$ 
- [ ] 
$\text{boxRatio}=R=10$
$\text{fillRatio}=\phi=0.5$
$L_{yHalf} = \sqrt{\left( \frac{N\cdot\pi\cdot\sigma^2}{(4\cdot R \cdot \phi)} \right)}/2$
$L_{xHalf} = R\cdot L_{yHalf}$
$\phi = \frac{N \cdot \pi \cdot \sigma^2}{4\cdot R\cdot2\cdot L_{yHalf}^2}$
### box boundaries xlo,xhi,ylo,yhi,zlo,zhi L_y=sqrt(N Pi sigma²/(20 phi))
region 	box block -${LxHalf} ${LxHalf} -${LyHalf} ${LyHalf} -0.5 0.5	
# Simulate
## current create-sim command
```shell
create-simulation_mod_p.sh -er -pr "equilibrateMaster_mod_p.in" "productionMaster_mod_p.in" "PE,55" 3500 "m" -3 .04 .04 .01 . 05000 -ts 4 -ss -sc 8

```
## other
![](Pasted%20image%2020251211005701.png)
<span style="font-size:120%;color:green"> Atm there is enough simulation data</span>
- [ ] 224k
	- [ ] .04 
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .045
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .05 
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .055 
		- [x] 5 eq
		- [x] 5 pr
		- [x] 4 eq
		- [x] 4 pr
	- [ ] .06 
		- [x] 3 eq
		- [x] 3 pr
	- [ ] .062 
		- [x] 3 eq
		- [x] 3 pr
	- [ ] .064 
		- [x] 3 eq
		- [ ] 3 pr
	- [ ] .065 
		- [x] 3 eq
		- [ ] 3 pr
	- [ ] .0676 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
	- [ ] .0677 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
	- [ ] .0678 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
	- [ ] .0679 
		- [x] 4 eq
		- [ ] 4 pr
		- [x] 5 eq
		- [ ] 5 pr
## Create-sim
- [ ] add some something like a progress bar / time estimation
- [ ] a checker which simulations are finished 
- [ ] a little GUI, where you can see all the data you already have
- [ ] modify it that it does not run on the cluster... it need to connect via sftp to do the stuff... would be better...
- [x] add dependency to create-simulation - dependency of production run to equilibration run
	-  Hier ein Beispiel: 
```{SLURM}
#!/bin/bash
jid1=$(sbatch --parsable impact_sol_${NUM}1.sh)
jid2=$(sbatch --parsable --dependency=afterok:$jid1 impact_sol${NUM}2.sh)
jid3=$(sbatch --parsable --dependency=afterok:$jid2 impact_sol${NUM}_3.sh)
echo "Stage 3 jobs submitted: $jid1 → $jid2 → $jid3"
```

-  Jeder Job wird zugewiesen, z.B. jid1, jid2, ... und der folgende Job muss auf das OK des vorherigen warten, d. h. dass er abgeschlossen ist. Das wird gemacht mit `--dependency=afterok`.
	- There has to be the possibility to set up equilibration and production at the same time where the number of cores for the equilibration run will be divided by 8 (make sure that its an integer)
	- <span style="font-size:200%;color:gold;"> soooo geil dependency funktioniert</span>
- [ ] ask why the equilibration run is still so slow in comparison to the production run by $ts=1^{-4}$ 

# Read
- [ ] Feng2025~Theory for the anomalous phase behavior of inertial active Brownian particles
	- [ ] + Supplement

# Report
<span style="color:red" > finish the Slides today </span>
- L corresponds to the particle number $\#N$ through: 
- $L_{yHalf} = \sqrt{\left( \frac{N\cdot\pi\cdot\sigma^2}{(4\cdot R \cdot \phi)} \right)}/2$
- $L_{xHalf} = R\cdot L_{yHalf}$
- $\phi = \frac{N \cdot \pi \cdot \sigma^2}{4\cdot R\cdot2\cdot L_{yHalf}^2}$
- describe $M=\frac{\tau_{M}}{\tau_{R}}$ which resembles our mass "m"
## Slides
### Vertical Split
- Why is the resolution of the snapshots of the half sized boxes worse
- $\left< \text{NP} \right> - \left< \text{NP}^{2} \right>$ 
- [ ] Slides:
	- [ ] 112k different m: .06, .065, .067, .068, ~~.069~~ ⟹.07
		- [ ] pictures of Δy Density Distribution 
		- [ ] pictures for avg 
		- [x] pictures for peak 
		      <span style="color:gold;font-size:100%;">⟹ the peak evaluation is depreciated for now!</span>
		- [ ] square size max
		- [ ] square size half
- [ ] add the current results for CP and $\nu$ 
- [x] Fitting $\mathcal{B}$ ⟹ CP:
	- [ ] show CP in ledgend
	- [ ] max evalbox size
		- [ ] replot the non cut out plot with legend and higher smoothing
	- [ ] half evalbox size
		- [x] replot non cut out with legend
		- [x] replot cut out with legend
- [x] Fitting $\nu$ 
- [x] Fitting $\beta$
- [x] Fitting $\gamma$ 
- [ ] $\mathbb{M}=\frac{\tau_{d}}{\tau_{p}}$

# Test note
- [ ] this is a test note $\sqrt{x}$ 
$$\frac{ \partial f }{ \partial x }
$$
$\partial \Delta$
$\frac{ \partial f }{ \partial 2}$

$x^{2}\frac{ \partial g(x) }{ \partial x }$

```mermaid 
%% --- %%
%% config: %%
 %% layout: elk %%
 %% look: handDrawn %%
 %% theme: dark %%
%% --- %%
flowchart TB
	a[Tenant admins] 
	a-->SubRoles
	
	subgraph SubRoles [Sub Roles]
		direction LR
		b[Playbook admins]
		c[Playbook managers]
		d[Playbook global viewers]
		b-->c
		c-->d
	end
```
# New Note
1. First 
2. Second 
3. $\frac{ \partial y }{ \partial x }$ 
4. $t_{7}$ ❃☩⚔☠✠⤭✼⛥꙳

# MIPS
- competition between the time scale of reorientation and collision
- overdamped ⟹ no reason for bouncing back
- underdamped ⟹ the bounce back
- Reentrance effekt for higher Pe with higher masses 
  ![[Pasted image 20251118121845.png]] (Hecht2021)
- Something (Weaks-chanderler potential) is hard to parallelize 
# JC / group meeting
## 25-04-28 palash
**Inferring phase transitions and critical exponents from limited observations with thermodynamic maps**:
- characterizing generic attributes of phase transitions from very limited observations 
- Our approach is called thermodynamic maps 
- combines statistical mechanics and molecular simulations with score-based generative models. 
- learning the temperature dependence of arbitrary thermodynamic observables across a wide range of temperatures
- calculating phase transition attributes such as 
	- melting temperature
	- temperature-dependent heat capacities
	- and critical exponents. 
- ~={Gold}infer=~ the ~={LawnGreen}ferromagnetic phase transition of the Ising model,=~ including temperature dependent heat capacity and critical exponents, despite ~={DeepPink}never having seen samples from the transition region=~
- 



### general
- <u>forward process</u>
	- applying gaussian noise until for example an image vanishes
	- In machine learning, specifically within Diffusion Models, the forward process (or forward diffusion) is a fixed, non-learnable procedure that gradually degrades data quality by adding noise until it becomes indistinguishable from Gaussian noise.
	- from this you get the noise protocol to get a certain for example image from noise
	- we try to learn $\epsilon$ by applying gaussian noise to a langevin equation until its completely gaussian
	- $\mathcal{L}(\theta)=E_{x_{0}\sim p(x),t} \left[ \left|| s_{\theta}(x,t)-\nabla_{x} \log p_{t}(x_{t}|x_{0})   \right||^2 \right]$
	- $x_{t}=\sqrt{ 1-\beta_{t} }x_{0}+\sqrt{ \beta_{t} }\epsilon$ it's an langevin equation
	- ⤷ $p_{t}(x_{t}|x_{0})=\mathcal{N}(\sqrt{ 1-\beta_{t} }x_{0},\beta_{t})$
	- ⤷ $\nabla_{x}\log p_{t}(x_{t}|x_{0})= \frac{\sqrt{ 1-\beta_{t} }x_{0}-x_{t}}{\beta_{t}}$
	- $\nabla_{x}\log p_{t}(x_{t}|x_{0})=-\frac{\epsilon}{\beta_{t}}$ 
- like a decryption problem:
	- it's like if you know the signal to decrypting the key
	- or decrypting without knowing the key
	- but you cannot use it for decrypting, because you would have to train for ex. 10k encryptions with the same encryption key
## 26-04-07
- <u>intention:</u> exchange about the own usage
	- I didn't use it that much in past, but try to be more open
		- but I'am always careful and skeptical 
		- since it made me insecure, because of it seams in the form and from the formulations quiet sensible, but in the details were so many flaws.
			- this created a great insecurity in me, since I cannot trust in it and have to check twice
			- and also have to check what I have already written and thought trough, since I do not know and cannot check every particular change and makes it more vague why it works or why not, its so much trust and guessing in some points
		- in some chases it produces errors in texts or code that weren't there before
		- and I had no brain capacity to check it, and made me insecure about mistakes
	- checking for translations and formulations
	- learning language
	- In past to find out how to do/solve things.
		- I had to use it for work a lot, since my employer/principal expected it from me
		- give an overview for a new field I have to explore. simple step by step guides
	- if you use google as a search engine than you always stumble about the small summaries
		- I read them always but I found so often mistakes
	- I recognized extrem sycophancy 
		- when friends use them and try to argue with it
		- if you ask for "if something is true", it tends to say "yes"
		- it finds arguments for it, so some people may think that their opinion is true
	- I have a friend who use it frequently for psychological advises
		- analyse conversations with people and what happend today
		- I can say in total that these psychological advises are quite good. studies show that its much better than have no advise and it tends to be 
		- but here it also tends to sychophancy
	- summarize a video
### Benno
- check if calculations are right
### leif
- stopped using chatgpt, since it is to agreeable
- especially for coding
	- how to make code more efficient
	- debugging
### kayro
- you need to know how to code, since you need to check it quite thoroughly 
### Blackboard
- <u>analytical:</u>
	- check analytical calculations
	- get ideas of analytical derivations
- <u>write papers:</u>
	- spell & language checking
	- rewriting language style & coherence
	- quickly write bullet points
- <u>Coding:</u>

## 26-03-31 LLM Discussion
- take over so much work which was work for a week before
- we cannot avoid it
- certain obvious tasks
	- shorten a text
	- proof it for language
	- we have to proof it always
	- ask llm to look for coherence
	- there are many non obvious hallucination 
		- especially if you are not familiar with the subject you can be tricked
- Dennis:
	- llm are much better for coding, were it is really reliable
	- doing simulations
	- but for text production there is an order of magnitude in quality
	- doesn't read documentation by his own any more
- Benno:
	- if you dont use it for text quality / content
	- but if you use it for the form, writing errors, translation and shortening only
	- check your calculations
	- doing analytical stuff
	- checked an old paper of him if everything is correct:
		- this didnt work for the whole paper, because it didnt understand some approximations
		- but if you use it for sections step by step and check it, it works quite well
	- there is no way to fighting it away
	- it feels very uncomfortable if you did this for years and the llms do it much better in much shorter time
	- human like counter part who you can ask
- kayro:
	- quite good for analytics if you have some insight what is the outcome of it
- aritra:
	- gemini Nano bana pro:
		- good for image generation
		  ![[Pasted image 20260331120941.png]]
		- better than chat gpt
		- you can upload an image you already have and it can manipulates it quite well
		- but the out come is much better if you give it good context
	- click the button - that they don't use your data for training
		- but don't trust it
	- agentic planning/programming
		- codex open AI
		- anthropic claude code
		- antigravity google
		- github copilot - you can upgrade it with TU account
	- claude is much better for analytic stuff like stability analysis
	- visual studio code (installable on ubuntu)
		- codex plugin
		- showed how use it and it produced the whole code for plotting and fitting
		- you only have to check it
		- ![[Pasted image 20260331123047.png]]
		- he uploaded a handwritten note ~={LightBlue}he did it with antigravity=~
		  ![[Pasted image 20260331123310.png]]
		- and it translated it into latex code 
		  ![[Pasted image 20260331123341.png]]
		- it also did the stability analysis and the coding for him
		  ![[Pasted image 20260331123450.png]]
		- 
- me:
	- if you want it more confidential
		- use the european ones like mistral, which are more confidential with the data
		- or the TU 
	- if something is already in the internet it doesn't matter, because it was already scraped by the american and they don't care on the creative commons

## 25-11-28: Feng(25-04) Theory from the anomalous phase behavior of inertial active Brownian particles
- $\mathcal{S}=\frac{\varepsilon}{\zeta U_{0}\sigma}$ gives us a measure for how much can particles overlap?
- Coexisting phases in non equilibrium systems are the binodals ⟹ when you start in a uniformal regime you don't see the binodal
- in equilibrium you don't have a free energy
- reentrance disappears, when the stiffness $\mathcal{S}$ ? Question from Benno
	- you need both stiffness and inertia?
	- if you dont have inertia
	- They didnt rule out the influence of inertia?
- mechanical balance of the interface - modeled by the *dynamic stress tensor* $\mathbb{\Sigma}$ 
- My questions
	- no contradiction to the groups work?⟹yes
	- where is a parallelization problem?
		- ⟹only for strictly hard spheres 
		- WCA isn't about strict hard spheres than I understood it correct
		- what exactly the identify as the binodal?
			- ⟹ When there are two separated phases
			- but since you don't have a free energy this is speculative / not accurate
- $\text{St}\equiv \frac{\tau_{M}}{\tau_{R}}$, $\tau_{M}\equiv \frac{m}{\zeta}$, $\zeta=\gamma_{t}$, $[\tau_{M}]=s=\frac{kg}{\frac{kg}{s}}$ ⟹$[\gamma_{t}]=\frac{kg}{s}$ <span style="font-size:80%;color:orange;">(assumption that </span>$\tau_M$ <span style="font-size:80%;color:orange;">is a time)</span>
	- $\zeta$ translational drag coefficient  $[\gamma]=1$
	- $\tau_{R}$ represents characteristic reorientation/persistence time (or inverse rotational diffusion) $\tau_{R}=\frac{1}{D_{R}}$, $D_{R}=\frac{k_{B}T_{b}}{\gamma_{r}}$, $[D_{t}]=\frac{m^{2}}{s}$ $[D_{R}]=\frac{1}{s}$ $\gamma_{r,\text{sphere}}=8 \pi \eta R^{3}$, $\eta$ is the dynamic viscosity, $[\eta]=\frac{kg}{m s}$, $[k_{B}]=\frac{J}{K}$ 
	- $St \equiv \tau_{M} \cdot \frac{1}{\tau_{R}} =\frac{m}{\gamma_{t}} \cdot D_{R}= \frac{m}{\gamma_{t}} \cdot \frac{k_{B}T_{b}}{\gamma_{r}}$ , $[St]=kg \cdot \frac{1}{s}$ 
	- What are $\gamma_{t}$ , $\gamma_{r}$ and $T_{b}$ in my case? <span style="color:orange;font-size:100%;">lammps script</span>  
```python
# use:: fix ID group-ID langevin/lh Tstart Tstop gamma_t seed alpha(=10*gamma_r/sigma^2/gamma_t) omega <yes/no> zero <yes/no> 
fix 	noise all langevin/lh 1.0 1.0 1.0 §seed 10 omega yes zero yes	# add Langevin thermostat (noise+friction)
``` 
```python
compute	erot all erotate/sphere
thermo_style	custom step temp epair c_erot etotal press
thermo		5000
```
![[Pasted image 20251118151512.png]]
- $\gamma_{t}=1$
- $\gamma_{r}$ 
	- Since $\alpha=\frac{10 \gamma_{r}}{\sigma^{2}\gamma_{t}}=10$
	- $\gamma_{r}=1 \cdot \sigma^{2}\gamma_{t}=1$  

## 25-12-2: Marcos2009~Separation of Microscale Chiral Objects by Shear Flow
DOI: 10.1103/PhysRevLett.102.158103
This is old from 2009
![](Pasted%20image%2020251202122408.png)![](Pasted%20image%2020251202122436.png)
- chiral molecules
- switched the gene off of the bacteria for motility (Dennis asked if a ethic commission approved this🤭), the bacteria was also mutated that it does not split, but in stead grow and get a spiral structure (all controled by protein)
- microfluidic channel 
- shear two opposite planes against each other ⟹ shear on microscale chiral objects in between
- bacterias drift perpendicular to the shear plane
- Net drift results from the preferential alignment of helices with streamlines, with a direction that depends on the chirality of the helix and the sign of the shear rate. 
- separation efficiency $\eta = \frac{|N_{L}-N_{R}|}{N_{L}+N_{R}}$  
- The flow around the particle is approximated linear $u(y)=\frac{vy}{H}$ 

# AMEP
## 25-12-04 Introduction meeting
- color coding is recommended because it is generalized 
	- ⟹for example: If you use AMEP with FFMPG to generate animations you can see from the color of the particle, see the structure factor
-  with the <span style="font-size:100%;color:red;">API Reference</span> you can search the documentary of all used/integrated packages
- hdf5:
	- Used for really huge files
	- AMEP uses a hdf5 file based format: **H5AMEP** 
	  ![](Pasted%20image%2020251204155111.png)
	- infos are in **User Guide** on the AMEP Page
	  
# Papers
## M.Rovere1993~Simulation studies of gas-liquid transitions in two dimensions via a subsystem-block-density distribution analysis
### 4. low temperature limit of the cumulants in the 2D-Ising model
- 2D-Ising model on a square lattice in the groundstate at constant magnetization $\left< m \right> = -1 + 2 \left< \rho \right>$
- The groundstate (or configuration of minimum free energy, respectively) is easily identified by the property of minimal interface energy of the states with spins pointing in opposite directions.
- Let us denote the linear extension perpendicular to the interface of the area with positive spins by A. $$
A= \frac{S\left( \left< m \right> +1  \right)}{2}
$$
- probability $P_{L}(m)$ for having the magnetization $m$ in subsystems of size $L \times L$ is for case
	- **(I)** $L \le S - A = \frac{S}{2} \left( 1-\left< m \right> \right)$
	  $$
P_{L}(m)=
\begin{cases}
\frac{2}{S}  &m=-1+\frac{2i}{L}; \quad \{i=1,2,\dots,L-1\}\\  
\left( A-L+1 \right)/S  &m=+1 \\
(S-A-L+1) /S &m=-1
\end{cases}
$$
	- **(II)** $L>S-A$ $$
P_{L}(m)=
\begin{cases}
\frac{2}{S} &m=-1+\frac{2i}{L};  \{i=S-A+1,\dots,L-1\}   \\
 \left( L-S+A+1 \right) /S &  m=1-\frac{2(S-A)}{L}\\
 (A-L+1) /S & m=1\\
\end{cases}
$$
- $M:=\frac{S}{L}$ and $A= \frac{S\left( \left< m \right> +1  \right)}{2}$ we get
	- **(I)**  $L \le S - A = \frac{S}{2} \left( 1-\left< m \right> \right)$ ⟹ $L \le S - \frac{S\left( \left< m \right>+1 \right)}{2} =\frac{2S-S\left< m \right>-S}{2}=\frac{S\left( 1-\left< m \right> \right)}{2}$ 
	  ⤷$\frac{S}{L}=M \ge \frac{2}{\left( \left< m \right>-1 \right)}$
	- **(II)** $L>S-A$ 
	  ⤷$\frac{S}{L}=M < \frac{2}{\left( \left< m \right>-1 \right)}$

## [Mukhopadhyay2025](https://doi.org/10.1038/s42005-025-02265-0) - Active adaptolates featuring motilityinduced percolating structures with an adaptive packing geometry

![](images/Papers/Mukhopadhyay2025-Fig3-a.png)
## Mandal2019~Motility-Induced Temperature Difference in Coexisting Phases

### Supplement
diffusion coefficients ($D_r$ and $D_t$) and friction coefficients ($γ_r$ and $γ_t$) are not related by the Stokes-Einstein relation. Thus, for simplicity, we choose $γ_t = γ_r/σ^2$ .

Stokes-Einstein relation $D=\frac{k_BT}{6 \pi \eta r}$ with $\tau=\frac{\gamma}{m}$ the relaxation or persistence time. For spherical particles of radius $r$ Stokes' law gives $\gamma = 6 \pi \eta r$. 
- $\gamma_{t}=1$
- $\gamma_{r}$ 
	- Since $\alpha=\frac{10 \gamma_{r}}{\sigma^{2}\gamma_{t}}=10$
	- $\gamma_{r}=1 \cdot \sigma^{2}\gamma_{t}=1$  
-  $\tau_{p} = \frac{1}{D_{r}}$ 
- $Pe=$

### [Scholz2018 | Inertial delay of self-propelled particles | Nature Communications](https://www.nature.com/articles/s41467-018-07596-x)
- P.2; **Underdamped Langevin model.**:
   Owing to the strong non-equilibrium nature of the system, the <span style="font-size:100%;color:green;">diffusion and damping constants</span> are <span style="font-size:100%;color:red;">not related</span> by the Stokes-Einstein relation
  
- P.5-6 **Discussion:**
   The long-time diffusion coefficient of passive particles is independent of inertia and is related to the friction coefficient via the Stokes−Einstein relation. However, for actively moving particles we find an explicit dependence on the moment of inertia (with no explicit dependence on the total mass M) 

### [Lei2020|]()
- P.2 Result ⟹ **Model**:
	 For simplicity, we set $\gamma_{t}=\frac{\gamma_{r}}{\sigma^2}$ 
- E44D0A

# What is my $Pe$ ?
![](Pasted%20image%2020260116235151.png)
- $Pe=\frac{v_{0}}{D_{r}\sigma}\propto \frac{\tau_{p}}{\tau_{c}\varphi}$ [Mandal2019](https://doi.org/10.1103/physrevlett.123.228001) with the persistence time $\tau_{p}=\frac{1}{D_{r}}$, the packing fraction $\varphi$ and the Mean time between collisions $\tau_{c}=\frac{\pi \sigma}{4v_{0}\varphi}$ 
Stokes-Einstein relation $D=\frac{k_BT}{6 \pi \eta r}$ with $\tau=\frac{\gamma}{m}$ the relaxation or persistence time. For spherical particles of radius $r$ Stokes' law gives $\gamma = 6 \pi \eta r$. 
- $\gamma_{t}=1$
- $\gamma_{r}$ 
	- Since $\alpha=\frac{10 \gamma_{r}}{\sigma^{2}\gamma_{t}}=10$
	- $\gamma_{r}=1 \cdot \sigma^{2}\gamma_{t}=1$  
-  $\tau_{p} = \frac{1}{D_{r}}$ 

⟹ $Pe \propto \frac{\tau_{p}}{\tau}$
$Pe = \frac{v_{0}}{\sqrt{ 2D_{r}D_{t} }}$, $D_{t}=\frac{k_{B}T}{\gamma_{t}}$, $D_{r}=\frac{k_{B}T}{\gamma_{r}}$ 
LAMMPS: 
![](Pasted%20image%2020260116235234.png)
Where this defines the selfpropulsion force $F_{i}=f_{p}e_{i}$ with the Magnitude $f_{p}=42.4264$ 
$f_{p}=\gamma_{t}v_{0}$ 
$\frac{\sigma}{\sqrt{ D_{r}D_{t} }}=1$ 
$\frac{\varepsilon}{k_{B}T}=10$ ![](Pasted%20image%2020260117000418.png)
$Pe=\frac{42.4264}{\sqrt{ 2 }}\sim 30$
Laut Mandal2019 P. 2 ist die kritische $Pe \ge 20$ 
<span style="font-size:100%;color:red;">Simulationen mit einer deutlich höheren Pe versuchen</span>

## Buchkapitel [book:BookChapter](https://doi.org/10.48550/arXiv.2102.13007)
### The different time scales
1. The motion of  ABP is initially diffusive with a diffusion coefficient $D$ for $t\ll \frac{D}{v_{0}^2}$. 
2. For $\frac{D}{v_{0}^2}\ll t\ll \tau_{p}$ a ballistic regime comes about which represents directed motion due to activity of the particle. 
3. Finally for $t\gg \tau_{p}$, the motion is again diffusive with an "active Diffusion coefficient" $D_{A}=D+\frac{l_{p}^2}{2\tau_{p}}$ 
![](Pasted%20image%2020260116152453.png)
- The initial directed motion takes place over a distance $l_{p}=\frac{v_{0}}{D}$ for a persistence time $\tau_{p}=\frac{1}{D_{R}}$ 
- $\Braket{\vec{r}_{i}(t)-\vec{r}_{i}(0)}=l_{p}\left( 1-e^{-t / \tau_{p}} \right)$ the average displacement of a ABP
- An ABP moves on average over a distance $l_{p}$ along its initial orientation $\vec{p}(0)$ before it's orientation is randomized, which rationalizes the term "persistence length" for $l_{p}$ 
- $\Braket{\left( \vec{r}_{i}(t)-\vec{r}_{i}(0) \right)^{2}}=2l_{p}^{2}\left( \frac{t}{\tau_{p}}-1+e^{-t / \tau_{p}} \right) +4Dt$ the mean square displacement of a ABP

### The Péclet number

- The relative importance of activity in comparison with diffusion can be characterized by the **Péclet number**:
- $Pe=v_{0}\sqrt{ 2DD_{R} }$ ,$D=\frac{4}{3}R^2D_{R}$, $Pe=\frac{\sqrt{ \frac{3}{2} }v_{0}}{\sigma D_{R}}$ or $Pe=\frac{v_{0}\sigma}{\sqrt{ 6 }D}$


# Critical Exponents
## Correlations Length $\xi$
is the overall driving factor for the behavior at a continuous phase transition (2. Order). At the phase transition fluctuations grow large until no distinction between two phases is possible.  
⟹The correlation goes to infinity. In the vicinity of the phase transition point it exhibits a power law,  
⟹$ξ(X)∼|X-X_C |^{-ν},ν=1$ for 2D Ising model

## Scaling relations and Universality 
Critical Exponents aren't independent, the six critical exponents are connected by four scaling relations. [Herrmann_CompPhys_2021](https://doi.org/10.1017/9781108882316)
- $\alpha + 2\beta + \gamma =2$ (Rushbrooke)
- $\gamma = \beta(\delta-1)$ (Widom)
- $\gamma=(2-\eta)\nu$ (Fisher)
- $2-\alpha=d\nu$ (Josephson)
### Hyperscaling relation
Rushbrooke and Josphson ⟹ $2-(2-2\beta-\gamma)=d\nu$ with $d=2$  ⟹ $2\nu= 2\beta+\gamma$ 
# Reports

## Bennos Answer to my report slides 26-01-22
Hi Lukas, 

Thanks a lot for preparing the report! This is quite useful to see where you are. 

- Slide 5, bottom right; inside the green frames, the particle distribution looks patterned. Is this true? 
	- [ ] Send Ovito pictures from ⟹ isn't necessary, this is the exact snapshot like in the picture above. This comes from the resolution of the particles, which is somehow different when depicting them with a smaller evaluation box size. I recognised this earlier and was confused by, but didn't investigated this depiction problem, since there were more important tasks and I am affected enough by such distractions


- Slide 11: The different curves seem to meet in one point (roughly), which is nice! The results on slides 13 and 14 are probably useless, right? 
	- Maybe it looks this way, because the Binder cumulant curves for the two smallest system sizes were shift so far away from the others.


- Slides 19, 20: The susceptibilities do not show any peaks. Why is that? Aren't you crossing a phase transition line? What is the idea here? What are the values of the fixed parameters? 
	- That's true an Explanation is found in [Maggi2021](https://doi.org/10.1039/d0sm02162h) . 
	  *⟹Due to the fact that it is obtained by averaging over the evaluation boxes in the dense and dilute phase.*
		- Fig 2 c) of [Maggi2021](https://doi.org/10.1039/d0sm02162h) 
		  ![](images/Report/Maggi2021-Fig2c.png)
		  Here it was discussed:  
		  *Note also that the $\chi$ in Fig. 2(c) does not show the typical peak as in the Ising model. This is due to the fact that the $\chi$ is obtained here by averaging the values of Nb in both the dense and dilute phases. In the ESI† we show that the $\chi$ (computed in the same way) for the lattice gas displays a similar s-shaped curve a  way) for the lattice gas displays a similar s-shaped curve as a function of the inverse temperature and scales with $\gamma= 7/4$.* 
	- I compared them with the Fig 1. b) of [Feng2025, P.2](https://doi.org/10.48550/ARXIV.2502.09069) , where I took also the expression for susceptibility. My plots are looking quite similar and I didn't find a further discussion about the missing peak in the paper and it's supplement material. They discussed the value for it's exponent $\gamma$ only. 
		- Fig2 b) of Feng2025 ![](Pasted%20image%2020260122172821.png)


- Slide 28: This is nice; the results for the critical point seem to be similar in all cases. 
	- Thanks

- Slide 30: I am not sure I understand the difference between the left and the right plot. In either case, the determined exponent for correlation length (\nu) looks unusually large! (For overdamped ABPs \nu ~ 1.5 I think and for the 2D Ising model it is 1). 
	- Yes this is something I worried about and we have to investigate. I guess there is some mistake.

- Slides 32. 33: Why is \beta negative? How do you interpret this? Can this be correct? (It is 1/8 for the 2D Ising case; and ~1/2 for ABPs perhaps) 
	- No it isn't negative. This was a mistake. I forgot to take into account that. 
	  $m=-\frac{\beta}{\nu}$ So if m is negative, than $\beta$ is positive. Sorry for that.

- Slide 35: The obtained coefficient for \gamma is quite small. Why is that? Why is it that small (<1/4) compared to the Ising case (7/4) and the case of overdamped ABPs (2.2)? 
	- My answer for that was:
	  ⟹because I wasn't able to transform a simple equation as I see... so shameful. I wasn't present in this moment. The same issue for $\beta$

The obtained results would mean that the scaling relation (\gamma + 2\beta = 2\nu ) is very strongly violated. It could be violated, perhaps, but probably not that strong. 

In view of the obtained very unusual results for the critical exponents, it would probably be good to check results for the overdamped case too and compare with known literature results. 

  

@Aritra and Suvendu: What is your take on the report and obtained results? I am somewhat sceptical if this is all correct, I must say, but I guess you have discussed this with Lukas. 

Best wishes

Benno

# Glossar

## driven vs. active system
When comparing **driven** vs. **active** systems, the distinction usually boils down to the source of power and control. ==A **driven system** relies on an external, overarching force to move or guide it. An **active system** generates its own energy or intelligence to self-regulate, adapt, or perform specific actions==
## renormalization group (RG)
The renormalization group is intimately related to scale invariance and conformal invariance, symmetries in which a system appears the same at all scales (~={LightBlue}self-similarity=~), where under the fixed point of the renormalization group flow the field theory is conformally invariant.

To be more concrete, consider a magnetic system (e.g., the Ising model), in which the J coupling denotes the trend of neighbor spins to be aligned. The configuration of the system is the result of the tradeoff between the ordering J term and the disordering effect of temperature.
For many models of this kind there are three fixed points:

1. T = 0 and J → ∞. This means that, at the largest size, temperature becomes unimportant, i.e., the disordering factor vanishes. Thus, in large scales, the system appears to be ordered. We are in a ferromagnetic phase.
2. T → ∞ and J → 0. Exactly the opposite; here, temperature dominates, and the system is disordered at large scales.
3. A nontrivial point between them, **T = Tc and J = Jc.** In this point, changing the scale does not change the physics, because the ~={Gold}system is in a fractal state=~. It corresponds to the Curie phase transition, and is also called a ~={Tomato}critical point=~.
### Elementary theory
In more technical terms, let us assume that we have a theory described by a certain function Z of the state variables {$s_{i}$} and a certain set of coupling constants {$J_{k}$}. 
This function may be a partition function, an action, a Hamiltonian, etc. It must contain the whole description of the physics of the system.

Now we consider a certain blocking transformation of the state variables $\{s_{i}\}\rightarrow\{\tilde{s}_{i}\}$. The number of $\tilde{s}_{i}$ must be less than the number of $s_{i}$ . Now let us try to rewrite the Z function _only_ in terms of the $\tilde{s}_{i}$. If this is achievable by a certain change in the parameters, $\{J_{k}\}\rightarrow\{\tilde{J}_{k}\}$, then the theory is said to be **renormalizable**.

The change in the parameters is implemented by a certain beta function: $\{\tilde{J}_{k}\}=\beta(\{J_{k}\})$, which is said to induce a **renormalization group flow** (or **RG flow**) on the J-space. The values of J under the flow are called **running couplings**.

The most important information in the RG flow are its **fixed points**.

### Relevant and irrelevant operators and universality classes
Consider a certain observable A of a physical system undergoing an RG transformation. The magnitude of the observable as the length scale of the system goes from small to large determines the importance of the observable(s) for the scaling law:

| _**If its magnitude**_ ... | _**then the observable is**_ ... |
| -------------------------- | -------------------------------- |
| always increases           | **relevant**                     |
| always decreases           | **irrelevant**                   |
| other                      | **marginal**                     |
A _relevant_ observable is needed to describe the macroscopic behaviour of the system. _Irrelevant_ observables are not needed. _Marginal_ observables may or may not need to be taken into account. A remarkable broad fact is that _most observables are irrelevant_, i.e., _the macroscopic physics is dominated by only a few observables in most systems_.

The coincidence of the critical exponents (i.e., the exponents of the reduced-temperature dependence of several quantities near a second order phase transition) in very disparate phenomena, such as magnetic systems, superfluid transition (Lambda transition), alloy physics, etc. So in general, thermodynamic features of a system near a phase transition depend *only on a small number of variables*, such as the **dimensionality** and **symmetry**, but are *insensitive to details of the underlying microscopic properties of the system.*

This coincidence of critical exponents for ostensibly (angeblich) quite different physical systems, called universality, is easily explained using the renormalization group, by demonstrating that the differences in phenomena among the individual fine-scale components are determined by irrelevant observables, while the relevant observables are shared in common. Hence *many macroscopic phenomena* may be grouped into a **small set of universality classes**, specified by the shared sets of relevant observables.
## Vicsek model
- collective motion and swarming 
- ~={DeepPink}minimal=~ and describes a kind of universality
- point-like self-propelled particles
	- evolve at ~={DeepSkyBlue}constant speed=~
	- ~={purple}align their velocity=~ with their neighbours' one in presence of noise
- ~={MediumSpringGreen}collective motion=~
	- at ~={orange}high density=~ 
	- or ~={yellow}low noise on the alignment=~
- it assumes that ~={Teal}flocking=~ is due to the combination
	- any kind of self propulsion
	- and effective alignment
- Velocity of each particle is constant ~={Crimson}⟹=~ net momentum of the system is not conserved during collisions
- individual $i$ described by
	- position $\mathbf{r}_{i}(t)$
	- the angle direction of its velocity $\mathbf{\Theta}_{i}(t)$ at time $t$
- Discrete time evolution of one particle
	- At each time step $\Delta t$ each agent aligns with its neighbors within a given distance $\mathbf{r}$ with an uncertainty due to a noise $\eta_{i}(t)$ 
	  $$
\mathbf{\Theta}_{i}(t+\Delta t)  = \langle \mathbf{\Theta}_{i} \rangle _{\left| r_{i}-r_{j} \right| <r} + \eta_{i}(t)
$$
	- the particle then moves at constant speed $v$ in the new direction
	  $$
\mathbf{r}_{i} (t+\Delta t) = \mathbf{r}_{i}(t)+ v \Delta t \begin{pmatrix}
\cos \mathbf{\Theta}_{i}(t) \\
\sin \mathbf{\Theta}_{i}(t)
\end{pmatrix}
$$
- $\langle \mathbf{\Theta}_{i} \rangle _{\left| r_{i}-r_{j} \right| <r}$ denotes the average direction of the velocities of particles (including particle $i$) within a circle of radius $r$ surrounding particle $i$. 
- The average normalized velocity acts as the order parameter for this system and is given by $$v_{a} = \frac{1}{Nv} \left| \sum_{i=1}^{N} v_{i}\right|$$
- The whole model is controlled by ~={DarkViolet}three parameters=~:
	- the density of particles
	- the amplitude of the noise on the alignment
	- the ratio of the travel distance $v\Delta t$ to the interaction range $r$ 

## **Non-reciprocal interactions** 
==occur when the effect Entity A has on Entity B is unequal to the effect Entity B has on Entity A==. This violates Newton’s third law of motion (action and reaction) and the principle of detailed balance, creating dynamic, out-of-equilibrium systems.
### Why They Matter

- **Active Matter & Biology:** In biological and active matter systems (like cellular components or swarms), non-reciprocal couplings allow for self-organization, regulate system stability, and prevent stagnation. For instance, one organism may actively pursue another while the target ignores the pursuer, driving run-and-chase dynamics.
- **Physics & Materials:** In photonics and materials science, non-reciprocal systems (such as optical isolators) allow waves or particles to travel in one direction but not the reverse. This enables exotic phenomena like odd elasticity and persistent heat currents, even in thermal equilibrium.
- **Emergent Behaviors:** These asymmetries often result in unexpected collective states, including non-reciprocal phase transitions, chimera states, and high-dimensional chaos. [[1](https://link.aps.org/doi/10.1103/PhysRevX.14.011029), [2](https://www.ds.mpg.de/4080176/250422_Saha_non-reciprocal), [3](https://www.rieger.uni-saarland.de/Paper/Choi-Noh-Rieger.pdf), [4](https://arxiv.org/abs/2503.20908), [5](https://dgklab.ch.rachip.com/non-reciprocal-systems/), [6](https://physik.univie.ac.at/news/news-detailansicht/news/non-reciprocal-interactions-can-stabilize-dynamical-phases-of-matter/)]
## **Non-polar active nematics**
are ==non-equilibrium active materials made of elongated, symmetric units (like rod-shaped bacteria or vibrated granular rods) that have no distinct "head" or "tail"==. Despite lacking polar directionality, these systems continuously consume energy to generate spontaneous, chaotic flow and self-driven topological defects.

### Core Physical Properties
- **Nematic Order**: The constituents align locally along a shared axis, represented mathematically by a director field $\mathbf{n}$ and a symmetric traceless tensor $Q_{ij}$. The orientation states $\mathbf{n}$ and $-\mathbf{n}$ are physically indistinguishable.
- **Active Stress**: Unlike passive liquid crystals, internal stresses generated by the constituent agents (e.g., cell divisions or molecular motors) drive the fluid out of equilibrium.
- **Active Turbulence**: The competition between continuous active forcing and viscous dissipation gives rise to a chaotic, swirling flow state known as active turbulence.

### Topological Defects and Dynamics
- **Symmetry**: In two-dimensional non-polar nematics, the orientational order breaks at isolated points known as topological defects, which are characterized by their topological charge $k=\pm \frac{1}{2}$.
- **Self-Propulsion**: Because the system is active, the $+\frac{1}{2}$ defects (which resemble comets) are inherently self-propelled. They swim through the fluid at a velocity $\mathbf{v}$  scaling with the local active stress gradient. In contrast, the $-\frac{1}{2}$ defects (which are trefoil-shaped) remain essentially stationary.
- **Creation and Annihilation**: The active turbulence continuously generates and destroys defect pairs. Pairs of $+\frac{1}{2}$ and $-\frac{1}{2}$ defects are created, after which the faster, self-propelled $+\frac{1}{2}$ defects often encounter and annihilate defects of the opposite charge.

### Biological and Synthetic Examples

- **Biophysics**: Non-polar active nematic physics are frequently used to model dense tissues and cell monolayers. In these systems, elongated cells organize into aligned nematic domains, and the chaotic movement of cells is directly governed by defect generation and annihilation.
- **Microtubule Assays**: A classic _in vitro_ experimental system consists of microtubules and motor proteins (such as kinesin) sandwiched at an oil-water interface, creating an active two-dimensional nematic layer.
- **Synthetic Systems**: Non-polar active nematics can also be replicated using granular systems, such as vibrated monolayers of elongated rods that exhibit collective alignment and chaotic streaming.

### Theoretical Framework

The hydrodynamic theory for non-polar active nematics relies on the coupled equations for the nematic order tensor $Q_{ij}$ and the velocity field $\mathbf{u}$. The equations are extensions of the passive Beris-Edwards framework, modified to include active stress tensors. The key governing parameters include the friction coefficient $\zeta$ and the active stress coefficient $\alpha$, which controls the transition to chaotic flow. [[1](https://www.nature.com/articles/s41467-018-05666-8)]

## mixtures of non-self-propelling scalar active matter
Mixtures of non-self-propelling scalar active matter refer to ==out-of-equilibrium systems where individual particles lack directional motion (self-propulsion)==. Instead, activity emerges entirely from their asymmetric, nonreciprocal interactions, meaning particles of different species react to one another differently than vice versa. This microscopic violation of action-reaction symmetry drives complex, large-scale dynamical patterns.
### Core Concepts
- **Scalar Active Matter:** Systems where the primary variable is the particle density rather than orientation (like aligning polar/nematic groups).
- **Newton's Third Law Violation:** In isolation, spherical non-self-propelling particles exhibit only anomalous fluctuations. When mixed, their interactions lose reciprocity (e.g., A chases B, but B avoids A), creating dynamic, out-of-equilibrium behavior.
- **The Non-Reciprocal Cahn-Hilliard (NRCH) Model:** The standard theoretical framework. It modifies the classical equilibrium Cahn-Hilliard equations—which govern phase separation and spinodal decomposition—by adding antisymmetric currents.

### Emergent Phenomena & Phases

- **"Chase and Rest" Phase:** Instead of static, segregated domains, nonreciprocal species create dynamical steady states. For instance, a droplet of one species may continuously trail a shrinking droplet of another.
- **Traveling Density Bands:** The system can spontaneously generate macroscopic polar order from scalar components. These collective density bands travel in defined directions with an intrinsic wavelength.
- **Active Smectic Phases:** Alternate moving bands of different species can form an active layered structure that coarsens over time via topological defect annihilation. 
### Physical Mechanisms

- **Non-conserved dynamics:** The system fundamentally behaves similarly to the complex Ginzburg-Landau equations, driven entirely by the coupling constants that represent active, nonreciprocal energy consumption.
- **Phase-space compression:** The non-equilibrium nature of the system causes a coupling between densities and fluxes, meaning phase transitions differ drastically from conventional Ostwald ripening. [1](https://www.researchgate.net/publication/341396358_Scalar_Active_Mixtures_The_Non-Reciprocal_Cahn-Hilliard_Model), [2](https://arxiv.org/abs/2005.07101)

# LLM
## TUDaGPT
![[Pasted image 20260407132230.png]]
![[Pasted image 20260407132257.png]]
![[Pasted image 20260407132320.png]]![[Pasted image 20260407132336.png]]


# Forschungsidee
- phasenübergänge in Lernumgebungen
	- beobachtetes system: Klasse zb. 5c an der BAS
	- schüler sind aktive materie
		- 
	- phasenübergang: chaos -> ruhe -> produktive atmosphäre 
		- physikalisch optimale methode: wie schafft man es ruhe in ein system hineinzubringen, dass chaotisch ist:
			- schulklasse
			- staaten
			- menschenmengen
	- perkolation: 
		- brände eindämmen (negativ) - das keine störungen entstehen:
			- Vertrauensherde schaffen
		- schüler stecken sich mit motivation an 
		- helfen sich gegenseitig und begeistern sich
		- wollen sich in der gruppe vor störquellen beschützen und sich gegenseitig postiv verstärken
	- Lehrerkeimzelle für phasenübergänge, um lokal die energie zu minimieren
	- Energieminimierung:
		- lehrer will energie minimieren: 
			- was ist dessen messgröße für guten Unterricht
			- ruhe in der klasse
			- der schein, dass alle mitarbeiten
			- ein guter schnitt in der klassenarbeit
		- schüler wollen eigene Energie minimieren
			- wollen spaß haben -> gibt Energie
			- energieschwelle/potentialbarriere: 
				- motivationsbarriere
				- störgeräusche
				- aktive physische störungen
				- unkonzentriert
				- demotiviert/ich kann es nicht
			- energie quelle: 
				- motivation
					- intrinsich
					- extrinsich 
				- Bedürfnisse erfüllt
					- toilette
					- essen
					- trinken
					- fühlen sich gut
						- gutes familienklima
						- gutes klassen setting
						- fühlen sich wertgeschätzt
							- durch lehrer
							- eltern
							- mitschüler
						- psychisch stabil
				- angst vor bestrafung
			- energie kosten:
				- zwang 
				- angst vor bestrafung
				- demotivation
				- krach
				- energieverbrauch durch arbeit
				- schlechte bewertungen
				- sprachbarrieren
- videoaufzeichnungen vom verhalten einer klasse, des ablaufs einer schulstunde
- ziel: phasenübergang zur positv bestärkenden arbeitsatmosphäre: systeme: schulklasse, schule, stadt, staat, region, krieg, paniksituation
	- klasse:
		- ideal:
			- sie kommen gerne
			- sie arbeiten selbstständig
			- ich kann vertrauen,
				- wenn ich mich umdrehe
				- ich aus der klasse gehe
				- einzelperson wegschicke
				- die kinder in anderen situationen sind
					- schulhof
					- zu hause
					- freizeit
			- sie denken weiter
			- kommen mit "positiven"/konstruktiven fragen zu einem 
				- keine destruktiven fragen und themen:
					- streit 
					- probleme
					- jemand hat mich gestört
				- ich beantworte gerne bereichernde fragen, wenn die motivation in einem anderen erzeugen
			- neutrale Fragen:
				- orga

- Modellierung:
	- interaktion mit nachbarn (kurzreichweitige WW), next neighbor interaction
				- nicht vom arbeiten abhalten (neutral)
				- stören nachbarn aktiv (negativ)
				- beruhigen nachbarn (positiv)
				- befördern nachbarn zum lernen (sehr positiv)
				- helfen nachbarn bei gewissen aufgabenstellungen (extrem positiv)
	- WW in teilgruppe: 
				- explizite freunde
				- lose schulhoffreunde
				- Kernklasse
				- fachunterricht klasse
				- jahrgang
				- schule
	- WW zwischen teilgruppen
	- perkolation
	- lossfunction
	- energie verbrauchsminimierung
	- 