# FSEGitTest

Riccardo hat ein GIT Repository erstellt.
Anschließend eine Java Datei erstellt und eine Nachricht platziert. Zusätzlich wurde ein Commit hinterlassen

```
git add Dateiname
git commit -m "Commit nachricht"
```

Diese wurde anschließend auf origin main gepusht.

```
git push
```

Danach wurde Branch "Julian" erstellt und julian hat das Repository auf sein Gerät geklont. Zum klonen wurde ein HTTPS Link verwendet

```
git clone URL
```

Branch Riccardo wurde Online erstellt und Riccardo hat auf diesen Branch mit seiner Dateiversionen gewechselt.

```
git checkout Riccardo - auf Riccardos Gerät
git checkout Julian - auf Julians Gerät
```

Julian hat in seinem Branch eine Änderung (zusätzliche Nachricht hinzugefügt) und diese Änderungen auf origin main gepusht.

Riccardo hat in seinem Branch eine Änderung gemacht ohne von den Änderungen von Julian zu wissen und wollte diese Änderungen auf den origin main mergen.
Dabei ist ein Konflikt entstanden.

Riccardo hat einen neuerlichen

```
git pull

```

durchgeführt und hat die Datei mit dem Konflikt heruntergeladen.
Nachdem der Konflikt aufgelöst (Code wurde in IDE zum laufen gebracht)
wurde konnte der merge auf origin main durchgeführt werden.

Nachdem der Konflikt gelöst wurde konnten wir online mit "Open pull Request" die "Julian Branch" zur main Branch mergen.

Anschließend wurde der Fehler von Julian erneut produziert um die Online Resolve Möglichkeit auszuprobieren.
Siehe Commits

**GitHub Flow Vor und Nachteile**

_Vorteile_

-Einfachheit - Weil GitHub Flow einfach zu verstehen und zu implementieren ist. Gut für kleinere Teams und Projekte

-Schnelle Iteration der Codeveränderungen

-Transparenz - Es ist durchgehen möglich den Entwicklungsstatus zu sehen und den Veröffentlichungsprozess zu verfolgen

_Nachteile_

-Zu viele Köchen verderben den Brei - Wenn viele Mitarbeiter damit arbeiten, kann es schnell unübersichtlich werden. Eher schlecht geeignet für große Projekte
-GitHub Flow setzt auf schnelle Integration, dabei kann es passieren dass nicht fertige Features schlecht isoliert werden und somit zu Instabilität führen.
-Schlecht für monolithische Anwendungen

**Andere Codeversionierungsstrategien**

Während der Recherche bin ich auf Feature Branch Workflow und Trunk Based Development gestoßen.

Feature Branch Workflow die auch auf GIT basiert und ähnlich wie Git Flow ist jedoch ohne die komplexen Release Branches.

Jede Funktion hat ihren eigenen Branch, die Entwickler arbeiten in Ihren Feature Branches und ermöglicht Isolation der einzelnen Funktionen.

Trunk Based Development ist eine radikalere Code-Versionierungsstrategie bei der alle Entwicklungen direkt im Hauptbranch, der oft als Trunk bezeichnet wird.

Alle Entwicklungen, sei es das hinzufügen neuer Funktionen oder das Beheben von Fehlern findet im Hauptbranch statt. Ich persönlich glaube dass diese Art der Codeversionierung hauptsächlich von versierten Programmierern verwendet wird.
