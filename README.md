# Jeux vidéos & live coding

---

## Présentation du projet

**Nom du jeu** : I love U

**Choix de la machine** : MACINTOSH PLUS

**Langage utilisée** : HyperTalk (HyperCard)

**Outils graphiques utilisés** : outils de création d’images bitmap (1-bit) car je travaillerai en petites tailles

**Emulateur utilisé** : [pce/macplus [E-Maculation wiki]](https://www.emaculation.com/doku.php/pce_macplus)

**Description** :

> *I love U* est un jeu HyperText crée avec HyperCard. Se voulant anachronique afin de confronter des machines anciennes avec des sujets contemporains, *I love U* met en scène une correspondance amoureuse sur les réseaux sociaux. Mais, de qui êtes-vous tombé amoureux ?

---

## Références

- bla bla bla
- bla bla bla 

---

## Points techniques importants

    > **Peut-on graver un jeu en HyperCard sur disquette ?**

oui - techniquement je peux distribuer une pule HyperCard jouable depuis une **disquette 800 KB** (le Mac Plus utilise un *lecteur 3.5" 800 KB*)

/!\ *Attention aux contraintes de taille*

    > **Quelle est ma limite de poids et de nombre d'images ?**

Un *Macintosh Plus* utilise des **disquettes 3,5** en 800 KB (double densité). C'est le format max, il ne lit pas les disquettes haute densité 1,44 MB sans modifications ou émulation.

→ Volume total = **~800 000 octets** (~780-800 KB utilisables réellement sur une image disque)

→ Chaque image (bitmap) est monochrome (1-bit par pixel) est une résolution maximale de **512 x 342 px**.

→ Bitmap B&W simple (512×342, 1 bit/pixel) ≈ **21 944 octets** (~22 KB). Je peux stocker environ **30-35 images si l’espace était uniquement pour des images** (~22 KB × 35 ~ ~770 KB), avant d’atteindre 800 KB.  
→ **Mais** HyperCard ajoute aussi :

- scripts (code),
  
- champs de texte,
  
- boutons,
  
- metadata de la pile,
  
- fonds de cartes réutilisés…  
  **Donc en pratique, viser ~10-20 images est raisonnable** pour garder de la place pour le texte/les scripts et une bonne fluidité du stack.
  

    > **Recommendation d'organisation**

Mettre les images partagées par plusieurs cartes en *backgrounds* (pour réduire les duplications).

Utiliser des zones d’images « tuilées » ou découpées.

Charger des graphismes uniquement quand nécessaire.

---

## Plan de travail

**1. Prototype écriture**

- écriture des dialogues en arborescence
  
- utilisation de Twine pour organiser la narration
  

**2. Prototye Graphique**

- Maquette de l'interface du jeu avec une image du Macintosh
  
- création des images individuelles à importer
  
- récupération des sons de notifications
  

**3. Création du jeu avec HyperCard avec un émulateur**

- Création des différentes cards et backgrounds
  

**4. Exportation**

- création d'une image disque partagée
  
  1. Créer une img disque 800 KB sur mon ordi ("i_love_u.dsk)
    
  2. Glisser cette img dans un émulateur, il le repére
    
  3. [dans l'émulateur] glisser mon fichier MonJeu.stack (le jeu HyperCard) dans la disquette "i_love_u.dsk"
    
  4. [Ejecter la disquette] Finder > glisser la disquette vers la corbeille ou menu > special > eject
    
  5. [dans mon ordi] "i_love_u.dsk" est maintenant exporté
    
- cette image peut être :
  
  - montée dans Floppy Emu
    
  - écrite sur une vraie disquette
    
  - archivée distribuée
    

**5. Plus, itch.io**

- Publier un jeu HyperCard sur itch.io
  
  - fichier .dsk
    
  - readme
    
  - un lien vers un émulateur
    
- Publier et faire une option jouable dans le navigateur
  
  - uploader mon jeu sur Internet Archive
    
  - utiliser leur émulation Macintosh intégrée
    
  - lier cette version depuis itch.io
