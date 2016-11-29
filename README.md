# BPMN
= business process model and notation

[Playlist Youtube 1](https://www.youtube.com/playlist?list=PLSkCdDPNwJTCH2i9dj0DhmQ85ZDxLvR-Q)

## 4 modèles de diagramme

[Vidéo Youtube au bon moment](https://youtu.be/ouL01C-LRww?t=8m28s)

### Diagramme d'orchestration

Définition de la séquence d'un processus, du début à la fin, avec les différents éléments de flux (évènements, activités, passerelles).

### Diagramme de collaboration

Représentation graphique des interactions entre processus, en précisant les messages échangés.

### Diagramme de conversation et diagramme de chorégraphie

Interactions et échanges également, mais représentations différentes. Moins utilisés.

## Approches de réalisation

### Hiérarchique : Top/Down
Niveau de détail croissant.
D'abord, processuses de façon macroscopique. Processuses parents.
Ensuite, détails. Sous-processuses.

## Critères de qualité

Attention :
- Trop général, ne sert à rien pour l'opérationnel
- Trop détaillé, devient inutilisable

Questions à se poser pour un processus :
- Objectif
- Déclencheur(s)
- Résultats, fins possibles
- Activités (flux, exceptions, contrôle, fins)
- Acteurs
- Interactions (flux de message)

Critères de réussite d'un diagramme :
- Conformité à la norme
- Cohérence
- Clarté
- Complétude

## Vocabulaire

### "Activité"

Action avec début et fin.
Rectangle aux bordures arrondies.
Deux types : tâche et sous-processus.
Exemples : saisir commande, préparer commande, servir client, encaisser client

### "Flux d'orchestration"

Flèche.

### "Evènement"

Cercle.

Déclencher :
- **Départ** = obligatoire et unique.
- Bordure fine

Interrompre :
- **Fin** = obligatoire, mais peut être multiple.
- Bordure épaisse

Influencer :
- **Intermédiaire** = optionnel
- Bordure double

Types (non obligatoire) :
Début :
- Réception d'un message (enveloppe)
- Timer (horloge)
- Règle de gestion (feuille A4)
- Evènements multiples, pentagone = un seul evènement déclenche, croix = tous les évènements pour déclencher)
- Captation d'un signal (triangle) (d'un autre processus)

Fin :
- Message
- Signal
- (Multiple)
- Terminaison (cercle plein) -> met fin à TOUT le process

Intermédiaire :
- Timer
- Réception ou envoi message
- Réception ou envoi signal
- Lien de réception ou envoi (flèche) (pour couper diagramme - juste graphique)


### "Passerelle"

Losange.
Chemins parallèles ou alternatifs.

Pour indiquer chemin par défaut, trait oblique sur flèche.

#### Exclusive
Par défault, alternatif : passerelle **exclusive**.
Vide, ou avec croix.
1/ Diviser le flux en fonction d'une condition
2/ Reconstituer le flux

#### Parellèle
Avec un "plus".
Tous les trucs se font.

#### Inclusion
Cercle vide.
Un, certains ou tous les chemins.

#### Exclusive évènementielle
Pentagone dans un cercle.

#### Complexe
Astérisque.
Quand ne peut pas être expliquée.

Article intéressant : http://edutechwiki.unige.ch/fr/Bpmn_2.0

(fichier non terminé)
