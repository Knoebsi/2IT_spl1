# Git

<img alt="Git-Logo" src="/images/git.png">

- [How to git](#how_to_git)
	- [Git installieren](#install_git)
	- [Git verstehen](#understand_git)
	- [Wichtige Tipps für Git](#important_hints_for_git)
	- [Wichtige Befehle für die Git Bash](#important_commands_for_gitbash)
	- [Meine Git Erfahrung](#my_git_experience)
- [Kleines Code Beispiel](#small_code_example)
- [Einkaufen](#shopping)
	- [Preistabelle](#table)
	- [Einkaufsliste](#shoppinglist)

<a name="how_to_git"></a>
## How to git



<a name="install_git"></a>
### Git installieren
Hier befindet sich ein _Youtube_ Video, das erklärt, wie man **Git** installiert. <br>
[How to install Git on Windows 10 | Updated 2022](https://www.youtube.com/watch?v=cJTXh7g-uCM)

<a name="understand_git"></a>
### Git verstehen
Hier befindet sich ein _Youtube_ Video, das erklärt, wie man **Git** versteht und verwendet. <br>
[Git and GitHub Tutorial for Beginners](https://www.youtube.com/watch?v=tRZGeaHPoaw)

<a name="important_hints_for_git"></a>
### Wichtige Tipps für Git

1. Git installieren
2. Git verstehen
3. Falls Sie verzweifeln wenden Sie sich an [Ferdinand Knapitsch](https://www.knapitsch.at/)
4. Git verwenden
5. Spaß haben mit Git!!!

<a name="important_commands_for_gitbash"></a>
### Wichtige Befehle für die Git Bash

Diese Befehle wurden von **David Gasparin** _kopiert_, da ich vorige Woche nicht da war. <br>

#### Befehle zum Installieren von Git:

**git config --global user.name “name“** (hinterlegt einen Benutzernamen ) <br>
**git config –global user.email  „Email-Adresse“** (hinterlegt eine Email-Adresse) <br> 
**git config --list** (zeigt zB. Den Benutzernamen oder die E-mali Adresse an) <br>
**git help config** (oder) **git config –help** (Hilfewebsite) <br>
**git restore (Ordner Name)+(Datei Name)** (kann gelöschtes wiederherstellen) <br> 

#### Generelle Git Befehle:

**git status** (zum Überprüfen ob schon geaddet oder gepusht wurde (branch Status)) <br>
**git init** (zu master machen eines Folders) <br>
**git --version** (aktuelle Version von git) <br>

#### Zum pushen auf den Server:

**git add** (lässt git wissen, was man beim nächsten commit dabeihaben will) <br>
**git commit -m „Kommentar(message)“** (Dateien einchecken) <br> 
**git push origin master** (pusht von master die Dateien auf den remote-Server) <br> 

#### Generelle Linux Befehle:

**cd** (change Directory) <br>
**ls -a** (zeigt alles im jetzigen Ordner an) <br>
**ls -la** (zeigt auch versteckte Dateien) <br>
**mkdir** (neuen Ordner erstellen) <br>
**nano** (Text-editor) <br>
**rm** (zum entfernen) <br>
**mv** (zum bewegen von zB. Text-files) <br>
**rmdir** (löscht leeren ordner) <br>
**pwd** (zeigt den aktuellen Pfad an) <br>

<a name="my_git_experience"></a>
### Meine Git Erfahrung

Meine Erfahrung mit Git war für mich persönlich sehr angenehm. Ich kenne mich nun einigermaßen gut aus und werde es in Zukunft hoffentlich mehr verwenden. Es ist eine sehr nützliche Anwendung. <br>
Mit freundlichen Grüßen <br>
Martn Knöbelreiter

<a name="small_code_example"></a>
## Kleines Code Beispiel

```python
#Zahlenraten für Fortgeschrittene

from random import *

def game():
    
    #Zufallszahl generieren
    zahl = randint(1, 20)
    
    #Schätzung resetten
    schaetzung = 0
    
    #Versuche definieren
    versuche = 0
    
    #Die Schätzung des Nutzers bekommen
    while schaetzung != zahl:
        schaetzung = int(input("Raten Sie eine Zahl zwischen 1 und 20: "))
        versuche = versuche + 1
        if schaetzung == zahl:
            print("Gewonnen!")
            print("Sie haben", versuche, "Versuche gebraucht!")
        elif schaetzung < zahl:
            print("Zu niedrig.")
            if schaetzung <= zahl -5:
                print("Sie sind weit entfernt!")
            else:
                print("Sie sind knapp dran!")
        else:
            print("Zu hoch.")
            if schaetzung >= zahl +5:
                print("Sie sind weit entfernt!")
            else:
                print("Sie sind knapp dran!")

#Start des Programms
game()
```

<a name="shopping"></a>
## Gehen Sie Einkaufen

Hier sind Sachen zum einkaufen.

<a name="table"></a>
### Preistabelle
| Produkt        | Preis |
| -------------- | -----:|
| Brot           |    €5 |
| Semmel         | €0.45 |
| HTL Leoben     |  €540 |

<a name="shoppinglist"></a>
### Einkaufsliste
- [x] Semmel
    - [x] Eis
        - [x] Chips
- [ ] Brot
