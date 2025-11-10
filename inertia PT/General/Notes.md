# fast notes
- 
# Arbeit
-  
# Tage infolge Produktiv
Tage prodiktiv gewesen:
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
  `{bash} pdftk *.jpg cat output Dokument_Name.pdf`
- #663399

# git
- Comment in `.gitignore` with # 
- Ausnahmen mit `!`
- wenn Dateien der `.gitignore` hinzugefügt werden, müssen sie auch aus dem chache entfernt werden
  `{git} git rm --cached .obsidian/hotkeys.json`
- - Wenn dies für alle Unterordner gemacht werden soll, dann:
  `{git} git rm -r --cached .obsidian/plugins/\\*`


# Latex Suite
 {trigger: "Brk", replacement: "\\Braket{$0} $1", options: "mA"},
 
$\Braket{\int \frac{ \partial r }{ \partial t }^{2} \, dx}$
$\Braket{\frac{x}{y}^{2}\cdot x^{2}}$

