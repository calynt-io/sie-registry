# SIE — REGISTRY

## Pré-enregistrement public des modèles de prédiction

> Ce document désigne, de façon datée et publique, quel modèle sert de
> référence pour chaque marché et chaque périmètre. Toute modification
> future passe par un commit horodaté sur ce dépôt — jamais de désignation
> rétroactive.
>
> **v1.0 — désignations initiales du 6 juillet 2026.**

---

## La règle de promotion (fait foi, publiée avant toute décision)

Un changement de champion (un challenger prend la place publique) n'est
possible que si TOUS ces critères sont vrais simultanément, évalués
UNIQUEMENT aux fenêtres fixes ci-dessous :

- **Fenêtres d'évaluation** : 1-15 janvier · trêve internationale de mars ·
  intersaison de juillet · trêve d'octobre.
- **P1** : n ≥ 100 matchs appariés **LIVE** (jamais backtest), challenger
  inchangé (même hash) sur toute la période.
- **P2** : écart de Brier moyen (challenger − champion) ≤ −0,005.
- **P3** : p-value Holm-ajustée < 0,05 (test unilatéral) ET bootstrap
  concordant (intervalle de confiance ajusté entièrement négatif).
- **P4** : garde-fou de calibration — ECE du challenger ≤ ECE du champion + 0,01.
- **P0 (nouveau, 22/07/2026)** : le pipeline de maintenance automatique du
  challenger (ré-entraînement, backfilling walk-forward, publication du
  hash) doit être fonctionnel et documenté — un challenger statistiquement
  significatif mais dont le pipeline n'est plus maintenu (ex. cerveau
  abandonné après un changement de méthode) est disqualifié,
  indépendamment de P1 à P4.

Si plusieurs challengers remplissent ces critères à la même fenêtre, le
meilleur écart de Brier moyen gagne.

