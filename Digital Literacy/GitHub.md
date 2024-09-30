# Git - Open Souce Projekt zur Versionskontrolle

## Was ist ein Commit?

Unter dem Beriff 'commit' kann man sich einen Speicherpunkt, in Form eines Kommentares, vorstellen.
Bei der Erstellung eines Commites wird der aktuelle Stand eines Projektes gespeichert, um diesen Stand später aufrufen zu können falls nötig. Um eine Bildliche Vorstellung einem Commits zu haben, könnte man diesen als eine Art Backup/Wiederherstellungpunkt zu sehen.

## Was ist ein Branch?

Stell dir vor, du entwickelst eine Webseite, die bereits Live ist. Nun könntest du neue Features natülich auf dem Main-Branch entwickeln, diese sind dann Live auf der Webseite zu sehen. Um dies zu vermeiden, erzeugt man einen Branch. Ein Branch ist eine Art Kopie des aktuellen Mainbranches. Das bedeutet in dem Momante, in dem du einen Branch erzeugst, wird der aktuelle IST-Zustand, deiner Webseite, in den neuen Branch übernommen.  
Dadurch ist es möglich ein neues Feature direkt in deinem jetzigen Stand der Seite aufzubauen ohne dass sich die Live Webseite ändert.

## Was ist Mergen?

Unter dem Begriff Merge versteht man den Zeitpunkt in dem man den Branch wieder mit dem Main-Branch zusammenführt. An diesem Punkt wird alles was ihr in eurem Branch an Änderungen durchgeführt habt in den Main-Branche implementiert. Am Ende des Merge-Vorganges **muss Commitet** werden.

## Git Commands

|command|Beschreibung|
|---|---|
|git init|Erzeuge/Inizialisiere ein git Repository. Ein Projekt in dem ein git-Repo erzeugt wurde steht unter der Beobachtung von git. Das bedeutet, dass git jegliche Änderungen den den Enthaltenen Datein bemerkt und diese Änderungen speichert.|
|add .|Der `git add` Befehl sorgt dafür, dass git alle Änderungen übernimmt.|
|git commit -m "text"|Nach dem Befehl `git add.` verlangt git, dass ein Commit gemacht wird. Der Erste Commit in einem neuen Projekt sollte immer ein `inital commit` sein.|
|git checkout -b "branchName" oder git switch -c "branchName"|Beide Befehle erzeugen einen neuen Branch. `checkout -b` ist der alte Befehl und wurde von `switch -c` ersetzt. Beide Befehle funktionieren.|
|git clone ...|Mit dem `git clone` Befehl clonst du Repos von GitHub auf dein lokales System um diese bearbeiten zu können.|
|git pull |Bei der Bearbeitung eines Repos auf deinem lokalen System, kann es sein, dass jemand das Repo auf GitHub bereits bearbeitet hat. Um deine geclonte Version auf den neusten Stand zu bringen musst du den pull Befehl einmal ausführen. Der `git pull` Befehl ist eine **Kombination aus `git fetch` und `git merge`!**|
|git push -u origin main|Der `git push` Befehl ist der "upload" auf GitHub. Hierbei muss beim ersten Push `-u origin` + `branchName` angegeben werden.|
|git fetch|Änderungen/Commits, die von Anderen in ihrenen eigenen Branches vorgenommen wurde, werden nicht gepullt. Um diese Informationen zu erhalten gibt es den `git fetch` Befehl.|
|git merge|Der `git merge` Befehl ist das zusammenführen von unterschiedlichen Branches. Bei einem Merge können Merge-Konflikte auftreten, wenn sich beide Versionen voneinander unterscheiden. Diese Merge-Konflikte lassen scih entweder direkt auf GitHub oder in VS-Code lösen.|
|git Status|Mit dem `git Status` Befehl sieht man den Status der Dateien. Dateien, die noch nicht mit dem add Befehl|
|git log|Mit dem `git log` Befehl erhält man Einsicht, die Commit History (Wer, Wann welchen commit gesetzt hat. Ebenfalls sieht man hier den Ccommit Hashtag, mit dem man Projekte zurück setzen kann.|

[mehr Infos zu Git](https://www.atlassian.com/git/tutorials/syncing)

