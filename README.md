# M122
* Projekt vom Modul 122
* Skriptsprachen
* Gruppenmitglieder: Alberto Manser

# Einleitung
Dieses Skript ermöglicht das einfache transferieren von Daten mit bestimmten Präfixen in einen Zielordner aus dem Download Ordner und erleichtert somit das sortieren von downloads, es speichert alle bisher ausgeführten Aufträge in einem Log-File ab was ich euch jetzt erklären werde.

# Anwendung
Ein Log- File ist nützlich für verschiedene Programme da man damit ausgeführte Aufträge kontrollieren kann und einen Überblick behalten kann.
ein einfacher Weg ein Log file zu erstellen das sich nicht überschreibt ist wie folgt:
```PS1

<#deklarieren des Namen des Log-Files und des Inhaltes#>
$filename = "name.txt"
$content = "Inhalt welcher in das Log file eingefügt werden soll"

<#Ausfüllen des Log-Files und falls es nicht existiert erstellen des Log-Files#>
"$content" >> $PSScriptRoot\"$filename"

```
Hier wird das Log-File am gleichen ort gespeichert wie das Skript. dies wird durch das "$PSScriptRoot" ermöglicht. ist die Log-File noch nicht existent wird diese erstellt und der Content direkt eingefügt.

# Ausführen
sobald sie dieses Skript geöffnet haben wird der Code ausgeführt, erst müssen sie einen Gütligen Dateipfad zu ihrem Zielordner angeben.
![image](https://github.com/albertomanser/M122/assets/110892537/5f5559fa-c914-462e-89f8-d8d3bc1ad080)

Danach müssen sie den Präfix nach dem gefilter werden soll auswählen. Ein Beispiel wäre: "LB" etc.
![image](https://github.com/albertomanser/M122/assets/110892537/47570d94-4cab-4b14-b62f-7cee06ee5e2a)

sobald sie dies getan haben werden alle Daten mit diesem Präfix transferiert. Um den Auftrag später noch zu suchen können sie beim Speicherort des Skriptes die File namens: "Log.txt" anschauen.