**Rétrogradation** : symétrique — un champion n'est rétrogradé que par un
challenger qui remplit P1 à P4 (même mécanisme, vu de l'autre côté).

**Frein d'urgence** (non-statistique) : si le Brier glissant du champion
sur 100 matchs devient pire que le plancher naïf (fréquences de base), ce
n'est plus de la variance — gel immédiat, retour au dernier état sain,
note publique dans ce dépôt.

**Montée de version** (le même modèle, estimation corrigée — ex. Poisson
v1 → v2) : autorisée uniquement aux fenêtres, sur preuve walk-forward,
suivie d'une surveillance live de 50 matchs avec rollback automatique si
le Brier live de la nouvelle version dépasse l'ancienne (en shadow) de
+0,02. Ce n'est pas une promotion au sens ci-dessus : l'identité du
champion ne change pas, seule son estimation est corrigée.

---

## Périmètre INTERNATIONAL (labo — non commercialisé)

| Marché | Modèle affiché | Hash d'état (SHA-256) | Désigné le | Prochaine revue |
|---|---|---|---|---|
| 1X2 | `elo-davidson-intl-ens-mle` | `sha256:0db2195fc648fe872d53ab5ee9a579b3de17f7812499d6499efe1cdff229c98f...` | 2026-07-22 (remplace elo-davidson-wc-v1), renommé le 24/07/2026 (hash corrigé, voir "Renommage CdM → International") | trêve d'octobre 2026 |
| Score exact | `elo-davidson-intl-poisson` | `sha256:124b87ed808e2955e0eace897c4bfa02c00c4ba3c88...` | 2026-07-06 (gelé le 01/07/2026), renommé le 24/07/2026 | trêve d'octobre 2026 |
| Over/Under | `elo-davidson-intl-poisson` | `sha256:124b87ed808e2955e0eace897c4bfa02c00c4ba3c88...` | 2026-07-06 (gelé le 01/07/2026), renommé le 24/07/2026 | trêve d'octobre 2026 |
| Distribution des buts | `elo-davidson-intl-poisson` | `sha256:124b87ed808e2955e0eace897c4bfa02c00c4ba3c88...` | 2026-07-22 (première désignation), renommé le 24/07/2026 | trêve d'octobre 2026 |

### Note de gouvernance — pourquoi v1 est champion

`elo-davidson-wc-v1` est champion **parce que désigné avant l'existence
des challengers**, pas parce qu'il est mesuré meilleur. C'est l'argument
central de ce dispositif : couronner un challenger sur la seule base d'un
backtest ou d'un petit échantillon live violerait notre propre règle
(P1 : n≥100 matchs live). Le meilleur challenger courant est documenté
ci-dessous, avec son statut réel — jamais maquillé en champion tant que
la règle n'est pas remplie.

### Challengers enregistrés (roster GELÉ — aucun ajout hors fenêtre)

- **1X2** : `elo-davidson-wc-gd` (hash `sha256:be2f3e1da9e3f841b2df2db3dfee43b813f9afac78b...`)
  — ⭐ **challenger en tête** au 6 juillet 2026, statistiquement non
  significatif à ce stade (échantillon live encore trop petit pour une
  décision — voir seuils ci-dessous) · `elo-davidson-wc-ens`
  (hash `sha256:81877bd1c69ce8294b414842aff918b6548f7603eae...`) ·
  `elo-davidson-wc-v2` (hash `sha256:e3d1c53a8beaedc6b0c9fd78b2497d8a5769dab19d1b6c97589b58e6d2bc3ce4...`)
  — challenger officielle (recalibrée), actif dans l'arène depuis la
  création du registre mais omis par erreur jusqu'au 21/07/2026, corrigé
  lors d'un audit de cohérence ·
  famille λ/w24/hfa (l10-l14, w24, w24t, hfa, hfat) : statut R&D interne,
  hors course à la promotion (micro-variantes, écarts indétectables sur
  tout horizon réaliste).
- **Score exact / Over-Under** : **`elo-davidson-wc-poisson-v2`** — statut
  inchangé depuis le 06/07/2026 (n=88, Brier −0,0075, IC 95% négatif,
  résultat directionnel non probant). **Mise à jour du 21/07/2026** :
  backfilling walk-forward complet sur les 104 matchs de la CdM effectué
  le 20/07/2026, cerveau branché en production le 21/07/2026.

  **Note d'intégrité** : le hash publié ici entre le 06/07 et le 21/07
  correspondait à un état antérieur à la correction de la contamination
  méthodologique du 11-12/07 — jamais republié entre-temps. Confirmé par
  vérification des métadonnées du fichier (créé le 06/07, écrasé sur
  place le 12/07, aucune copie antérieure conservée). Le hash ci-dessus
  reflète l'état décontaminé actuellement en production.

  ⚠️ Le prédicteur qui l'alimente ne couvre que la Coupe du Monde — le tournoi
  étant terminé, aucune nouvelle donnée live ne viendra plus enrichir son
  échantillon tant qu'il n'est pas repointé vers un autre calendrier
  international. Le seuil n≥100 requis pour toute promotion reste donc
  hors de portée en l'état.

  **`elo-davidson-wc-negbin`** — challenger ajouté le 13/07/2026, gel
  effectif le 15/07/2026, ajout au registre le 16/07/2026 : exception
  documentée et datée au cycle trimestriel formel, cohérente avec le
  rythme de développement actif du labo pendant le tournoi. Mécanisme :
  distribution Negative Binomial (r=8) remplaçant Poisson standard pour
  mieux répartir P(0-0)/P(1-1). Sweep + holdout confirmés (gain +0,0011
  sweep, +0,0020 holdout en Brier).

  **`elo-davidson-wc-poisson-mle`**, **`elo-davidson-wc-negbin-mle`**,
  **`elo-davidson-wc-ens-mle`** — migration vers estimation MLE (espace
  log, gradient analytique, régularisation ridge), construits le
  19/07/2026, en production depuis. Enregistrés ici avec retard le
  21/07/2026, suivant le même principe de transparence que l'exception
  `negbin` du 16/07 : le retard est nommé explicitement plutôt que
  silencieux.

### Décision de promotion du 22 juillet 2026

Première vraie promotion de champion depuis la création de ce registre,
à l'issue du protocole complet P0 à P4.

- **1X2 — `elo-davidson-wc-ens-mle` remplace `elo-davidson-wc-v1`** :
  écart de Brier moyen −0,0280, p=0,0002 (Holm-ajustée), IC 95%
  bootstrap [−0,0425 ; −0,0126] (entièrement négatif), ECE 0,0644 contre
  0,0834 pour l'ancien champion. Les quatre critères P1-P4 sont remplis
  simultanément ; P0 (pipeline fonctionnel) l'est également —
  ré-entraînement automatique, backfilling walk-forward et publication
  du hash tous vérifiés opérationnels pour `ens-mle`.
- **Distribution des buts — première désignation officielle** :
  `elo-davidson-wc-poisson` désigné champion sur ce marché, qui n'avait
  jamais été formellement enregistré dans ce document avant ce jour.
- **`elo-davidson-wc-ens` (ensemble classique) — NON promu malgré des
  statistiques favorables** : significatif sur Over/Under (écart
  −0,0093, p<0,0001) et sur Distribution des buts (écart −0,0052,
  p=0,0004), donc P1-P4 remplis sur ces deux marchés — mais disqualifié
  par la nouvelle règle P0, son pipeline de maintenance n'étant plus
  fonctionnel (abandonné au profit de la migration MLE sans bascule
  propre du pipeline de production).
- **`elo-davidson-wc-ens-mle` — NON promu sur Score exact / Over-Under**
  malgré la promotion sur 1X2 : échoue P3 sur ces marchés (meilleur
  candidat, p=0,0643 pour un seuil Holm requis de 0,0083 à ce rang).
- **`elo-davidson-wc-poisson-v2` — statut challenger inchangé** :
  meilleur Brier brut sur Distribution des buts (0,5031) parmi tous les
  candidats testés, mais jamais soumis au protocole formel P0-P4 sur ce
  marché précis — reste challenger documenté, aucune promotion tant que
  le test complet n'est pas mené.

## Renommage CdM → International (24 juillet 2026)

**Pourquoi** : les cerveaux du roster CdM sont en réalité entraînés sur
tout l'historique international (~50 000 matchs, toutes compétitions
depuis 1872), pas seulement la Coupe du Monde. Ce renommage est
anticipatif, en vue du repointage du collecteur vers la prochaine
fenêtre internationale mondiale (21 septembre-6 octobre 2026), prévu à
partir du 22 août 2026.

