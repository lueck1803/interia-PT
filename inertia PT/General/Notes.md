# fast notes
- latex suite:
  {trigger: "|", replacement: "|$0|$1", options: "mA"},
- ![](Pasted%20image%2020251205205458.png)
# Arbeit
-  
# Tage infolge Produktiv
Tage produktiv gewesen:
||||/ ||||/ ||||/ ||||/
||||/ ||||/ ||||/ ||||/


# Backen und kochen
- <span style="color:gold">ei steif schlagen</span> 
- hoher Becher statt breite Schüssel 
- Metall Schüssel statt Plastik, wegen dem fett was an Plastik besser haftet.⟹Fett ist der Feind von Steifem Eiweiß 
- Prise Salz ⟹wirkt auf die elektrische Ladung der Proteine, die stoßen sich weniger ab

# Pdftk
- Gerade (`A.pdf`) und ungerade Seiten (`B.pdf`) eines Dokuments zusammen fügen.
  `{bash} pdftk A=A.pdf B=B.pdf shuffle A Bend-1 output Dokument_Name.pdf`
- Alle Bilddateien (pdf, jpg), mit der passenden Dateiendung (\*.ext) werden in ein Dokument zusammengefügt.
  `{bash} pdftk *.ext cat output Dokument_Name.pdf`
- <span style="font-size:100%;color: orange;">Scanner Software unter Linux</span> ⟹Scan Gear <br>PdfTK unnötig, da hier bereits Shuffle Funktion integriert ist 

# git
- Comment in `.gitignore` with # 
- Ausnahmen mit `!`
- wenn Dateien der `.gitignore` hinzugefügt werden, müssen sie auch aus dem chache entfernt werden
  `{git} git rm --cached .obsidian/hotkeys.json`
- - Wenn dies für alle Unterordner gemacht werden soll, dann:
  `{git} git rm -r --cached .obsidian/plugins/\\*`
- `{git} git config --global --edit`
## What is git fetch?[](https://about.gitlab.com/blog/git-pull-vs-git-fetch-whats-the-difference/#what-is-git-fetch)

