# SOP - AI Drop Servicing - Création de site démo prospect

## Résumé en 1 phrase
Trouver un prospect > générer HTML avec IA > copier dans un nouveau dossier GitHub > commit > attendre 1 min > URL live > appeler le prospect.

---

## ÉTAPE 1 - Trouver le prospect (2-3 min)

**Où chercher :**
- Google Maps : taper le secteur + ville (ex: "detailing auto Toulouse")
- Instagram : chercher le nom de l'entreprise
- Pages Jaunes : vérifier si l'entreprise est encore active

**Infos à noter :**
- Nom exact de l'entreprise
- Ville / secteur géographique
- Services proposés
- Horaires d'ouverture
- Site web ou Instagram
- Numéro de téléphone

**Vérifier que le prospect est actif :**
- Le site web fonctionne-t-il ? (pas de redirection vers site porno ou erreur)
- Le dernier post Instagram date-t-il de moins de 1 an ?
- L'entreprise est-elle listée sur Pages Jaunes ?

---

## ÉTAPE 2 - Générer le HTML avec l'IA (3 min)

**Prompt à donner à l'IA (Perplexity, etc.) :**

```
Crée un fichier HTML complet avec Tailwind CSS via CDN pour un site vitrine de :
- Nom : [NOM ENTREPRISE]
- Service : [TYPE DE SERVICE]
- Ville : [VILLE]
- Horaires : [HORAIRES]
- Site web : [SITE WEB OU EMAIL]

Le site doit avoir :
1. Une hero section avec une grande image de fond Unsplash pertinente, le nom, le service, la ville, les horaires, et un bouton CTA
2. Une section Services avec 3 cartes
3. Une section Contact
4. Un footer

Style : fond sombre (bg-gray-900), texte blanc, bouton bleu, moderne et pro.
Responsive mobile.
```

**Image Unsplash à choisir selon le secteur :**
- Detailing auto : https://images.unsplash.com/photo-1601362840469-51e4d8d58785?w=1920&q=80
- Box CrossFit : https://images.unsplash.com/photo-1517836357463-d25dfeac3438?w=1920&q=80
- Plombier : https://images.unsplash.com/photo-1581094794329-c8112a89af12?w=1920&q=80
- Electricien : https://images.unsplash.com/photo-1621905251189-08b45d6a269e?w=1920&q=80
- Nettoyage industriel : https://images.unsplash.com/photo-1581578731548-c64695cc6952?w=1920&q=80
- Restaurant : https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?w=1920&q=80
- Coiffeur / Barbier : https://images.unsplash.com/photo-1585747860715-2ba37e788b70?w=1920&q=80
- Boulangerie : https://images.unsplash.com/photo-1509440159596-0249088772ff?w=1920&q=80

---

## ÉTAPE 3 - Copier le HTML dans GitHub (3 min)

**Sur GitHub :**

1. Aller sur https://github.com/TenzinTsultrim31/tenzintsultrim31.github.io
2. Cliquer sur le bouton "+" (Add file) > "Create new file"
3. Dans le champ du nom du fichier, taper : `nom-prospect/index.html`
   - Remplacer `nom-prospect` par le nom du prospect en minuscules, avec des tirets
   - Exemple : `elite-auto-detail/index.html`
4. Coller le code HTML généré par l'IA dans la zone d'édition
5. Vérifier que le breadcrumb en haut montre bien : `tenzintsultrim31.github.io / nom-prospect / index.html`
6. Cliquer sur "Commit changes..."
7. Mettre un message de commit : "Add [Nom Prospect] site in nom-prospect/"
8. Cliquer sur "Commit changes"

**ATTENTION - Points importants :**
- Si l'image affichée ne correspond pas au secteur, changer l'URL de l'image dans le code HTML
- Vérifier que les 3 services correspondent vraiment à ce que fait l'entreprise
- Vérifier que les horaires sont corrects

---

## ÉTAPE 4 - Attendre le déploiement (1 min)

- GitHub Pages déploie automatiquement en 30 secondes à 2 minutes
- Vérifier que le site est accessible sur : `https://tenzintsultrim31.github.io/nom-prospect/`
- Si 404, attendre encore 1 minute et rafraîchir

---

## ÉTAPE 5 - Appeler le prospect (1-2 min)

**Hook d'appel (accroche) :**

"Bonjour, je suis [votre nom]. Je suis tombé sur votre entreprise en cherchant [secteur] à [ville] et j'ai remarqué un problème avec votre présence en ligne."

**Démonstration :**

"J'ai pris la liberté de créer une maquette de ce à quoi votre site pourrait ressembler. Je peux vous montrer ?"

→ Envoyer le lien : `https://tenzintsultrim31.github.io/nom-prospect/`

**Proposition :**

"Je peux vous créer un site complet comme celui-ci pour [prix] euros. Intéressé ?"

---

## URLs à retenir

| URL | Description |
|-----|-------------|
| https://github.com/TenzinTsultrim31/tenzintsultrim31.github.io | Repo principal GitHub |
| https://tenzintsultrim31.github.io/ | Page d'accueil du site |
| https://tenzintsultrim31.github.io/nom-prospect/ | Site d'un prospect |
| https://github.com/TenzinTsultrim31/demo-sites | Ancien repo avec templates et workflow guide |

---

## Raccourcis clavier utiles

| Raccourci | Action |
|-----------|--------|
| Cmd+H | Rechercher/Remplacer dans l'éditeur GitHub |
| Cmd+Up | Aller au début du fichier |
| Cmd+Down | Aller à la fin du fichier |
| Cmd+R | Rafraîchir la page |
| Cmd+Shift+R | Rafraîchir en forçant le cache |

---

## Checklist rapide (copier-coller)

- [ ] Prospect trouvé (Google Maps + Instagram + Pages Jaunes)
- [ ] Prospect vérifié actif (site ok, Instagram récent, Pages Jaunes ok)
- [ ] HTML généré avec l'IA (prompt ci-dessus)
- [ ] Image Unsplash choisie (liste ci-dessus)
- [ ] Dossier créé sur GitHub : `nom-prospect/index.html`
- [ ] Code collé et commité
- [ ] Site accessible sur `https://tenzintsultrim31.github.io/nom-prospect/`
- [ ] Appel au prospect effectué

---

## Fichiers du repo

| Fichier | Rôle |
|---------|------|
| README.md | Liste de tous les sites prospects en ligne |
| template/index.html | Template vierge avec placeholders à remplacer |
| SOP/instructions.md | Ce fichier - mode d'emploi complet |
| nom-prospect/index.html | Site d'un prospect |

---

## Questions fréquentes

**Q : Comment changer le nom d'un prospect déjà créé ?**
R : Il faut créer un nouveau dossier avec le bon nom et supprimer l'ancien. Pas de renommage direct possible.

**Q : Le site affiche 404, que faire ?**
R : Attendre 1-2 minutes, puis rafraîchir. Si toujours 404, vérifier que le fichier s'appelle bien `index.html` et qu'il est dans un dossier.

**Q : Comment supprimer un site prospect ?**
R : Sur GitHub, aller dans le dossier du prospect, cliquer sur les 3 points > Delete folder.

**Q : Puis-je avoir plusieurs sites actifs en même temps ?**
R : Oui, chaque dossier = un site actif avec sa propre URL.

---

## Ce fichier est fait pour être redonné à l'IA

Si tu reviens vers moi plus tard, tu peux simplement me redonner ce fichier et dire :
"Voici le SOP de mon workflow AI Drop Servicing, aide-moi à créer un site pour [nom prospect]."

Je saurai exactement quoi faire.
