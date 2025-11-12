# fast notes
- 
# Arbeit
-  
# Tage infolge Produktiv
Tage prodiktiv gewesen:
||||/ ||||/ ||||/ ||||/
|

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
- #663399

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
`youtubelinkt`+`?t=MMmSSs`⟹`youtubelink`+`?t=17m18s` ⟹ https://youtu.be/Yz9Bj9kEtKc?si=17m18s
Mann muss die Zeit wohl in Sekunden umrechnen 🤷 und ohne Angabe der Zeiteinheit.
`youtubelinkt`+`?t=Sekunden`
17m 18s ⟹ 17 \* 60 + 18 = 1038
`youtubelinkt`+`?t=1038`
https://youtu.be/Yz9Bj9kEtKc?t=1038
Und man muss den ganzen Murks bis zum ersten Fragezeichen entfernen:
https://youtu.be/Yz9Bj9kEtKc?si=umUGQ2rElxZL_YgD

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