The git fetch command retrieves the latest commit history from the remote repository, but it does not affect the local working directory. Even after fetching remote changes, they are not reflected in the local branch. It is primarily used when you want to retrieve the latest status from the remote repository and review the changes before they are reflected in the local repository. To apply the retrieved changes to the local branch, you need to manually run git merge or [git rebase](https://docs.gitlab.com/ee/topics/git/git_rebase.html).

## What is git pull?[](https://about.gitlab.com/blog/git-pull-vs-git-fetch-whats-the-difference/#what-is-git-pull)

The git pull command combines `git fetch` and `git merge` (or `git rebase`) into a single command. This allows you to fetch changes from the remote repository and automatically integrate them into the current local branch.

While git fetch retrieves changes from the remote repository without applying them to the local branch, running git pull automatically integrates the changes from the remote repository into the local branch.

Git pull is suitable for quickly reflecting remote changes in the local branch, but it can lead to conflicts, so caution is needed, especially when working with multiple people.

## When to use git fetch[](https://about.gitlab.com/blog/git-pull-vs-git-fetch-whats-the-difference/#when-to-use-git-fetch)

Git fetch is a command used to retrieve the latest information from a remote repository. The retrieved information is not directly reflected in the local branch. Using git pull will reflect all remote branches, including incorrect or problematic ones, in the local branch.

When changes are made simultaneously on both remote and local branches, or when there are new users on the team, it is safer to use git fetch to retrieve the remote branch contents first and then perform merge or rebase.

## When to use git pull[](https://about.gitlab.com/blog/git-pull-vs-git-fetch-whats-the-difference/#when-to-use-git-pull)

Git pull is a command that performs more processes compared to git fetch. Git pull can perform both git fetch and additionally execute git merge or git rebase. For this reason, git pull is recommended when you want to quickly reflect changes from the remote repository in the local branch.

# YouTube 
Wenn man bei der YouTube app ein Video ab einem Zeitpunkt verlinken möchte 
`youtubelinkt`+`?t=MMmSSs`⟹`youtubelink`+`?t=17m18s` ⟹ https://youtu.be/Yz9Bj9kEtKc?si=umUGQ2rElxZL_YgD?t=17m18s
Mann muss die Zeit wohl in Sekunden umrechnen 🤷 und ohne Angabe der Zeiteinheit.
`youtubelinkt`+`?t=Sekunden`
17m 18s ⟹ 17 \* 60 + 18 = 1038
`youtubelinkt`+`?t=1038`
https://youtu.be/Yz9Bj9kEtKc?t=1038
Und man muss den ganzen Murks bis zum ersten Fragezeichen entfernen:
https://youtu.be/Yz9Bj9kEtKc?si=umUGQ2rElxZL_YgD
dh. `si=umUGQ2rElxZL_YgD` 
Ne geht auch mit dem `?t=MMmSSs` Format. Das Problem ist der Murks hinter dem ersten Fragezeichen.
https://youtu.be/Yz9Bj9kEtKc?t=17m18s

# Latex Suite
 {trigger: "Brk", replacement: "\\Braket{$0} $1", options: "mA"},
 
$\Braket{\int \frac{ \partial r }{ \partial t }^{2} \, dx}$
$\Braket{\frac{x}{y}^{2}\cdot x^{2}}$

# Bash / zsh

## grep and find
_The Major difference is **FIND** is for searching files and directories using filters while **GREP** is for searching a pattern inside a file or searching process(es)_

**FIND** is an command for searching file(s) and folder(s) using filters such as size , access time , modification time.  
The find command lists all of the files within a directory and its sub-directories that match a set of filters.  
This command is most commonly used to find all of the files that have a certain name.

To find all of the files named theFile.txt in your current directory and all of its sub-directories, enter:
```Bash
find . -name theFile.txt -print
```

To look in your current directory and its sub-directories for all of the files that end in the extension .txt , enter:  

```Bash
find . -name "*.txt" -print
```

**GREP** :(Globally search a Regular Expression and Print)

Searches files for a specified string or expression.

Grep searches for lines containing a specified pattern and, by default, writes them to the standard output.

```Bash
grep myText theFile.txt
```

Result : Grep will print out each line contain the word _myText_.

`{bash} ls -l *.ps | grep May`

## ls
The `ls` command has a variety of options to customize its output:

- `-l` - Long listing format
- `-a` - Include hidden files
- `-h` - Human-readable sizes
- `-t` - Sort by modification time
- `-r` - Reverse order while sorting
- `-R` - List subdirectories recursively
- `-S` - Sort by file size
- `-1` - List one file per line
- `-d` - List directories themselves, not their contents
- `-F` - Append indicator (one of */=@|) to entries

## column
# PowerShell
## find string after a command
```PowerShell
 COMMAND | Where-object PROPERTY -match "string"
```
```PowerShell
choco list | findstr -i "kee*"
```
# copy content of a file on the clipboard
```PowerShell
gc .\myfile.txt | scb
```

# PW manager
Wechsel von heylogin zu keypass als Standard autofill

> [!Navigate]
> Keepass ⟹three dots ⟹settings⟹app settings ⟹password entry access ⟹autofill service ⟹autofill service enable

# Nachricht an Maria 
Meditation ist diese Woche eher hinten runter gefallen.
Ich hab für meine Verhältnisse sehr viel gearbeitet.

Und ja gerade da hätte es mir gut getan.

Ich merke auch wie sehr es mir fehlt.
Ich glaube Montag habe ich meditiert.

Ich war dafür Mittwoch morgens laufen. Das ist ein wenig wie Meditation für mich. 

Irgendwie war so viel los in meinem Kopf. 

Gerade da wäre es gut gewesen.🤷‍♂️

Ich war dann auch etwas krank aber zum Glück nicht wirklich 

Da ich das gut mit schlaf und Achtsamkeit gemanagt habe. 

Ich war halt so voller Tatendrang.

Und hab da in meinem Job auch Verantwortung übernommen. Mittwoch war ich dann noch bei nem Vortrag zu Abwehrmechanismen von Pflanzen, das war sehr interessant.
Die Frau hat dabei auch das Schöllkraut in ihrer Forschung erwähnt. Das hat mich sehr gefreut, da Otmar das hier in Ahl ja eingeführt hat, um es auf Wunden zu tun und gegen Warzen.
Zumindest die Antimikrobielle Wirkung und die Verhinderung von Biofilmbildung haben die nachgewiesen.
Ich habe auch Lob von meinem Chef bekommen.
Nachdem Vortrag habe ich mit einer noch über 2h vor dem hessischen Landesmuseum in der Kälte über alles Mögliche geredet... 
Das war im Endeffekt auch viel zu verarbeiten.

Es geht so viel durch meinen Kopf und Körper. Letzte Woche hatte sich auch spontan ergeben, dass mein Psychiater nicht mehr da ist/aufhört und da musste ich mir einen neuen suchen... hatte ganz andere Sachen zu tun...
Das habe ich letzte Woche zum Glück hinbekommen, halt in Offenbach. Dafür bin ich letzte woche zwei mal nach offenbach gefahren, musste meine Patientenakte und alles besorgen.
Dabei ist mir auch wieder sehr viel durch den kopf und Körper gegangen, hatte das Gefühl ich müsste mich wieder erklären und rechtfertigen, ob ich wirklich ADHS habe.
Damit hatte ich viel, was ich zu verarbeiten und zu recht zu rücken hatte, dass es mich nicht wieder aus der Bahn wirft.
Das habe ich aber recht gut gemeistert. Diesen Mittwoch musste ich dann nochmal nach Offenbach, um meine Patientenakte abzugeben und entgültig mein Medikament zu bekommen.

Da waren die letzten zwei Wochen also paar Entscheidungen und momente da hab ich Energie für aufwenden müssen, um klar zu bleiben und mich zu positionieren.

Und um nicht wieder in das alte Grübeln zu verfallen 

Das war genug kognitive Arbeit, da hatte ich dann leider nicht mehr die muse jeden Tag zu meditieren.

Auch wenn es mir wohl gerade dabei geholfen hätte. 

Aber ich bleibe da standhaft und dabei. 

Das Laufen ist auch eine Form der Meditation und Achtsamkeit.

Ich mache schon so vieles besser und anders.

Das zu reflektieren und zu verarbeiten..
Da fiel es mir schwer meinen Geist zu leeren...

Gerade wenn alte Gedankengänge und Muster wieder hoch kommen.

Ich habe dem Papa den Scanner an seinem Drucker eingerichtet, damit der unter Linux läuft, was ich ihm auf seinem Laptop installiert habe. Das habe ich ihm noch gezeigt. 
Das freut mich, wenn es klappt und ihm das Freude macht.

Es ist auch schön, wenn meine Eltern und ich uns jetzt endgültig einig sind bzgl meiner schwester und ich nicht mehr die Sorge haben muss, dass es von einem auf den anderen Tag doch wieder kippt.

Jetzt waren da heute wieder Gedanken bezüglich Arooj...

Sehr viel Einsamkeit. 
Die Sorge wie der nächste Monat wird. 
Wieder nicht ganz zu wissen wo ich hingehöre. 🤷

Ich habe mich aber entschieden, dass ich mein Feuer in mir schüre, mit mir und in mir etwas wachsen lasse, was mich warm hält und antreibt.
Egal ob ich im Endeffekt alleine bin. 
Ich habe die Gewissheit dass ich einen guten Kompass habe, richtig bin, etwas kann, gewisse Dinge gerne mache und Lust habe die Dinge richtig und gut zu machen.

Ich finde schon Orte wo ich hingehöre.

Im realistischsten und unvoreingenommensten Fall gehts Arooj genauso wie mir 🤷‍♂️.

Sie ist mir ja sehr sehr ähnlich.

Aber ich habe häufig genug versucht Brücken zu bauen. Irgendwann sind die Steine auch mal aufgebraucht.
Das schlimmste dabei war ja, dass meine Gutmütig- und Herzigkeit von ihr noch als etwas schlechtes, niederträchtiges und böses ausgelegt wurde. Das hat mich am meisten verletzt.
Ich weiß, dass diese Zuschreibungen nie für mich gegolten haben. Ich habe da anderen zu viel Macht und Deutungshoheit über mich gegeben.
Das ist aber jetzt vorbei.

ich versuche mich durch Meditation innerlich mit Wärme und Geborgenheit zu füllen, um das endgültig hinter mir zu lassen.

ich weiß nicht was in Arooj vorgeht und ich kann es nicht herausfinden. 
An mir liegt es nicht, dass sie diese eigenartigen Unwahrheiten über mich in ihrem Kopf hat.

Es sind nicht meine.

LG Lukas

# Kontaktaufnahme mit Arooj 

Ich hab auch jetzt endgültig beschlossen irgendwie Kontakt mit Arooj aufzunehmen.

Muss das noch irgendwie planen und mir für eine eventuelle E-Mail einen guten und nicht zu langen Text zu überlegen.

Der auch sehr klar ist.

Für Ideen und Unterstützung bin ich offen
Ich darf die Kontaktaufnahme aber auch nicht mit zu viel überfrachten


- Ich habe ja in Vergangenheit den "Fehler" gemacht zu viel zu erklären und zu viel zu reden. 

- Zu wenig Ruhe im Gespräch gehabt, dem Gespräch die Chance zugegeben zu atmen und ihr die Chance zu geben sich auch mal erklären zu müssen. 

- (Jetzt gebe ich mir wieder zu sehr die Verantwortung, das ist auch Aroojs Art in den Themen zu springen und nicht erstmal eins abzuhaken, in dem man Konsens und Dissens klar macht und dann erst weiter geht... Das habe ich ja versucht...Also den Punkt streichen, dass "ich ... Nicht ... Genug". Ist ganz klar nicht meine alleinige Verantwortung.)
- So was muss auch knapp ohne Übererklären angesprochen werden.
- Sehr lieb danke.

Ob ich "bereit" bin weiß ich nicht 100%.

Aber das wird dann ja nie sein.

Die Kontaktaufnahme wäre ja eh nicht sofort/heute/morgen.

Ich will das ja gut durchdenken.

Und mir Zeit lassen, um bereit zu sein. 

Ich würde gerne daraufhin arbeiten und daran feilen, um eben eine linearität hinzubringen und nicht mehr zu sehr in die Schwankungen/extreme zu rutschen.

Das hilft ja hoffentlich in erster Linie mir, um noch stabiler zu werden. 

Ich möchte gerne Schritt für Schritt bereit werden.

Vielleicht steht am Ende des Prozesses aber auch dass ich doch keinen Kontakt aufnehme.

Ziel wäre Ende diesen/Anfang nächsten Monats.

Vielleicht ist Arooj ja beim Adventskaffeekränzechen des bot. Gartens.

Ich vermute aber langsam dass sie die Veranstaltungen meidet da ich da hingehe🤷‍♂️.

Vielleicht hat sie aber auch extrem viel zu tun. 
(Was sehr wahrscheinlich ist. Arooj hat den Hang zum Perfektionismus. Das ist ihre Coping strategie. Überorgansieren (gar nicht wertend) und alles tun.) 

Ich gehe auch davon aus dass meine Angst unbegründet ist dass sie jemanden neues hat. 

Ihre Aussagen im Frühjahr "dass sie bald mit dem Dating anfängt und auf der Suche ist".
War zum einen um mich zu verletzen und um mich wegzustoßen.

Meine Einschätzung ist, dass sie wie ich, nicht so ist.🤷‍♂️

In ihr sehr viel vorgeht und mich auch vermisst und an mich denkt, sonst hätte sie sich nicht so verhalten...

Ich sollte mir dies bezüglich innerlich gewiss sein, dies aber gar nicht nach außen tragen und an sprechen. Das kommt dann eher wie ein Vorwurf rüber bzw. Blockiert es sie.

Aber ja ich weiß nicht was sie wirklich in ihrer Freizeit macht und was ihr Stand ist.🤷‍♂️

Das gilt es herauszufinden.

Ich darf mir meiner selbst und meiner heuristik mit ihr schon gewiss sein. 

Diese Gewissheit wird ein eventuelles Gespräch auch tragen. 

Arooj hat mir ja bevor sie die Sachen geholt hat, ein Gespräch mit jemandem drittes zugesagt

-  mich nicht erklären, nicht entschuldigen (zumindest zu viel), nicht über die Vergangenheit reden
	- bei ihr und bei uns sein, über das schöne, gemeinsame, was mich freut (zb ihre Forschung), die Zukunft und was ich gelernt habe/wir beide gelernt haben
# Nachricht an fredin
## 25-11-17
Ich kann auch den nächsten Abschnitt, da habe ich aber den Übergang noch nicht wirklich geübt.
Also nicht so dass ich es auf 70% spielen könnte.

Der Bedarf auch noch etwas Arbeit damit der richtig klingt.

Insbesondere die Position meiner rechten hat damit die gemuteten teile besser klingen.
Und etwas entspannter in der linken Hand.

Den darauf folgenden Abschnitt kann ich nicht.
Hab ich mir schon mal angeschaut, hat grundsätzliche Ähnlichkeiten zum Intro.
Aber ist rhythmisch etwas anders.
Ich hab's schlicht noch nicht geübt.
Hatte ja eh immer Probleme mir die Reihenfolgen und Übergänge zu merken.
Das war immer mein kryptonite.

Dann folgt ne kurze Melodie die Ist einfach und die kann ich auch.

Es wiederholt sich dann alles mehrfach.

Im Prinzip kann ich daher schon so 60% vom Stück.
Aber halt nicht ansatzweise auf voller Geschwindigkeit.
So auf 80%+ kann ich teile auch komplett sauber spielen.

Da folgt dann noch ein wildes zweistimmiges Gitarren Extremum.
In mehreren Stufen 😅
Die Technik dafür kann ich. Das hört sich dadurch schneller und schwerer an als es ist. 
Es ist halt aber auch trotzdem extrem schnell und auch nicht wenig.
Das schere ist das in langsam zu üben bis man es auswendig kann. 
Denn in langsam hört es sich halt nicht so an wie im Stück.

Das ist im allgemeinen das Problem an dem Stück 🫣.

Der tapping teil vor dem melodischen solo, sind halt 32tl bei 155 bpm.
Das repetitive ist anstrengend, deshalb hab ich generell nicht so Lust tapping zu üben.
Wobei da glaube ich nur alibi getappt wird.
Das ist hauptsächlich Arbeit mit der linken Hand.
## 25-11-21
Ich hab sie gelöscht da die Frage unnötig war, so wie euch zu fragen wie ihr diesen oder jenen Song findet. Keine Ahnung was ich damit bezwecken will. Ebenso dass und wieso ich euch meine Gitarrenaufnahmen geschickt habe.🤷 Weiß nicht was da nicht mit mir stimmt.
Will ich euch irgendwelche Musik aufzwingen? Ne eigentlich nicht. 
Daher denke ich lieber vorher drüber nach ob ich unnötig kommuniziere und etwas Frage. 
Was ist der Zweck und meine Absicht.
Möchte keine Leute in unnötige Kommunikation zwingen.
Ich bin doch wahrscheinlich einfach nur einsam.
Und will etwas in mir umgehen und mich ablenken.

Naja prinzipiell habe ich das fragen wollen, ob euch das gefallen könnte da Freddie beispielweise die harsh vocals bei den unleash the archers songs nicht gefallen hat.
Der Song Apex kommt ja ohne diese aus. Da reichte ja Freddies "ok" aus, um da auch nicht weiter nach zu fragen/zu bohren.
Und im Endeffekt habe ich dann auch wieder sehr viel über mich geredet da ich dann geschrieben habe, was mir an dem Song im Vergleich zur Akustik Version fehlt.
Total ungefragt und mit welchem Zweck.
Will ich wieder Leute überzeugen?
Unnötige Kommunikation. Nur weil ich alleine bin und Arooj nicht mehr nerven und voll labern kann.
Missbrauche ich euch. 
Muss einfach mal lernen alleine klar zu kommen und mir klar überlegen warum ich etwas tue und sage. Kontrolle über mich und meine Absichten habe. 
Und nicht einfach drauf los etwas tue und sage. 
Muss besser lernen wann ich die Grenzen anderer überschreite und deren Bedürfnisse richtig lesen. 

## 25-12-02
Und mir tut dann auch so vieles so sehr leid, auch wenn ich nix falsches gemacht habe. 

Mir tut es ja schon leid wenn ich mal laut, launisch oder auch nur bestimmt war.

Mir tut auch Micro "Fehlverhalten" leid. Auch wenn sie das auch macht. 

Manchmal hatte sie dann auch so das Gefühl so schlecht behandelt zu werden, hat dabei aber null auf ihr micro Verhalten geachtet.

# yt Kommentare
5. Doch sehr möglich... Therapeuten und Ärzte sind auch nur Menschen. Die können zum Teil mit Menschen wie sie es ist nicht so viel anfangen. Da sie zu viel durchdenken und nicht handlungsarm sind. 

Gleichzeitig schwer depressiv und auf der anderen Seite so reflektiert und agitiert.

Das passt nicht so in die ICD X Schubladen, nach denen man lernt zu diagnostizieren.

Ich verstehe ihre Zurückhaltung aus ihrer Erfahrung zu 100%.

# Kinder Namen 
## Mädchen 
- Alva
- Maja 