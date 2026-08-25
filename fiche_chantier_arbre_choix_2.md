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
- [x] Import de devis PDF : analyse locale (sans IA), calibrée sur les devis de l'atelier.
- [x] Import de fiche PDF : via le bloc de données imprimé en dernière page (réimport à l'identique).
- [x] **Ordre des agencements modifiable** : boutons **↑ / ↓** sur chaque agencement pour le remonter ou le
  descendre dans sa zone (le bouton est grisé en haut / bas de liste). « Dupliquer » insère la copie
  juste après l'original.
- [x] **Lisibilité de la fiche imprimée** : titre souligné en gras sans encart marron ; client, adresse et
  contact en gras et plus grands ; accès dans un cadre bien visible ; **toutes les valeurs choisies en
  gras** ; **notes en rouge dans un encadré**.

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
**LED** · **Élém** = éléments intégrés · Composition & Notes = toujours affichés pour tous.

| Type | Liv | Cais | TF | Mat | Quinc | Poig | Tri | LED | Élém |
|---|---|---|---|---|---|---|---|---|---|
| Dressing | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Bibliothèque | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | ✔ | ✔ |
| Placard | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Cuisine *(+ bloc ELECTRO en 1re ligne)* | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Lit superposé | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | ✔ | ✔ |
| Banquette | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | · | ✔ |
| Bureau | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | · | ✔ | ✔ |
| Salle de bain | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| **Plan de travail** *(nouveau)* | **·** | **·** | **·** | **·** | **·** | **·** | **·** | **·** | ✔ |
| Autre | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ |
| Tête de lit | **·** | · | · | ✔ | ✔ | · | · | ✔ | ✔ |
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

### [x] Chêne massif · Pin massif · Plaqué bois · Aggloméré plaqué · CP marine · Autre
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
- [x] Une fois cochée, liste des quincailleries **non standard** : Charnière noire / Charnière invisible
  (Tectus) / Charnière 165° / Rail Hawa escamotable (Hawa Concepta) / Rail Hawa coulissant (Hawa Junior) /
  Système escamotable / Porte-manteau escamotable / Coulissant à galandage / Vérin - piston /
  Serrure - fermeture / Passe-câble / Autre
- [x] Pour chaque ligne : **Réf. / modèle** (liste, enrichissable) + **Réf. complémentaire** (champ libre :
  réf. exacte, dimension, coloris) + Finition (Nickelé / Noir / Inox / Laiton)
- [x] Plusieurs lignes possibles ; import de devis : détecte Hawa, escamotable, galandage, charnière noire/invisible/165°

### Plan de travail *(nouveau)*
Disponible **en type d'agencement** (liste « Type ») **et en élément intégré** (« + Ajouter une ligne »),
avec exactement les mêmes choix dans les deux cas :
- [x] Matière : Dekton / Corian / Marbre / Granit / Quartz / Céramique / Inox / Bois massif / Stratifié / Autre
- [x] Fournisseur : Granico / HMS / Autre → puis réf. (liste enrichissable par fournisseur)
- [x] Cases à cocher : **Rainurage · Cuve · Robinet · Prises · Plaque** — chaque case cochée fait
  apparaître **en dessous un champ « Réf. »** (réf., dimension, modèle), imprimé entre parenthèses
- [x] Bulle de précisions + composition + notes
- [x] Sections caisson / façade / poignées / tringle / LED / livraison masquées (sans objet)

### Électroménager — cuisines uniquement *(nouveau)*
- [x] **Première ligne du bloc Cuisine** : case à cocher **« Électroménagers »**
- [x] Si cochée → Fournisseur : **Cojer / Client direct / Autre**
- [x] Puis cases à cocher des éléments fournis : Plaque · Four · Hotte · Frigo · Lave-vaisselle ·
  Micro-ondes · Évier · Cave à vin · Autre — chaque case cochée fait apparaître **en dessous un champ
  « Réf. »** (marque, modèle), imprimé entre parenthèses : « Four (Bosch HBG675) »
- [x] Bulle de précisions. Si non cochée, la fiche imprime « Électroménager non fourni »

### Poignées
- [x] Type : Bouton de porte / Prise de doigt / Push-pull / Fournie par le client / Sans poignée
- [x] Bouton de porte → **réf. en liste** (Viefe / LMC / Corston + votre base, enrichie par les imports) + finition (Laiton / Noir mat / Inox / Chromé / Autre)
- [x] Prise de doigt → forme (Pente à 30° / Profilé → réf. profilé) + finition
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
- [x] Lignes libres de type : Tablette / Bureau / Miroir / Piètement — chacune ouvre sa propre
  mini-fiche (mêmes règles de sections et de matières que ci-dessus)

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
