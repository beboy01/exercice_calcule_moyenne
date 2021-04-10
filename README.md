# exercice_calcule_moyenne
# C’est fait, votre cousin est informé que vous êtes nanien et vous suggère de l’aider avec son exercice suivant:  Exercice : Calcul de moyenne:  Pour faciliter le calcul de # # moyenne et la prise de décision, l’on vous sollicite pour mettre en place un script qui automatise cette tâche. La tâche est expliqué ci-dessous: Le programme permet au #professeur de saisir les notes d’un étudiant, calcul la moyenne et affiche si l’étudiant est Admis ou Recalé.  NB: Tous les étudiants ont 03 notes Les note sont des réel #comprise entre 0 et 20 Un étudiant est déclaré admis si la moyenne de ce dernier est supérieure ou égale à 14   Pour ce projet, il sera question pour vous de jouer le rôle du #formateur. Vous allez enregistrer votre séance d’explication suivie du codage et héberger votre vidéo sur youtube afin de permettre à votre cousin de visualiser votre #explication au temps de fois qu’il le souhaite.

```python
def Moyenne():
    li=[]
    note=0
    s=0
    m=0
    np=0
    for i in range(3):
        note= float(input(f"Entrez la note numero {i} de l'etudiant"))
        li.append(note)
    for i in range(3):
        np=np +1
        s=s+ li[i]
        m=s/np
    if m>0 and m<14:
        print("L'Etudiant n'a pas eu la moyenne, donc il est ètre Récalé")
    elif m>14 and m<=20:
        print(f"Bravo l'etudiant à une moyenne de {m} donc il est déclarée Admin !")
    else:
        print("La moyenne ne doit pas ètre inferieur à 0 et Supérieur à 20 ")
     #ici le ressayer est facultatif c'est moi mème qui à ajouter cette partie afin de permette au professeur s'il veut calculer une autre moyenne  
    essaye= input("Voulez-vous ressayez (y=oui ou n= non).? ")
    while essaye =='o' or essaye == 'y':
        Moyenne()
    if essaye == 'N' or essaye =='n':
        exit()
Moyenne()
```
