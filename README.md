# Git

<img alt="Git-Logo" src="/images/git.png">

- [How to git](#how_to_git)
	- [Git installieren](#install_git)
	- [Git verstehen](#understand_git)
- [Wichtige Tipps für Git](#important_hints_for_git)
- [Meine Git Erfahrung](#my_git_experience)
- [Kleines Code Beispiel](#small_code_example)

<a name="how_to_git"></a>
## How to git



<a name="install_git"></a>
### Git installieren
Hier befindet sich ein Youtube Video, das erklärt, wie man Git installiert. <br>
[How to install Git on Windows 10 | Updated 2022](https://www.youtube.com/watch?v=cJTXh7g-uCM)

<a name="understand_git"></a>
### Git verstehen
Hier befindet sich ein Youtube Video, das erklärt, wie man Git versteht und verwendet. <br>
[Git and GitHub Tutorial for Beginners](https://www.youtube.com/watch?v=tRZGeaHPoaw)

<a name="important_hints_for_git"></a>
## Wichtige Tipps für Git

1. Git installieren
2. Git verstehen
3. Falls Sie verzweifeln wenden Sie sich an [Ferdinand Knapitsch](https://www.knapitsch.at/)
4. Git verwenden
5. Spaß haben mit Git!!!

<a name="my_git_experience"></a>
## Meine Git Erfahrung

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
