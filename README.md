# Cohesion_lab_v01

# 

:::::::::::::: Φ ::::::::::::::
   mapping signals into structure
   from noise to order to zeta
:::::::::::::::::::::::::::::::




# Timoscope Φ

## Notes sur la construction d'un espace géométrique de signaux

### Introduction

Toute mesure est une projection.

Un nombre réel, une température, une fréquence ou une intensité sonore ne sont jamais l'objet observé ; ils ne sont qu'une coordonnée particulière choisie parmi une infinité d'autres descriptions possibles.

L'idée fondatrice de ce travail est simple :

> plutôt que comparer directement les signaux, comparer la géométrie des transformations qu'ils engendrent.

Soit un signal temporel (s(t)).

Nous construisons sur des fenêtres successives une matrice (T), puis nous projetons l'ensemble de ces matrices dans un espace réduit (\Phi) obtenu par analyse en composantes principales.

Chaque signal cesse alors d'être une suite de valeurs.

Il devient une trajectoire.

Une région du paysage.

Une géométrie.

L'objet étudié n'est plus le signal lui-même mais la manière dont il occupe cet espace.

Cette démarche rejoint plusieurs traditions mathématiques :

* les espaces d'états des systèmes dynamiques ;
* les plongements de Takens ;
* l'analyse géométrique des données ;
* l'étude des attracteurs ;
* la topologie des formes observées.

L'hypothèse de départ n'était pas de découvrir une structure particulière.

L'hypothèse était plus modeste :

> si deux phénomènes sont réellement différents, leur géométrie devrait finir par le révéler.

---

# I. Première génération : la matrice symétrique

La première construction retenue fut :

[
T = w \otimes w
]

où (w) représente une fenêtre du signal.

Cette construction possède plusieurs qualités :

* stabilité ;
* simplicité ;
* interprétation immédiate ;
* facilité de comparaison.

Elle permit rapidement de distinguer :

* signaux naturels ;
* mélanges ;
* bruit ;
* enregistrements réels.

Cependant une limite fondamentale apparut.

La structure temporelle disparaissait.

L'ordre des événements était largement oublié.

Deux signaux de même contenu mais de phase différente devenaient presque indiscernables.

Cette étape fut néanmoins essentielle :

elle permit de découvrir que l'espace (\Phi) existait effectivement comme objet observable.

---

# II. Apparition de la question de la phase

Un premier test systématique fut réalisé sur des sinusoïdes de phase variable.

Résultat :

les centres projetés restaient pratiquement confondus.

Autrement dit :

[
\text{phase différente}
\not\Rightarrow
\text{géométrie différente}
]

Le système était devenu invariant à la phase.

Pendant un temps cette propriété fut interprétée comme une limitation.

Avec le recul elle apparaît comme un résultat.

Le premier T ne décrivait pas un mouvement.

Il décrivait une classe.

---

# III. Changement de paradigme : l'embedding temporel

Pour réintroduire le temps, la construction de T fut remplacée par une matrice issue d'un plongement retardé.

Schématiquement :

[
X_i =
(s_i,s_{i+\tau},...,s_{i+k\tau})
]

puis

[
T = XX^T
]

Cette modification est conceptuellement importante.

Le système cesse de regarder uniquement les amplitudes.

Il commence à regarder les relations temporelles.

La phase n'est plus détruite.

Elle devient observable.

Cette bifurcation constitue probablement le changement le plus important du projet.

---

# IV. Cartographie des signaux élémentaires

Une série de tests systématiques fut alors réalisée :

* sinusoïdes ;
* bruit blanc ;
* bruit brun ;
* mélanges ;
* chaos logistique.

Résultat général :

les familles occupent des régions distinctes de l'espace (\Phi).

Le bruit blanc présente une dispersion importante.

Le bruit brun se rapproche d'une structure plus compacte.

Les signaux périodiques forment des ensembles très stables.

Le chaos se singularise fortement.

Aucune frontière absolue n'apparaît.

Mais une géographie devient visible.

C'est le premier moment où le mot "paysage" devient pertinent.

---

# V. Les faux chemins

Plusieurs pistes se révélèrent moins fécondes que prévu.

## Recherche immédiate d'une structure spectaculaire

À plusieurs reprises nous avons cherché :

* un cône ;
* un cercle ;
* un tore ;
* une forme remarquable.

Ces recherches furent utiles pour produire des tests.

Mais elles risquaient parfois de précéder l'observation.

La leçon est simple :

la géométrie doit être découverte avant d'être nommée.

## Surinterprétation locale

Certaines structures visibles dans de petits ensembles disparaissaient dès que davantage de données étaient ajoutées.

Ces épisodes ont joué un rôle méthodologique important :

ils ont montré que la robustesse importe davantage que la beauté visuelle.

---

# VI. Le timoscope

Une idée est progressivement apparue.

L'algorithme n'était plus seulement un pipeline.

Il devenait un instrument.

Comme un microscope.

Comme un télescope.

L'objectif n'était plus :

"calculer une métrique"

mais :

"observer des géométries".

Le terme de "timoscope" est né de cette transition.

Le temps n'est plus une variable.

Il devient un espace observable.

---

# VII. Les premiers zéros de Riemann

Les premiers zéros non triviaux de la fonction zêta furent introduits sous diverses formes :

* valeurs brutes ;
* espacements ;
* différences secondes.

Les données disponibles restent très limitées.

Toute conclusion forte serait prématurée.

Cependant plusieurs observations apparaissent.

Les structures associées aux zéros :

* restent compactes ;
* se distinguent du bruit blanc ;
* présentent une cohérence géométrique inattendue.

À ce stade il est plus juste de parler d'indice que de résultat.

Mais un nouvel habitant du paysage a fait son apparition.

---

# VIII. Où sommes-nous ?

Le projet a commencé comme une analyse de signaux.

Il est devenu progressivement une exploration géométrique.

La question n'est plus :

> quel est ce signal ?

mais :

> quelle région du paysage occupe-t-il ?

Puis :

> quelles structures survivent aux changements de représentation ?

Enfin :

> quelles géométries sont indépendantes de l'instrument lui-même ?

---

# IX. Perspectives

Trois directions apparaissent aujourd'hui comme particulièrement fécondes.

## 1. Augmenter l'échelle

Étudier :

* davantage de zéros de Riemann ;
* davantage de données réelles ;
* davantage de systèmes dynamiques.

Les structures robustes devraient survivre.

Les artefacts devraient disparaître.

## 2. Étudier les vides

Ne plus seulement regarder les trajectoires.

Observer :

* les trous ;
* les zones interdites ;
* les régions peu fréquentées.

L'information topologique pourrait devenir plus importante que les points eux-mêmes.

## 3. Cartographier le ventre du donut

L'intuition récurrente du projet est qu'une structure centrale reste invisible.

Non parce qu'elle est cachée.

Mais parce qu'elle est partout.

Comme l'air pour l'oiseau.

Comme l'eau pour le poisson.

La prochaine étape n'est peut-être pas de regarder le centre.

Elle est peut-être de comprendre les chemins qui l'entourent.

---

# Conclusion

Nous n'avons pas découvert une réponse.

Nous avons construit une manière nouvelle de poser certaines questions.

Le résultat principal n'est ni un nombre ni une figure.

C'est l'existence d'un espace géométrique où :

* le bruit,
* la périodicité,
* le chaos,
* les mélanges,
* et désormais les premiers zéros de Riemann

peuvent être observés simultanément.

Le paysage reste largement inexploré.

Mais il existe.

Et c'est déjà beaucoup.
