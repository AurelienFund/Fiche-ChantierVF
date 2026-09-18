# Fiche récap chantier — Arbre des choix (v8 — arbitrages du 22/07/2026 intégrés)

**Mode d'emploi** : ce document décrit exactement ce que l'application affiche et propose.
`[x]` = actif aujourd'hui · `[ ]` = inactif. Pour demander un changement : modifiez les cases,
raturez, annotez, ajoutez des lignes — puis renvoyez-moi le fichier (ou dictez-moi les changements
en message). Chaque modification validée sera reportée dans l'application.

---

## 1. Règles générales

- [x] **Page vierge à l'ouverture.** Si une fiche est sauvegardée dans le navigateur, un bandeau propose
  « Reprendre cette fiche » ou « Repartir de zéro ». La sauvegarde n'est écrasée qu'à la première vraie saisie.
- [x] **Sauvegarde automatique continue** de la fiche en cours (locale au navigateur).
- [x] **Mise à jour des listes** : les nouveaux choix livrés avec une version de l'outil s'ajoutent
  automatiquement à la base déjà enregistrée dans le navigateur, sans effacer les choix ajoutés
  personnellement ni ressusciter ceux retirés volontairement (depuis le 30/07/2026).
- [x] **Pas de doublons** : deux écritures d'un même choix (accents, majuscules, espaces — « pietement »,
  « Piètement », « PIETEMENT ») sont reconnues comme une seule entrée. Le nettoyage est automatique au
  chargement, l'orthographe de référence est conservée, et les fiches déjà enregistrées sont réalignées.