**Méthode** : filiation explicite, jamais de renommage en place — les
19 cerveaux `-wc-*` originaux restent intacts (fichiers, hashs, lignes
de prédictions historiques), jamais modifiés ni supprimés. 19 nouveaux
cerveaux `-intl-*` ont été créés comme identités successeurs, avec de
nouveaux hashs calculés sur le même contenu (sauf correction du bug
d'intégrité ci-dessous).

| Cerveau historique (`-wc-*`) | Cerveau canonique (`-intl-*`) | Note |
|---|---|---|
| `elo-davidson-wc-v1` | `elo-davidson-intl-v1` | |
| `elo-davidson-wc-v2` | `elo-davidson-intl-v2` | |
| `elo-davidson-wc-l10` | `elo-davidson-intl-l10` | |
| `elo-davidson-wc-l11` | `elo-davidson-intl-l11` | |
| `elo-davidson-wc-l12` | `elo-davidson-intl-l12` | |
| `elo-davidson-wc-l13` | `elo-davidson-intl-l13` | |
| `elo-davidson-wc-l14` | `elo-davidson-intl-l14` | |
| `elo-davidson-wc-w24` | `elo-davidson-intl-w24` | |
| `elo-davidson-wc-w24t` | `elo-davidson-intl-w24t` | |
| `elo-davidson-wc-hfa` | `elo-davidson-intl-hfa` | |
| `elo-davidson-wc-hfat` | `elo-davidson-intl-hfat` | |
| `elo-davidson-wc-gd` | `elo-davidson-intl-gd` | |
| `elo-davidson-wc-poisson` | `elo-davidson-intl-poisson` | |
| `elo-davidson-wc-poisson-mle` | `elo-davidson-intl-poisson-mle` | hash corrigé le 24/07 — voir note d'intégrité ci-dessous |
| `elo-davidson-wc-poisson-v2` | `elo-davidson-intl-poisson-v2` | |
| `elo-davidson-wc-negbin` | `elo-davidson-intl-negbin` | |
| `elo-davidson-wc-negbin-mle` | `elo-davidson-intl-negbin-mle` | hash corrigé le 24/07 — voir note d'intégrité ci-dessous |
| `elo-davidson-wc-ens` | `elo-davidson-intl-ens` | |
| `elo-davidson-wc-ens-mle` | `elo-davidson-intl-ens-mle` | hash corrigé le 24/07 — voir note d'intégrité ci-dessous |

**Note d'intégrité — bug de nommage MLE corrigé** : découvert le
24/07/2026 en préparant ce renommage, les 3 cerveaux migrés vers la
vraie MLE le 19/07 (`poisson-mle`, `negbin-mle`, `ens-mle`) avaient un
champ `model_key` interne erroné dans leur fichier d'état JSON
(pointant vers le nom classique sans le suffixe `-mle`) — une erreur
de construction jamais détectée depuis leur création, sans conséquence
pratique connue (le nom de fichier et toutes les entrées en base
utilisaient déjà le bon nom complet). Corrigé le 24/07/2026, entraînant
un nouveau hash pour ces 3 cerveaux :

- `poisson-mle` : ancien hash erroné `sha256:65d610142822c336a24cc2345bcda030c261556c5cdb3dc1bd9ac7915308757b...` → nouveau hash correct `sha256:aba0aa5fe360d675b5176cfe50e8fb340158c22c8b92a55707bcdb2bc09e0848...`
- `negbin-mle` : ancien hash erroné `sha256:7222a586cdc0e3952a8707cbba45153458a9d7fa0681668848fb34d31c6deb6e...` → nouveau hash correct `sha256:d071c78bfd40c2c31a1851388aaf6799862786ea872738ef166c565588ec74fa...`
- `ens-mle` : ancien hash erroné `sha256:3c585db4807060eb74ab44b79762409734a9d074c6814c0856aea15b46ec407f...` → nouveau hash correct `sha256:0db2195fc648fe872d53ab5ee9a579b3de17f7812499d6499efe1cdff229c98f...` (ce dernier était déjà publié comme champion 1X2 depuis le 22/07/2026).

### Les trois seuils n (jamais confondus)

| Seuil | Fonction | Ce qu'il autorise |
|---|---|---|
| n ≥ 20 | Décrire | Couleurs internes (arène privée) uniquement |
| n ≥ 50 | Montrer | Première mention publique d'un challenger — obligatoirement accompagnée d'un intervalle de confiance et de la mention "non significatif" si applicable |
| n ≥ 100 | Décider | Seuil plancher de toute promotion (règle ci-dessus) |

---

## Périmètre PREMIER LEAGUE (produit, lancement 21 août 2026)

> **Section soldée le 03/08/2026.** Les désignations Premier League en
> vigueur vivent désormais dans la section « Périmètre CLUBS » ci-dessous
> (`poisson-mle-club-pl`, les 4 marchés). Cette section est conservée
> telle quelle pour la traçabilité : elle documente le premier champion
> historique du produit et les engagements pré-enregistrés pris avant
> l'existence de son remplaçant.

| Marché | Modèle affiché | Hash d'état | Désigné le | Statut au 03/08/2026 |
|---|---|---|---|---|
| 1X2 | `elo-davidson-v1` | `sha256:93cf543817f538b96141f95d43ed5026458dab7a0f74a0b6b6f5f2fc2d4ac6cc` | 2026-07-06 (gelé et backtesté en juin 2026) | **Remplacé** par `poisson-mle-club-pl` (désignation sur backtest walk-forward — remplacement d'un champion jamais confronté au live par un modèle mesuré meilleur sur le même historique ; voir périmètre CLUBS) |
| Score exact | *désignation engagée* | — | au plus tard le 14 août 2026 | **Engagement tenu le 03/08/2026** (11 jours d'avance) : `poisson-mle-club-pl` |
| Over/Under | *désignation engagée* | — | au plus tard le 14 août 2026 | **Engagement tenu le 03/08/2026** (11 jours d'avance) : `poisson-mle-club-pl` |

**Note technique** : le champ de hash de `elo-davidson-v1` s'appelait
`state_hash` (et non `integrity_hash` comme côté international) — une
différence de convention de nommage entre les deux pipelines, sans
conséquence sur la validité du mécanisme lui-même. Les deux garantissent
la même chose : toute modification manuelle de l'état invalide le hash.
Cette convention `state_hash` reste une spécificité historique de ce seul
gel : le périmètre CLUBS utilise `integrity_hash` (voir sa note de
nommage).

**Pré-enregistrer une date de désignation avant même d'avoir le modèle
final est déjà un acte de pré-enregistrement** : cette date ne pourra pas
être repoussée sans qu'un commit visible ne l'explique. Les deux
engagements du 14 août ci-dessus ont été tenus le 03/08/2026.

---

## Périmètre CLUBS — championnats classiques (produit, lancement 21 août 2026)

> Quatre premiers cerveaux du moteur Poisson-MLE club, geles le
> 03/08/2026 a l'issue de l'ablation {decay x rho} du 02-03/08/2026 et de
> son interpretation par consultation croisee. Architecture commune aux 4
> championnats (meme moteur, meme vraisemblance) -- la demi-vie de
> ponderation temporelle est un hyperparametre continu calibre PAR LIGUE
> (infini admis = pas de decay), exactement le meme statut que nu de
> Davidson ou le rating d'entree Elo des equipes promues, deja calibres
> par ligue ailleurs dans ce registre. Rho (Dixon-Coles) absent des 4
> modeles sans exception -- rejete a l'ablation dans chaque championnat.
>
> **Note de nommage** : le champ de hash de ce perimetre s'appelle
> `integrity_hash` (comme le perimetre international), PAS `state_hash`
> (specificite historique du seul premier gel PL 1X2 `elo-davidson-v1`,
> jamais reconduite depuis). Choix fait pour eviter une 3e convention
> dans un meme perimetre.

| Marché | Modèle affiché | Demi-vie decay | Hash d'état (integrity_hash) | Cutoff | Désigné le |
|---|---|---|---|---|---|
| 1X2 / Score exact / Over-Under / Distribution des buts (Premier League) | `poisson-mle-club-pl` | 730 jours | `sha256:e48f03d246d10451ca903ffed633123069c298cb6373151eccad1bed142983bc` | 2026-08-03 | 2026-08-03 |
| 1X2 / Score exact / Over-Under / Distribution des buts (La Liga) | `poisson-mle-club-la-liga` | 390 jours | `sha256:9c4f622c44afc8750e85de62fe6dc62f9997177b78ec736e2cc5e62b957394cd` | 2026-08-03 | 2026-08-03 |
| 1X2 / Score exact / Over-Under / Distribution des buts (Ligue 1) | `poisson-mle-club-ligue-1` | ∞ (baseline, aucun gain detecte) | `sha256:0ee4429ebb0f7a2741951df88972d8c1bb6a61a5abd38f68eafcc7244bfd3312` | 2026-08-03 | 2026-08-03 |
| 1X2 / Score exact / Over-Under / Distribution des buts (Bundesliga) | `poisson-mle-club-bundesliga` | ∞ (baseline, aucun gain detecte) | `sha256:4c24c842cd53c8ac993fcc180759cb7c22ca73834376f47a3d99b963ad870838` | 2026-08-03 | 2026-08-03 |

### Résultats de l'ablation ayant motivé ces désignations

- **Premier League (`decay730`)** : Δ Score exact = -0,00136 vs baseline,
  p<0,0001 (Holm), stable aux 3 seuils d'eligibilite N=5/10/15, tous les
  garde-fous de non-inferiorite respectes (1X2, Over/Under, Distribution).
- **La Liga (`decay390`)** : Δ Score exact = -0,00130 vs baseline,
  p=0,0018 (Holm), stable aux 3 seuils. `decay730` egalement significatif
  a l'etape Holm (gain moindre que `decay390`) -- confirme le critere
  inter-ligues (gain de type decay franchit Holm dans >=2 championnats
  independants, sous les deux lectures possibles du critere).
- **Ligue 1 (baseline)** : aucune cellule significative a aucun seuil.
  Meilleur candidat (`decay730`) plafonne a p=0,087-0,121 selon le seuil.
  IC bootstrap 95% du Δ vs baseline : [-0,00079 ; +0,00007] -- exclut la
  taille d'effet mesuree en PL/La Liga (~-0,0013). Test formel de
  difference inter-ligues (Δ_Ligue1 - Δ_PL) : p=0,0046, rejette
  l'hypothese d'un effet de meme taille masque par un simple deficit de
  puissance (reserve : le Δ PL compare est celui de sa cellule gagnante,
  donc potentiellement gonfle en magnitude par selection -- winner's
  curse). Les donnees restent compatibles avec un effet nul comme avec un
  effet reel plus petit qu'en PL/La Liga -- indistinguables sur cette
  fenetre. Reexaminable a une fenetre pre-enregistree future, jamais en
  rouvrant la presente ablation.
- **Bundesliga (baseline)** : une seule cellule a atteint la
  significativite (`decay730_rho`, seuil N>=15 seulement, p=0,0024) mais
  rejetee par le garde-fou Over/Under -- rejet de fond, pas un deficit de
  detection. `decay180` significativement PIRE que la reference
  (observation descriptive, hors famille de tests formels -- la famille
  de tests etait unilaterale, orientee detection d'amelioration).

### Équipes promues 2026-27 et prior synthétique

Pour chaque championnat, une seule equipe promue etait reellement absente
de la fenetre d'historique (2016-2026) et a recu le traitement
`new_team_policy="promoted_prior"` (prior v0 empirique,
`promoted_priors_v0.json`, calibration provisoire -- Phase 2 de
calibration MLE complete a faire avant le 13/08). Les autres equipes
promues de chaque championnat avaient deja un historique reel dans la
fenetre et ont ete estimees normalement par la MLE, sans prior
synthetique.

| Championnat | Équipe avec prior | Statut du nom utilisé |
|---|---|---|
| Premier League | Coventry | Vérifié (grep direct dans l'historique confirme l'absence, alias déjà en place) |
| La Liga | Santander | Vérifié (grep SP2, 03/08/2026) |
| Ligue 1 | Le Mans | Vérifié (grep F2, 03/08/2026) |
| Bundesliga | Elversberg | Vérifié (grep D2, 03/08/2026) |

**Note de vérification** : les 3 équipes La Liga / Ligue 1 / Bundesliga
étant promues depuis la deuxième division de leur pays, leur nom a été
confirmé directement dans le fichier de deuxième division de la même
source (`football-data.co.uk` — fichiers SP2/F2/D2, même convention de
nommage que la première division), le 03/08/2026, avant publication —
méthode symétrique à la vérification déjà faite pour Coventry. Aucune
divergence : les 4 gels utilisent des noms d'équipes confirmés.

---

## Historique des révisions de ce document

| Date | Changement |
|---|---|
| 2026-07-06 | Création — désignations initiales, règle de promotion v1.0 |
| 2026-07-21 | Audit de cohérence du registre public : ajout de `elo-davidson-wc-v2` (omission depuis la création, corrigée), `elo-davidson-wc-poisson-mle`, `elo-davidson-wc-negbin-mle`, `elo-davidson-wc-ens-mle` (migration MLE du 19/07, enregistrés avec retard) comme challengers. Statut de `elo-davidson-wc-poisson-v2` actualisé (backfilling 104/104 matchs, branchement production) — limite du périmètre `world-cup` de `predictor_intl.py` notée explicitement. |
| 2026-07-22 | Première promotion du roster CdM (`elo-davidson-wc-ens-mle`, marché 1X2) à l'issue du protocole complet P0-P4 — remplace `elo-davidson-wc-v1`. Désignation officielle de `elo-davidson-wc-poisson` sur le marché "Distribution des buts" (jamais enregistré avant ce jour). Ajout de la règle de gouvernance P0 (pipeline de maintenance fonctionnel requis). `elo-davidson-wc-ens` (ensemble classique) et `elo-davidson-wc-poisson-v2` explicitement non promus malgré des statistiques favorables — voir section "Décision de promotion du 22 juillet 2026". |
| 2026-07-24 | Renommage complet du roster CdM vers "International" (`elo-davidson-wc-*` → `elo-davidson-intl-*`), 19 cerveaux, par filiation explicite (aucune donnée historique modifiée ni supprimée, voir section "Renommage CdM → International"). Correction d'un bug d'intégrité découvert au passage : les 3 cerveaux MLE (`poisson-mle`, `negbin-mle`, `ens-mle`) avaient un `model_key` interne erroné depuis leur création le 19/07, jamais détecté avant ce jour, corrigé avec republication de leurs 3 hashs. Le champion 1X2 (précédemment `elo-davidson-wc-ens-mle`) est renommé `elo-davidson-intl-ens-mle`, avec son nouveau hash corrigé. |
| 2026-08-03 | Première désignation du périmètre CLUBS (championnats classiques) : 4 model_keys `poisson-mle-club-{pl,la-liga,ligue-1,bundesliga}`, à l'issue de l'ablation {decay×ρ} du 02-03/08 et de son interprétation par consultation croisée (incluant un test statistique formel construit pour trancher la formulation Ligue 1). Convention `integrity_hash` retenue pour ce périmètre (pas `state_hash`, spécificité historique isolée du premier gel PL 1X2). Les noms des 4 équipes promues traitées par prior ont été vérifiés avant publication (Coventry par grep de l'historique élite ; Santander, Le Mans, Elversberg par grep des fichiers SP2/F2/D2 de la même source, même convention de nommage). Section « Périmètre PREMIER LEAGUE » soldée dans le même commit : `elo-davidson-v1` marqué remplacé par `poisson-mle-club-pl` (1X2), engagements Score exact / Over-Under du 14/08 tenus avec 11 jours d'avance. |
