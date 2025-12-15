# Structure du jeu



### **Structure globale du mini-jeu** :

```
MENU
  ↓
NOTIFICATION
  ↓
CONVERSATION CIRCULAIRE
  (le joueur insiste / rassure)
  ↓
AVEU IMPOSSIBLE
  ↓
COUPURE / PAIEMENT
```

---

### **Cartes HyperCard dont j'ai besoin**

(chaque bloc twine = 1 card, donc j'ai **19 cards**)

**A. CARTES "STRUCTURES"**

1. MENU : `play` & `about`

2. ABOUT : txt explicatif + retour `menu`

3. PLAY : `notification` 

**B. LA CARTE "NOTIFICATION**

4. NOTIFICATION : 
   
   - texte : `j'ai quelque chose à te dire`
   
   - boutons : `tu préfères attendre` & `comment ça ? tout va bien ?` 

**C. CARTES CONVERSATION**

5. CONV

        > toutes les mêmes cartes avec les textes qui changent 

**D. CARTE FINALE**

6. SYSTEM 
   
   - texte : `vous avez dépassé la limite autorisée`
   
   - bouton : `4,99` > retour au `MENU` 

---

### Organisation HyperCard

**Background** (1)

- interface de messagerie 

- 1 grand field pour les textes

- 2, 3 boutons de réponse (réutilisés)

je change seulement le texte du field et la visibilité / destination des boutons

(+ un background pour le menu et pour le about)

**Cards**

- chaque card = un carré twine

- très peu d'images nécessaires 

---



### Ordre de travail

1. Créer les images background 

2. Créer toutes les cartes vides avec leurs noms 

3. Copier-coller les textes Twine dans chaque carte 

4. Créer les boutons de choix 

5. Ajouter les script `go to card "nom"`

6. Tester la boucle 

7. Ajouter la carte de paiement 

8. Tester le jeu final 



---



### Mapping Twine → HyperCard

| **Twine**  | **HyperCard** |
| ---------- | ------------- |
| Passage    | Card          |
| [[lien]    | Bouton        |
| Texte brut | Field         |
| MENU       | Carte Menu    |