- [x] **Toutes les listes déroulantes** proposent systématiquement :
  - « **À définir** » — choix à faire plus tard (affiché **en rouge** à l'impression) ;
  - « **—** » — sans / non concerné (affiché tel quel, en neutre, à l'impression) ;
  - puis les choix de la base, triés par fréquence d'usage ;
  - « ＋ Ajouter un choix… » / « － Retirer un choix… » pour enrichir sa base personnelle.
- [x] **Déclinaisons de matière identiques dans toutes les sections** : choisir « MDF » dans Caisson
  ouvre exactement les mêmes choix que « MDF » dans Façade (voir §3).
- [x] Les sections affichées dépendent du **type de mobilier** (voir §2).
- [x] **Deux façons d'ajouter un type** dans la liste « Type » :
  - « ＋ Ajouter un type **détaillé**… » → agencement complet (caisson, façade, poignées, tringle, LED),
    comme Dressing ou Placard ;
  - « ＋ Ajouter un type **simple**… » → aménagement ou élément simple (matière & finition, quincaillerie
    spéciale, LED, composition, notes), comme Tête de lit, Escalier ou Étagère.
  Le mode choisi est mémorisé dans votre base et suit le partage de base entre collègues.
- [x] Import de devis PDF : analyse locale (sans IA), calibrée sur les devis de l'atelier.
- [x] Import de fiche PDF : les données de réimportation sont incluses **de façon invisible** dans le PDF
  (aucun code ni page supplémentaire à l'impression) ; la fiche revient à l'identique.
- [x] **Fusion de plusieurs fiches** : si une fiche est déjà ouverte, l'import propose
  **« Ajouter à la suite »** ou **« Remplacer »**. En ajout, les zones s'empilent dans l'ordre et
  les **n° de dossier et de devis se cumulent** (« 00697 + 00701 », « DEV-…-00697-V2 + DEV-…-00701-V2 »),
  sans répéter un numéro déjà présent. Les champs du cartouche déjà remplis sont conservés, les vides
  complétés par la fiche ajoutée ; les généralités se cumulent sans doublon.
- [x] **Import de devis** tenu à jour des évolutions : reconnaît les types Escalier, Habillage mural et
  Plan de travail ; l'électroménager des cuisines (fournisseur Cojer / client, éléments) ; la matière,
  le fournisseur et les usinages du plan de travail ; l'aspect de peinture (mat / satiné / brillant) ;
  la quincaillerie spéciale (Hawa, escamotable, galandage, charnières hors standard).
- [x] **Réorganisation libre de la fiche** :
  - **↑ / ↓ sur chaque zone** (dans son bandeau) pour la remonter ou la descendre ;
  - **↑ / ↓ sur chaque agencement** pour le déplacer dans sa zone ;
  - **« ↔ Déplacer vers… »** sur chaque agencement : liste les autres zones et y transfère l'agencement
    avec toutes ses données (la zone d'arrivée s'ouvre automatiquement). Le sélecteur n'apparaît que
    s'il existe au moins deux zones.
  - « Dupliquer » insère la copie juste après l'original.
  L'ordre choisi est celui de la fiche imprimée et de la sauvegarde.
- [x] **Lisibilité de la fiche imprimée** : titre souligné en gras sans encart marron ; client, adresse et
  contact en gras et plus grands ; accès dans un cadre bien visible ; **toutes les valeurs choisies en
  gras**.
- [x] **Icône propre à l'outil** (caisson à poignées laiton, tons de la fiche) : visible dans l'onglet,
  les favoris, les onglets épinglés et sur l'écran d'accueil des téléphones. Elle est intégrée au
  fichier HTML, il n'y a aucune image à héberger à côté.
- [x] **Nom du PDF automatique** : à l'impression, le navigateur propose « **Fiche - nom du chantier.pdf** »
  (repli sur l'adresse si le nom est vide). Fonctionne aussi avec Ctrl+P.
- [x] **Notes et points d'attention séparés** sur chaque agencement :
  - **Notes** (précisions de fabrication) → imprimées **en gras, juste sous la composition** ;
  - **⚠ Points d'attention** → **encadré rouge**, texte rouge gras, titre plus petit et non gras.
  L'import de devis range ses repérages (hors lot, non fourni, à confirmer, prévoir renfort, en option,
  variante…) dans les **points d'attention**.

**Cartouche chantier** (en-tête de la fiche) :

- [x] Nom du chantier — *rétabli (coché « je veux » dans vos retours) ; rempli automatiquement à l'import d'un devis*
- [x] Client — *rétabli ; rempli automatiquement à l'import d'un devis*
- [x] **N° de dossier** — à renseigner, imprimé dans le cartouche *(nouveau)*
- [x] **N° de devis** — à renseigner, imprimé dans le cartouche *(nouveau)*
- [x] Adresse chantier (sert aussi de titre à la fiche et au nom du fichier JSON)
- [x] Contact sur place
- [x] Date
- [x] Accès (Plain-pied / Escalier / Ascenseur / Monte-charge / Grue nécessaire / Autre) + précision
- [x] Généralités (texte libre, imprimé en tête de fiche)

---

## 2. Sections affichées PAR TYPE de mobilier

Colonnes : **Liv** = mode de livraison · **Cais** = caisson · **TF** = type de façade (+ remplissage) ·
**Mat** = matière & finition · **Quinc** = quincaillerie spéciale (case à cocher) · **Poig** = poignées · **Tri** = tringle ·
**LED** · **Élém** = éléments intégrés · Composition, Notes et Points d'attention = toujours affichés
pour tous.

| Type | Liv | Cais | TF | Mat | Quinc | Poig | Tri | LED | Élém |
|---|---|---|---|---|---|---|---|---|---|
| Dressing | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Bibliothèque | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | ✔ | ✔ |
| Placard | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Cuisine *(+ bloc Électroménager)* | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| **Îlot** *(nouveau, identique à Cuisine)* | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Lit superposé | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | ✔ | ✔ |
| Banquette | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | · | ✔ |
| Bureau | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | **✔** | ✔ | ✔ |
| Salle de bain | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| **Plan de travail** *(nouveau)* | **·** | **·** | **·** | **·** | **·** | **·** | **·** | **·** | ✔ |
| Autre | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Tête de lit | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Escalier** | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Garde-corps** *(nouveau)* | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Habillage mural** | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Coussin / Tapisserie** | **·** | · | · | **·** | **·** | · | · | **·** | ✔ |
| **Porte** *(nouveau)* | ✔ | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Verrière** *(nouveau)* | ✔ | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Façade** *(nouveau)* | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Habillage** *(nouveau)* | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| Soubassement | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| Tablette | · | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| Console cache-clim | · | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Étagère** | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
| **Piètement** | **·** | · | · | ✔ | **·** | · | · | **·** | ✔ |
| **Manteau de cheminée** | **·** | · | · | ✔ | **·** | · | · | **·** | ✔ |
| **Miroir** | **·** | · | · | · | · | · | · | **·** | **·** |

✔ = affiché · **·** = masqué.

**Arbitrages intégrés (22/07/2026)** : quincaillerie retirée sur Piètement et Manteau de cheminée ·
livraison retirée sur Tablette, Soubassement, Console cache-clim et Tête de lit · LED conservée sur
Étagère / Tablette / Soubassement mais retirée sur Banquette · tringle retirée sur Bibliothèque,
Lit superposé, Banquette et Bureau · type **« Porte » supprimé** de la liste (et le champ béquillage
avec lui — signalez-moi si c'était involontaire).

**Cas particulier Miroir** — sections affichées :

- [x] Finition miroir : À définir / — / Clair / Vieilli
- [x] Épaisseur : À définir / — / 4 mm / 6 mm / 8 mm
- [x] Spécifications (cases à cocher) : Filmé · Perçage · Arrondi · Biseauté · Cadre
- [x] Composition / dimensions (un miroir par ligne, ex : « Miroir salle d'eau L. 1070 x H. 1700 »)
- [x] Notes
- [x] Spécifications ajoutées : **Biseauté** · **Cadre**

---

## 3. Déclinaisons par MATIÈRE (identiques dans Caisson, Façade et Éléments intégrés)

Quand une matière est choisie, voici ce qui s'ouvre — **quel que soit l'endroit** :

### [x] MDF
→ Finitions (cases multiples) : **Brut** · **Apprêté** · **Peint**
→ si Peint : Fournisseur peinture (Ressource / Little Greene / Farrow & Ball / Tollens / …) → Réf. couleur
→ **+ Aspect : Mat / Satiné / Brillant / Velours**

### [x] Mélaminé — et — [x] Stratifié
→ Fournisseur (Unilin / Egger / Polyrey / Fenix / Formica / Abet Laminati / …) → Réf. décor
(les réfs sont mémorisées par fournisseur dans votre base : U222 blanc écru, F0547 Papyrus…)

### [x] Chêne massif · Pin massif · **Plaqué chêne** · Plaqué bois · Aggloméré plaqué · CP marine · Autre
→ Finition : Brut / Peint / Vernis / Huilé (Rubio)
→ si Peint : Fournisseur peinture → Réf. → **Aspect : Mat / Satiné / Brillant / Velours**
→ si Vernis : Mat / Satiné / Brillant / Blanchi
→ si Huilé (Rubio) : teinte Pure / White / Natural / Smoke / Black / Chocolate
*(nouveau : « Plaqué bois » ouvre désormais la finition — vos devis disent « plaqué chêne, finition
huilée », c'était impossible à saisir avant)*

**Arbitré** : listes de matières Caisson et Façade conservées séparées ; pas de matière ajoutée.
(Les déclinaisons restent, elles, strictement identiques partout.)

---

## 4. Détail des autres sections

### Caisson
- [x] Construction : Standard IKEA / Standard à recouper / Sur mesure
- [x] si **Sur mesure** → Matériau → déclinaisons de matière (§3)
- [x] sinon (standard ou à définir) → Fournisseur panneau → Réf. décor
- [x] Bulle « autres possibilités / précisions »

### Façade
- [x] Type de façade : Simple / Cadre / Cadre + remplissage / Rainurée / Cintrée / Vitrée / Autre *(« Cadre + rainure » retiré)*
- [x] si **Cadre + remplissage** → Remplissage : Tissu / Tapisserie / Cannage / Miroir / Autre
  - Tissu ou Tapisserie → Fournisseur (Elitis / Pierre Frey / Casamance / Nobilis / …) → Réf.
  - Miroir → teinte (Clair / Vieilli) + pose (Percé / Filmé / Avec cadre)
- [x] Matière → déclinaisons (§3)

### Quincaillerie spéciale *(refonte)*
- [x] **Case à cocher « Quincaillerie spéciale »** : décochée par défaut. Tant qu'elle est décochée,
  aucune ligne n'apparaît et rien n'est imprimé — le standard atelier (charnières Blum amorties,
  glissières classiques…) reste implicite via les Généralités et n'encombre plus la fiche.
- [x] Bloc placé **sous les poignées et la tringle** (formulaire et impression), pour ne pas décaler
  la position habituelle des poignées quand il est absent.
- [x] Une fois cochée, liste des quincailleries **non standard** : Charnière noire / Charnière invisible
  (Tectus) / Charnière 165° / Rail Hawa escamotable (Hawa Concepta) / Rail Hawa coulissant (Hawa Junior) /
  Système escamotable / Porte-manteau escamotable / Coulissant à galandage / Vérin - piston /
  Serrure - fermeture / Passe-câble / Autre
- [x] Pour chaque ligne : **Réf. / modèle** (liste, enrichissable) + **Réf. complémentaire** (champ libre :
  réf. exacte, dimension, coloris) + Finition (Nickelé / Noir / Inox / Laiton)
- [x] Plusieurs lignes possibles ; import de devis : détecte Hawa, escamotable, galandage, charnière noire/invisible/165°

### Porte *(nouveau)*
Type simple, avec un bloc propre placé avant la matière :
- [x] **Type de porte** : Basique / Phonique / Coupe-feu / Âme pleine
- [x] **Ferrage** : Anuba / Paumelle invisible / Charnière invisible
- [x] Puis **matière & finition** (toutes les matières, dont Plaqué chêne, avec leurs déclinaisons)

### Verrière *(nouveau)*
Type simple (matière & finition) plus :
- [x] **Case « Verre »** → **4 mm / 6 mm / 33² / Miroir** (+ bulle de précisions)

### Façade et Habillage *(nouveaux)*
- [x] Types simples : matière & finition, quincaillerie spéciale, LED, éléments intégrés,
  composition, notes et points d'attention. Pas de mode de livraison.

### Garde-corps
Type simple (matière & finition, quincaillerie spéciale, LED, éléments intégrés, composition, notes),
sans mode de livraison — plus un bloc qui lui est propre :
- [x] **Case à cocher « Verre »**, décochée par défaut
- [x] Une fois cochée → **Modèle de verre** : Feuilleté / Trempé / Armé (+ bulle de précisions)
- [x] Import de devis : « garde-corps », « rambarde », « main courante » reconnus ; « verre feuilleté /
  trempé / armé » coche la case et renseigne le modèle

### Coussin / Tapisserie
Type simple, avec ses seuls choix propres :
- [x] **Matière** : Tissu / Papier peint
- [x] **Fournisseur** : Florence / Mimilo
- [x] **Modèle** : champ libre (nom du modèle, coloris, référence)
- [x] Bulle de précisions + composition + notes + points d'attention
- [x] Masqués : mode de livraison, caisson, façade, **finition**, **quincaillerie**, poignées, tringle, **LED**

### Plan de travail
Disponible **en type d'agencement** (liste « Type ») **et en élément intégré** (« + Ajouter une ligne »),
avec exactement les mêmes choix dans les deux cas :
- [x] Matière : Dekton / Corian / Marbre / Granit / Quartz / Céramique / Inox / Bois massif / Stratifié / Autre
- [x] **Si Bois massif** → **Essence** (Chêne / Hêtre / Frêne / Noyer) et **Épaisseur** (20 / 30 / 40 mm)
  *remplacent* fournisseur et référence, **+ Finition** : Brut / Peint / Vernis / Huilé (Rubio)
  — avec les mêmes déclinaisons que partout (peinture : fournisseur, réf. et aspect ; vernis : mat,
  satiné, brillant, blanchi ; huile : teinte Rubio)
- [x] **Sinon** → **Modèle** (liste enrichissable, saisi **avant** le fournisseur) → **Fournisseur**
  (Granico / HMS / Autre) → **Épaisseur** (8 / 12 / 20 / 30 mm)
- [x] Cases à cocher : **Rainurage · Cuve · Robinet · Prises · Plaque** — chaque case cochée fait
  apparaître **en dessous un champ « Réf. »** (réf., dimension, modèle), pré-rempli à **« À définir »**
  (en rouge) tant qu'il n'est pas renseigné, et imprimé entre parenthèses
- [x] Bulle de précisions + composition + notes
- [x] Sections caisson / façade / poignées / tringle / LED / livraison masquées (sans objet)

### Électroménager — cuisines uniquement *(nouveau)*
- [x] Bloc placé **sous le caisson et la façade** (même base d'affichage que tous les agencements),
  aussi bien dans le formulaire qu'à l'impression. Disponible sur **Cuisine** et **Îlot**.
- [x] Case à cocher **« Électroménagers »**
- [x] Si cochée → Fournisseur : **Cojer / Client direct / Autre**
- [x] Puis cases à cocher des éléments fournis : Plaque · Four · Hotte · Frigo · Lave-vaisselle ·
  **Congélateur** · Micro-ondes · **Cafetière** · Évier · Cave à vin · Autre — chaque case cochée fait apparaître **en dessous un champ
  « Réf. »** (marque, modèle), pré-rempli à **« À définir »** (en rouge) tant qu'il n'est pas renseigné,
  et imprimé entre parenthèses : « Four (Bosch HBG675) », « Hotte (À définir) » en rouge
- [x] Bulle de précisions. Si non cochée, la fiche imprime « Électroménager non fourni »

### Poignées
- [x] **Case à cocher « Poignées », cochée par défaut** (comme la tringle) : décochée, **plus aucun champ
  à renseigner** (pas même la bulle de précisions) et la fiche imprime simplement « Sans poignée ». Le choix « Sans poignée » a donc disparu de la liste des types,
  la case le remplace ; les fiches enregistrées avec l'ancien choix sont converties automatiquement.
- [x] Type : Bouton de porte / Prise de doigt / Push-pull / Fournie par le client
- [x] Bouton de porte → **réf. en liste** (Viefe / LMC / Corston + votre base, enrichie par les imports) + finition (Laiton / Noir mat / Inox / Chromé / Autre)
- [x] Prise de doigt → **forme uniquement** (Pente à 25° / Profilé → réf. profilé) : ni finition ni nombre
- [x] Push-pull → couleur (Noir / Blanc / Gris)
- [x] Nombre de poignées

### Tringle
- [x] Interrupteur Tringle → finition : Laiton / Inox / Noir

### Éclairage LED
- [x] Interrupteur LED → Couleur (Blanc chaud 2700K / Blanc neutre 4000K / Blanc froid 6000K / RGB-variable)
  + Emplacement (Joues à la verticale / Sous meubles hauts / Intérieur niche / Corniche / Sous étagères / Autre)

### Mode de livraison
- [x] Monté / Partiellement monté / À plat (démonté)

### Éléments intégrés à l'agencement
- [x] Deux boutons d'ajout, comme pour les types :
  - **« + Élément simple »** → matière & finition, quincaillerie spéciale, LED, composition, notes ;
  - **« + Élément détaillé »** → caisson, façade, poignées, tringle… (agencement complet).
  Le mode choisi prime sur le type : un élément « Tablette » créé en détaillé garde ses sections.
- [x] Chaque élément ouvre sa propre mini-fiche (mêmes règles de matières et de finitions que ci-dessus)

### Tête de lit *(complété)*
En plus de la matière & finition, deux blocs optionnels :
- [x] **Case « Remplissage »** → Type : Tissu / **Papier peint** / Tapisserie / Cannage / Miroir / Autre
  - Tissu, papier peint ou tapisserie → Fournisseur (Nobilis, Elitis, Pierre Frey…) → Réf.
  - Miroir → teinte + pose
- [x] **Case « Cadre »** → Matériau (mêmes matières que les façades) → puis les menus associés :
  fournisseur et réf. pour un mélaminé ou stratifié, finitions (brut / peint + aspect / vernis / huilé)
  pour un bois ou un MDF

---

## 5. Historique des arbitrages

- **22/07/2026** — retraits par type (quincaillerie, livraison, LED, tringle — cf. §2), suppression du
  type Porte, specs miroir Biseauté/Cadre, réf. bouton en liste, finitions poignées simplifiées,
  « Plan de travail » retiré des emplacements LED et « Sous étagères » ajouté, « Cadre + rainure » retiré,
  listes de matières conservées séparées.
- **30/07/2026** — ajout des **n° de dossier et n° de devis** au cartouche ; **quincaillerie → quincaillerie
  spéciale** (case à cocher, liste hors standard, réf. complémentaire libre) ; ajout du **plan de travail**
  comme type et comme élément intégré (matière, fournisseur, réf., usinages) ; bloc **ELECTRO fourni** en
  première ligne des cuisines (fournisseur + éléments cochés).
- **28/08/2026 (fin 2)** — mise en page unifiée : **quincaillerie spéciale sous les poignées** et
  **électroménager sous caisson / façade** (formulaire et PDF). Nouveau type **Îlot** (identique à
  Cuisine). Électroménager : ajout de **Congélateur** et **Cafetière**. Plan de travail : le **modèle**
  se renseigne **avant** le fournisseur et n'en dépend plus.
- **28/08/2026 (fin)** — ajout de **« Plaqué chêne »** dans toutes les listes de matières (caisson et
  façade, avec finitions) ; nouveaux types simples **Façade**, **Habillage**, **Verrière** (case Verre :
  4 mm / 6 mm / 33² / Miroir) et **Porte** (type basique / phonique / coupe-feu / âme pleine, puis
  ferrage anuba / paumelle invisible / charnière invisible, puis matière et finition).
- **28/08/2026 (suite)** — prise de doigt : **« Pente à 25° »** au lieu de 30°. Les bases et fiches
  déjà enregistrées sont migrées automatiquement (pas de doublon avec l'ancienne valeur).
- **28/08/2026** — éléments intégrés ajoutables en mode **simple** ou **détaillé** ; **tête de lit** dotée
  d'une case **Remplissage** (tissu, papier peint…) et d'une case **Cadre** (matériau + menus associés).
- **27/08/2026 (correctifs import)** — deux défauts corrigés sur la réimportation de fiches PDF :
  (1) `opacity:0` faisait *supprimer* les données du PDF à l'impression au lieu de les rendre invisibles ;
  (2) les champs restés à leur valeur par défaut revenaient **vides** au lieu de « À définir »
  (mode de livraison et type de poignée notamment). Lecture du bloc rendue tolérante (espaces, césures,
  marqueur de fin perdu). Version applicative passée à **v9** pour signaler à l'import qu'un PDF vient
  d'une version antérieure.
- **27/08/2026 (fin 10)** — **fusion de fiches** : une fiche PDF peut désormais être ajoutée à la suite
  de la fiche en cours ; n° de dossier et de devis cumulés (deux, trois ou plus).
- **27/08/2026 (fin 9)** — poignées : la **prise de doigt** n'affiche plus ni finition ni nombre ;
  **case décochée** = plus aucun champ ni note, seulement « Sans poignée » à l'impression.
- **27/08/2026 (fin 8)** — ajout du type simple **Garde-corps** avec une case **Verre** optionnelle
  (modèles Feuilleté / Trempé / Armé).
- **27/08/2026 (fin 7)** — ajout d'une **icône** intégrée au fichier (favicon SVG + PNG 32 px + icône
  180 px pour l'écran d'accueil mobile) et de la couleur de thème.
- **27/08/2026 (fin 6)** — le PDF est proposé sous le nom **« Fiche - nom du chantier.pdf »**
  (caractères interdits nettoyés ; repli sur l'adresse, puis « sans nom »).
- **27/08/2026 (fin 5)** — ajout du type simple **Coussin / Tapisserie** (matière Tissu ou Papier peint,
  fournisseur Florence ou Mimilo, modèle en champ libre) sans livraison, finition, quincaillerie ni LED.
- **27/08/2026 (fin 4)** — séparation **Notes** / **Points d'attention** : deux champs distincts par
  agencement, notes en gras sous la composition, points d'attention en encadré rouge au titre allégé.
- **27/08/2026 (fin 3)** — les poignées passent sur une **case à cocher cochée par défaut**, sur le modèle
  de la tringle : décocher masque les détails et imprime « Sans poignée ». Import de devis adapté
  (« sans poignée », « pas de poignée » décochent la case).
- **27/08/2026 (fin 2)** — plan de travail en **bois massif** : ajout de la **finition** (brut, peint,
  vernis, huilé) avec toutes ses déclinaisons, identiques à celles des autres sections. Les matières
  minérales (Dekton, Corian, marbre…) n'affichent pas de finition. Import de devis adapté.
- **27/08/2026 (fin)** — cocher un usinage ou un électroménager pré-remplit sa référence à
  « À définir » (rouge dans le formulaire et à l'impression) : plus d'oubli silencieux. Le champ se vide
  au clic pour la saisie et revient à « À définir » s'il est laissé vide.
- **27/08/2026 (suite)** — plan de travail : le **bois massif** ouvre **essence** (chêne, hêtre, frêne,
  noyer) et **épaisseur** (20 / 30 / 40 mm) au lieu de fournisseur et référence ; **épaisseur**
  (8 / 12 / 20 / 30 mm) ajoutée pour toutes les autres matières. Import de devis adapté (essence et
  « ép. 30mm » reconnues).
- **27/08/2026** — réorganisation complète : zones déplaçables (↑ / ↓) et agencements transférables
  d'une zone à l'autre via un sélecteur « Déplacer vers… ».
- **26/08/2026 (fin)** — le PDF n'affiche plus le bloc de code en bas de page : les données de
  réimportation y sont désormais invisibles (texte blanc 1 pt, sans page ni titre dédiés), la
  réimportation fonctionne à l'identique. Parseur d'import réaligné sur toutes les évolutions
  (types récents, électroménager, plan de travail, aspect de peinture, quincaillerie spéciale).
- **26/08/2026 (suite)** — **tringle rétablie sur Bureau** (case à cocher + finition) ; ajout du type
  simple **Habillage mural** ; **Escalier** confirmé présent (ajouté plus tôt le même jour).
- **26/08/2026** — ajout du type **Escalier** (structure identique à Tête de lit : matière & finition,
  quincaillerie spéciale, LED, éléments intégrés, composition et notes ; ni caisson ni façade ni poignées,
  livraison masquée). Ajout du **choix du mode à la création d'un type** (simple ou détaillé), mémorisé
  dans la base.
- **12/08/2026** — refonte de l'en-tête de la fiche imprimée (titre souligné, informations client en gras
  et plus grandes, accès encadré) ; valeurs choisies en gras dans toute la fiche ; notes d'agencement en
  rouge encadré ; boutons ↑ / ↓ pour réordonner les agencements ; **aspect de peinture** (mat / satiné /
  brillant / velours) ajouté après la référence, en façade comme en caisson.
- **06/08/2026 (correctif)** — dédoublonnage des listes : les variantes d'écriture d'un même choix
  fusionnent (comparaison sans accents ni casse), à l'affichage comme à l'import de devis et à l'ajout
  manuel d'un choix.
- **30/07/2026 (correctif)** — les nouveaux choix par défaut n'apparaissaient jamais chez qui avait déjà
  utilisé l'outil : la base enregistrée dans le navigateur écrasait les listes livrées (c'est pourquoi
  « Plan de travail » restait invisible). Les listes fusionnent désormais. Case « ELECTRO fourni »
  renommée **« Électroménagers »**. Champ **Réf.** sous chaque case cochée (électroménagers et usinages
  du plan de travail).
- **22/07/2026 (correctif)** — convention actée : dans ce document, **[x] = « je veux cet élément »**.
  En conséquence, les champs **Nom du chantier** et **Client** sont **rétablis** dans le cartouche,
  l'impression et l'import de devis.

## 6. Ce que vous pouvez me demander à partir de ce document

Répondez simplement, par exemple : « §2 : coche “retirer quincaillerie sur piètement” ; §3 : fusionne
les listes de matières ; §4 poignées : ajoute le type “Coquille” ». Je mets à jour l'application et je
vous renvoie ce document actualisé — il sert de référence commune avec vos collègues (vous pouvez le
déposer dans le dépôt GitHub à côté du `index.html`).
