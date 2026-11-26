# REGISTRY — Sports Intelligence Engine (miroir public)

> ⚠️ **Miroir généré automatiquement depuis Supabase `model_registry` le 2026-11-26T19:12:07.997881+00:00.**
> La production **ne lit jamais ce fichier** — `export_predictions_public.py`
> interroge la table Supabase **en direct** (`is_champion = true`). Ce document
> est publié pour la **transparence du lecteur**, régénéré par `generer_registry_public.py`.
>
> 🔒 **Version publique** : les champs `label`/`notes` (détail de paramétrage, ablations) sont volontairement retirés.

**Total : 367 modèles enregistrés** — 219 champion(s) désigné(s), 148 challenger(s).

> ℹ️ **Renommage CdM→International (24/07/2026).** 19 clés `historique` (préfixe `-wc-`, sous lesquelles vivent les prédictions en base) sont appariées 1-pour-1 à 19 clés `canonique` (préfixe `-intl-`, identité post-renommage) via la table `models`. **Les deux sont porteuses** — aucune n'est un doublon supprimable. `autonome` = hors renommage (clubs, PL).

## 1-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-1-liga` | autonome |  | champion | ✅ |  |  |

## 1-liga-classic-group-3 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-1-liga-classic-group-3` | autonome |  | champion | ✅ |  |  |

## 1-lyga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-1-lyga` | autonome |  | champion | ✅ |  |  |

## 1-snl (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-1-snl` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-1-snl` | autonome |  | champion | ✅ |  |  |

## 1a-divisio (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-1a-divisio` | autonome |  | champion | ✅ |  |  |

## 2-division-group-1 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-2-division-group-1` | autonome |  | champion | ✅ |  |  |

## 2-division-group-2 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-2-division-group-2` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-2-division-group-2` | autonome |  | champion | ✅ |  |  |

## 2-lig (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-2-lig` | autonome |  | champion | ✅ |  |  |

## 2-snl (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-2-snl` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-2-snl` | autonome |  | champion | ✅ |  |  |

## 3-lig-group-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-3-lig-group-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-3-lig-group-1` | autonome |  | champion | ✅ |  |  |

## 3-lig-group-2 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-3-lig-group-2` | autonome |  | champion | ✅ |  |  |

## 3-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-3-liga` | autonome |  | champion | ✅ |  |  |

## 3-liga-msfl (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-3-liga-msfl` | autonome |  | champion | ✅ |  |  |

## 4-liga-divizie-b (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-4-liga-divizie-b` | autonome |  | champion | ✅ |  |  |

## 4-liga-divizie-e (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-4-liga-divizie-e` | autonome |  | champion | ✅ |  |  |

## a-league-women (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-a-league-women` | autonome |  | champion | ✅ |  |  |

## a-lyga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-a-lyga` | autonome |  | champion | ✅ |  |  |

## afc-champions-league-elite (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-afc-champions-league-elite` | autonome |  | champion | ✅ |  |  |

## africa-cup-of-nations-qualification (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `selections-elo-poisson-v1-africa-cup-of-nations-qualification` | autonome |  | champion | ✅ |  |  |

## afrique-du-sud-1st-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-afrique-du-sud-1st-division` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-afrique-du-sud-1st-division` | autonome |  | challenger |  |  |  |

## albanie-1st-division (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-albanie-1st-division` | autonome |  | champion | ✅ |  |  |

## albanie-superliga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-albanie-superliga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-albanie-superliga` | autonome |  | champion | ✅ |  |  |

## algerie-ligue-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-algerie-ligue-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-algerie-ligue-1` | autonome |  | champion | ✅ |  |  |

## algerie-ligue-2 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-algerie-ligue-2` | autonome |  | champion | ✅ |  |  |

## allemagne-regionalliga-west (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-allemagne-regionalliga-west` | autonome |  | champion | ✅ |  |  |

## allsvenskan (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-allsvenskan` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-allsvenskan` | autonome |  | champion | ✅ |  |  |

## angleterre-fa-cup (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-angleterre-fa-cup` | autonome |  | champion | ✅ |  |  |

## angleterre-league-cup (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-angleterre-league-cup` | autonome |  | champion | ✅ |  |  |

## angleterre-national-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-angleterre-national-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-angleterre-national-league` | autonome |  | champion | ✅ |  |  |

## arabie-saoudite-division-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-arabie-saoudite-division-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-arabie-saoudite-division-1` | autonome |  | champion | ✅ |  |  |

## arabie-saoudite-pro-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-arabie-saoudite-pro-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-arabie-saoudite-pro-league` | autonome |  | champion | ✅ |  |  |

## armenie-first-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-armenie-first-league` | autonome |  | champion | ✅ |  |  |

## autriche-2-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-autriche-2-liga` | autonome |  | champion | ✅ |  |  |

## autriche-bundesliga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-autriche-bundesliga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-autriche-bundesliga` | autonome |  | champion | ✅ |  |  |

## autriche-regionalliga-west (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-autriche-regionalliga-west` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-autriche-regionalliga-west` | autonome |  | champion | ✅ |  |  |

## bielorussie-1-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-bielorussie-1-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-bielorussie-1-division` | autonome |  | champion | ✅ |  |  |

## bielorussie-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-bielorussie-premier-league` | autonome |  | champion | ✅ |  |  |

## botola-pro (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-botola-pro` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-botola-pro` | autonome |  | champion | ✅ |  |  |

## brasileirao (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-brasileirao` | autonome |  | champion | ✅ |  | `d4a6afe9f153…` |
| `projection-classement-forme-v1-brasileirao` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-brasileirao` | autonome |  | challenger |  |  |  |

## brasileiro-women (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-brasileiro-women` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-brasileiro-women` | autonome |  | champion | ✅ |  |  |

## bulgarie-first-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-bulgarie-first-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-bulgarie-first-league` | autonome |  | champion | ✅ |  |  |

## bulgarie-second-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-bulgarie-second-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-bulgarie-second-league` | autonome |  | champion | ✅ |  |  |

## bundesliga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-bundesliga` | autonome |  | champion | ✅ |  | `7e0a68f22f58…` |
| `projection-classement-forme-v1-bundesliga` | autonome |  | challenger |  |  |  |

## bundesliga-2 (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-bundesliga-2` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-bundesliga-2` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-bundesliga-2` | autonome |  | champion | ✅ |  |  |

## campionato (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-campionato` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-campionato` | autonome |  | champion | ✅ |  |  |

## challenger-pro-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-challenger-pro-league` | autonome |  | champion | ✅ |  |  |

## champions-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-champions-league` | autonome |  | champion | ✅ |  |  |

## championship (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-championship` | autonome |  | champion | ✅ |  | `d9eb1658a922…` |
| `projection-classement-forme-v1-championship` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-championship` | autonome |  | challenger |  |  |  |

## chili-primera-b (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-chili-primera-b` | autonome |  | champion | ✅ |  |  |

## chili-primera-division (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-chili-primera-division` | autonome |  | champion | ✅ |  |  |

## chine-league-one (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-chine-league-one` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-chine-league-one` | autonome |  | champion | ✅ |  |  |

## chine-super-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-chine-super-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-chine-super-league` | autonome |  | champion | ✅ |  |  |

## chypre-1-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-chypre-1-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-chypre-1-division` | autonome |  | champion | ✅ |  |  |

## chypre-2-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-chypre-2-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-chypre-2-division` | autonome |  | champion | ✅ |  |  |

## colombie-primera-a (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-colombie-primera-a` | autonome |  | champion | ✅ |  |  |

## colombie-primera-b (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-colombie-primera-b` | autonome |  | champion | ✅ |  |  |

## concacaf-nations-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `selections-elo-poisson-v1-concacaf-nations-league` | autonome |  | champion | ✅ |  |  |

## conference-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-conference-league` | autonome |  | champion | ✅ |  |  |

## copa-do-brasil (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-copa-do-brasil` | autonome |  | champion | ✅ |  |  |

## coppa-italia (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-coppa-italia` | autonome |  | champion | ✅ |  |  |

## costa-rica-primera-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-costa-rica-primera-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-costa-rica-primera-division` | autonome |  | champion | ✅ |  |  |

## croatie-hnl (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-croatie-hnl` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-croatie-hnl` | autonome |  | champion | ✅ |  |  |

## czech-liga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-czech-liga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-czech-liga` | autonome |  | champion | ✅ |  |  |

## danemark-1-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-danemark-1-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-danemark-1-division` | autonome |  | champion | ✅ |  |  |

## danemark-superliga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-danemark-superliga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-danemark-superliga` | autonome |  | champion | ✅ |  |  |

## division-intermedia (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-division-intermedia` | autonome |  | champion | ✅ |  |  |

## division-profesional-apertura (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-division-profesional-apertura` | autonome |  | champion | ✅ |  |  |

## division-profesional-clausura (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-division-profesional-clausura` | autonome |  | champion | ✅ |  |  |

## ecosse-championship (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-ecosse-championship` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-ecosse-championship` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ecosse-championship` | autonome |  | champion | ✅ |  |  |

## ecosse-league-one (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-ecosse-league-one` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-ecosse-league-one` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ecosse-league-one` | autonome |  | champion | ✅ |  |  |

## ecosse-league-two (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-ecosse-league-two` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-ecosse-league-two` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ecosse-league-two` | autonome |  | champion | ✅ |  |  |

## ecosse-premiership (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ecosse-premiership` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ecosse-premiership` | autonome |  | champion | ✅ |  |  |

## eerste-divisie (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-eerste-divisie` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-eerste-divisie` | autonome |  | champion | ✅ |  |  |

## ekstraklasa (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ekstraklasa` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ekstraklasa` | autonome |  | champion | ✅ |  |  |

## elite-one (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-elite-one` | autonome |  | champion | ✅ |  |  |

## eliteserien (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-eliteserien` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-eliteserien` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-eliteserien` | autonome |  | champion | ✅ |  |  |

## eredivisie (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-eredivisie` | autonome |  | champion | ✅ |  | `a935d6be8f95…` |
| `projection-classement-forme-v1-eredivisie` | autonome |  | challenger |  |  |  |

## eredivisie-women (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-eredivisie-women` | autonome |  | champion | ✅ |  |  |

## erovnuli-liga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-erovnuli-liga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-erovnuli-liga` | autonome |  | champion | ✅ |  |  |

## erovnuli-liga-2 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-erovnuli-liga-2` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-erovnuli-liga-2` | autonome |  | champion | ✅ |  |  |

## ettan-norra (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ettan-norra` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ettan-norra` | autonome |  | champion | ✅ |  |  |

## ettan-sodra (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ettan-sodra` | autonome |  | champion | ✅ |  |  |

## europa-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-coupes-v1-europa-league` | autonome |  | champion | ✅ |  |  |

## fa-wsl (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-fa-wsl` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-fa-wsl` | autonome |  | champion | ✅ |  |  |

## feminine-division-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-feminine-division-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-feminine-division-1` | autonome |  | champion | ✅ |  |  |

## first-nl (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-first-nl` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-first-nl` | autonome |  | challenger |  |  |  |

## fnl (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-fnl` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-fnl` | autonome |  | challenger |  |  |  |

## frauen-bundesliga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-frauen-bundesliga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-frauen-bundesliga` | autonome |  | champion | ✅ |  |  |

## ghana-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ghana-premier-league` | autonome |  | champion | ✅ |  |  |

## girabola (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-girabola` | autonome |  | champion | ✅ |  |  |

## grece-super-league-1 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-grece-super-league-1` | autonome |  | champion | ✅ |  |  |

## guatemala-liga-nacional (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-guatemala-liga-nacional` | autonome |  | champion | ✅ |  |  |

## i-liga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-i-liga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-i-liga` | autonome |  | champion | ✅ |  |  |

## ii-liga-east (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ii-liga-east` | autonome |  | champion | ✅ |  |  |

## indonesie-liga-1 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-indonesie-liga-1` | autonome |  | champion | ✅ |  |  |

## irlande-du-nord-championship (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-irlande-du-nord-championship` | autonome |  | champion | ✅ |  |  |

## irlande-du-nord-premiership (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-irlande-du-nord-premiership` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-irlande-du-nord-premiership` | autonome |  | champion | ✅ |  |  |

## irlande-premier-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-irlande-premier-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-irlande-premier-division` | autonome |  | champion | ✅ |  |  |

## j1-league (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-j1-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-j1-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-j1-league` | autonome |  | champion | ✅ |  |  |

## j2-league (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-j2-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-j2-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-j2-league` | autonome |  | champion | ✅ |  |  |

## j3-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-j3-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-j3-league` | autonome |  | champion | ✅ |  |  |

## jamaique-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-jamaique-premier-league` | autonome |  | champion | ✅ |  |  |

## jupiler-pro-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-jupiler-pro-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-jupiler-pro-league` | autonome |  | champion | ✅ |  |  |

## k-league-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-k-league-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-k-league-1` | autonome |  | champion | ✅ |  |  |

## k-league-2 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-k-league-2` | autonome |  | champion | ✅ |  |  |

## k3-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-k3-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-k3-league` | autonome |  | champion | ✅ |  |  |

## kakkonen-lohko-a (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-kakkonen-lohko-a` | autonome |  | champion | ✅ |  |  |

## kakkonen-lohko-b (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-kakkonen-lohko-b` | autonome |  | champion | ✅ |  |  |

## kakkonen-lohko-c (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-kakkonen-lohko-c` | autonome |  | champion | ✅ |  |  |

## kazakhstan-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-kazakhstan-premier-league` | autonome |  | champion | ✅ |  |  |

## koweit-premier-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-koweit-premier-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-koweit-premier-league` | autonome |  | champion | ✅ |  |  |

## la-liga (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-la-liga` | autonome |  | champion | ✅ |  | `430ed6efb722…` |
| `projection-classement-forme-v1-la-liga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-la-liga` | autonome |  | challenger |  |  |  |

## league-one (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-league-one` | autonome |  | champion | ✅ |  |  |

## league-two (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-league-two` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-league-two` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-league-two` | autonome |  | champion | ✅ |  |  |

## liga-de-expansion-mx (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-de-expansion-mx` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-liga-de-expansion-mx` | autonome |  | champion | ✅ |  |  |

## liga-ii (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-ii` | autonome |  | champion | ✅ |  |  |

## liga-leumit (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-leumit` | autonome |  | champion | ✅ |  |  |

## liga-mx (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-mx` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-liga-mx` | autonome |  | champion | ✅ |  |  |

## liga-panamena-de-futbol (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-panamena-de-futbol` | autonome |  | champion | ✅ |  |  |

## liga-portugal-2 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-portugal-2` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-liga-portugal-2` | autonome |  | champion | ✅ |  |  |

## liga-pro (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-pro` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-liga-pro` | autonome |  | champion | ✅ |  |  |

## liga-profesional-argentina (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-liga-profesional-argentina` | autonome |  | champion | ✅ |  |  |

## ligat-haal (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ligat-haal` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ligat-haal` | autonome |  | champion | ✅ |  |  |

## ligi-kuu-bara (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ligi-kuu-bara` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ligi-kuu-bara` | autonome |  | champion | ✅ |  |  |

## ligue-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-ligue-1` | autonome |  | champion | ✅ |  | `621ae1b8e5f9…` |
| `projection-classement-forme-v1-ligue-1` | autonome |  | challenger |  |  |  |

## ligue-2 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ligue-2` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ligue-2` | autonome |  | champion | ✅ |  |  |

## macedoine-du-nord-first-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-macedoine-du-nord-first-league` | autonome |  | champion | ✅ |  |  |

## macedoine-du-nord-second-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-macedoine-du-nord-second-league` | autonome |  | champion | ✅ |  |  |

## major-league-soccer (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-major-league-soccer` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-major-league-soccer` | autonome |  | champion | ✅ |  |  |

## malaisie-super-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-malaisie-super-league` | autonome |  | champion | ✅ |  |  |

## malte-challenge-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-malte-challenge-league` | autonome |  | champion | ✅ |  |  |

## malte-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-malte-premier-league` | autonome |  | champion | ✅ |  |  |

## meistaradeildin (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-meistaradeildin` | autonome |  | champion | ✅ |  |  |

## meistriliiga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-meistriliiga` | autonome |  | champion | ✅ |  |  |

## montenegro-first-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-montenegro-first-league` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-montenegro-first-league` | autonome |  | challenger |  |  |  |

## montenegro-second-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-montenegro-second-league` | autonome |  | champion | ✅ |  |  |

## national-2-group-a (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-national-2-group-a` | autonome |  | champion | ✅ |  |  |

## national-2-group-b (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-national-2-group-b` | autonome |  | champion | ✅ |  |  |

## national-2-group-c (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-national-2-group-c` | autonome |  | champion | ✅ |  |  |

## national-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-national-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-national-division` | autonome |  | champion | ✅ |  |  |

## national-league-north (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-national-league-north` | autonome |  | champion | ✅ |  |  |

## national-league-south (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-national-league-south` | autonome |  | champion | ✅ |  |  |

## nb-i (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-nb-i` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-nb-i` | autonome |  | champion | ✅ |  |  |

## nb-ii (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-nb-ii` | autonome |  | champion | ✅ |  |  |

## nb-iii-northeast (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-nb-iii-northeast` | autonome |  | champion | ✅ |  |  |

## nb-iii-southwest (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-nb-iii-southwest` | autonome |  | champion | ✅ |  |  |

## non-league-premier-isthmian (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-non-league-premier-isthmian` | autonome |  | champion | ✅ |  |  |

## non-league-premier-northern (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-non-league-premier-northern` | autonome |  | champion | ✅ |  |  |

## norvege-1-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-norvege-1-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-norvege-1-division` | autonome |  | champion | ✅ |  |  |

## npfl (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-npfl` | autonome |  | champion | ✅ |  |  |

## nwsl-women (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-nwsl-women` | autonome |  | champion | ✅ |  |  |

## oberliga-hamburg (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-oberliga-hamburg` | autonome |  | champion | ✅ |  |  |

## ouganda-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ouganda-premier-league` | autonome |  | champion | ✅ |  |  |

## ouzbekistan-super-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ouzbekistan-super-league` | autonome |  | champion | ✅ |  |  |

## pays-de-galles-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-pays-de-galles-premier-league` | autonome |  | champion | ✅ |  |  |

## perou-segunda-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-perou-segunda-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-perou-segunda-division` | autonome |  | champion | ✅ |  |  |

## persian-gulf-pro-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-persian-gulf-pro-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-persian-gulf-pro-league` | autonome |  | champion | ✅ |  |  |

## premier-league (4)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `elo-davidson-v1` | autonome |  | retired |  | 1X2 |  |
| `poisson-mle-club-pl` | autonome |  | champion | ✅ |  | `c2b71a4012c6…` |
| `projection-classement-forme-v1-premier-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-premier-league` | autonome |  | challenger |  |  |  |

## premier-soccer-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-premier-soccer-league` | autonome |  | champion | ✅ |  |  |

## premijer-liga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-premijer-liga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-premijer-liga` | autonome |  | champion | ✅ |  |  |

## premyer-liqa (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-premyer-liqa` | autonome |  | champion | ✅ |  |  |

## primeira-liga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-primeira-liga` | autonome |  | champion | ✅ |  | `93a2eb1014cf…` |
| `projection-classement-forme-v1-primeira-liga` | autonome |  | challenger |  |  |  |

## primera-b-metropolitana (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-b-metropolitana` | autonome |  | champion | ✅ |  |  |

## primera-c (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-c` | autonome |  | champion | ✅ |  |  |

## primera-division-clausura (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-division-clausura` | autonome |  | champion | ✅ |  |  |

## primera-division-femenina (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-division-femenina` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-primera-division-femenina` | autonome |  | champion | ✅ |  |  |

## primera-division-rfef-group-1 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-division-rfef-group-1` | autonome |  | champion | ✅ |  |  |

## primera-division-rfef-group-2 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-division-rfef-group-2` | autonome |  | champion | ✅ |  |  |

## primera-nacional (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-primera-nacional` | autonome |  | champion | ✅ |  |  |

## prva-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-prva-liga` | autonome |  | champion | ✅ |  |  |

## regionalliga-nordost (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-regionalliga-nordost` | autonome |  | champion | ✅ |  |  |

## regionalliga-ost (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-regionalliga-ost` | autonome |  | champion | ✅ |  |  |

## regionalliga-sudwest (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-regionalliga-sudwest` | autonome |  | champion | ✅ |  |  |

## roumanie-liga-i (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-roumanie-liga-i` | autonome |  | champion | ✅ |  |  |

## russie-first-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-russie-first-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-russie-first-league` | autonome |  | champion | ✅ |  |  |

## russie-premier-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-russie-premier-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-russie-premier-league` | autonome |  | champion | ✅ |  |  |

## segunda-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-segunda-division` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-segunda-division` | autonome |  | champion | ✅ |  |  |

## segunda-division-rfef-group-5 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-segunda-division-rfef-group-5` | autonome |  | champion | ✅ |  |  |

## serbie-super-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serbie-super-liga` | autonome |  | champion | ✅ |  |  |

## serie-a (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-serie-a` | autonome |  | champion | ✅ |  | `94d8ed795e93…` |
| `projection-classement-forme-v1-serie-a` | autonome |  | challenger |  |  |  |

## serie-a-women (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serie-a-women` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-serie-a-women` | autonome |  | champion | ✅ |  |  |

## serie-b (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serie-b` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-serie-b` | autonome |  | champion | ✅ |  |  |

## serie-c (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serie-c` | autonome |  | champion | ✅ |  |  |

## serie-c-girone-a (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serie-c-girone-a` | autonome |  | champion | ✅ |  |  |

## serie-c-girone-b (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serie-c-girone-b` | autonome |  | champion | ✅ |  |  |

## serie-c-girone-c (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-serie-c-girone-c` | autonome |  | champion | ✅ |  |  |

## singapour-premier-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-singapour-premier-league` | autonome |  | champion | ✅ |  |  |

## slovaquie-2-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-slovaquie-2-liga` | autonome |  | champion | ✅ |  |  |

## slovaquie-super-liga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-slovaquie-super-liga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-slovaquie-super-liga` | autonome |  | champion | ✅ |  |  |

## stars-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-stars-league` | autonome |  | champion | ✅ |  |  |

## suisse-challenge-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-suisse-challenge-league` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-suisse-challenge-league` | autonome |  | challenger |  |  |  |

## suisse-super-league (3)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `projection-classement-recette-v1-suisse-super-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v1-suisse-super-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-suisse-super-league` | autonome |  | champion | ✅ |  |  |

## super-lig (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-super-lig` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-super-lig` | autonome |  | champion | ✅ |  |  |

## superettan (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-superettan` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-superettan` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-14 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-14` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-15 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-15` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-16 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-16` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-18 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-18` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-2 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-2` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-3 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-3` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-5 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-5` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-6 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-6` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-7 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-7` | autonome |  | champion | ✅ |  |  |

## tercera-division-rfef-group-8 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tercera-division-rfef-group-8` | autonome |  | champion | ✅ |  |  |

## thai-league-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-thai-league-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-thai-league-1` | autonome |  | champion | ✅ |  |  |

## thai-league-2 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-thai-league-2` | autonome |  | champion | ✅ |  |  |

## tunisie-ligue-1 (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tunisie-ligue-1` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-tunisie-ligue-1` | autonome |  | champion | ✅ |  |  |

## turquie-1-lig (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-turquie-1-lig` | autonome |  | champion | ✅ |  |  |

## tweede-divisie (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-tweede-divisie` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-tweede-divisie` | autonome |  | challenger |  |  |  |

## uefa-nations-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `selections-elo-poisson-v1-uefa-nations-league` | autonome |  | champion | ✅ |  |  |

## ukraine-premier-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-ukraine-premier-league` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-ukraine-premier-league` | autonome |  | champion | ✅ |  |  |

## uruguay-segunda-division (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-uruguay-segunda-division` | autonome |  | champion | ✅ |  |  |
| `recette-generique-v2-c1-uruguay-segunda-division` | autonome |  | challenger |  |  |  |

## urvalsdeild (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-urvalsdeild` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-urvalsdeild` | autonome |  | champion | ✅ |  |  |

## usl-league-one (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-usl-league-one` | autonome |  | champion | ✅ |  |  |

## veikkausliiga (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-veikkausliiga` | autonome |  | challenger |  |  |  |
| `recette-generique-v2-c1-veikkausliiga` | autonome |  | champion | ✅ |  |  |

## venezuela-primera-division (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-venezuela-primera-division` | autonome |  | champion | ✅ |  |  |

## virsliga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-virsliga` | autonome |  | champion | ✅ |  |  |

## world-cup (38)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `elo-davidson-intl-ens` | canonique | `elo-davidson-wc-ens` | challenger |  |  |  |
| `elo-davidson-intl-ens-mle` | canonique | `elo-davidson-wc-ens-mle` | champion | ✅ |  |  |
| `elo-davidson-intl-gd` | canonique | `elo-davidson-wc-gd` | challenger |  |  |  |
| `elo-davidson-intl-hfa` | canonique | `elo-davidson-wc-hfa` | challenger |  |  |  |
| `elo-davidson-intl-hfat` | canonique | `elo-davidson-wc-hfat` | challenger |  |  |  |
| `elo-davidson-intl-l10` | canonique | `elo-davidson-wc-l10` | challenger |  |  |  |
| `elo-davidson-intl-l11` | canonique | `elo-davidson-wc-l11` | challenger |  |  |  |
| `elo-davidson-intl-l12` | canonique | `elo-davidson-wc-l12` | challenger |  |  |  |
| `elo-davidson-intl-l13` | canonique | `elo-davidson-wc-l13` | challenger |  |  |  |
| `elo-davidson-intl-l14` | canonique | `elo-davidson-wc-l14` | challenger |  |  |  |
| `elo-davidson-intl-negbin` | canonique | `elo-davidson-wc-negbin` | challenger |  |  |  |
| `elo-davidson-intl-negbin-mle` | canonique | `elo-davidson-wc-negbin-mle` | challenger |  |  |  |
| `elo-davidson-intl-poisson` | canonique | `elo-davidson-wc-poisson` | challenger |  |  |  |
| `elo-davidson-intl-poisson-mle` | canonique | `elo-davidson-wc-poisson-mle` | challenger |  |  |  |
| `elo-davidson-intl-poisson-v2` | canonique | `elo-davidson-wc-poisson-v2` | challenger |  |  |  |
| `elo-davidson-intl-v1` | canonique | `elo-davidson-wc-v1` | challenger |  |  |  |
| `elo-davidson-intl-v2` | canonique | `elo-davidson-wc-v2` | challenger |  |  |  |
| `elo-davidson-intl-w24` | canonique | `elo-davidson-wc-w24` | challenger |  |  |  |
| `elo-davidson-intl-w24t` | canonique | `elo-davidson-wc-w24t` | challenger |  |  |  |
| `elo-davidson-wc-ens` | historique | `elo-davidson-intl-ens` | challenger |  |  |  |
| `elo-davidson-wc-ens-mle` | historique | `elo-davidson-intl-ens-mle` | challenger |  | 1X2 |  |
| `elo-davidson-wc-gd` | historique | `elo-davidson-intl-gd` | challenger |  |  |  |
| `elo-davidson-wc-hfa` | historique | `elo-davidson-intl-hfa` | challenger |  |  |  |
| `elo-davidson-wc-hfat` | historique | `elo-davidson-intl-hfat` | challenger |  |  |  |
| `elo-davidson-wc-l10` | historique | `elo-davidson-intl-l10` | challenger |  |  |  |
| `elo-davidson-wc-l11` | historique | `elo-davidson-intl-l11` | challenger |  |  |  |
| `elo-davidson-wc-l12` | historique | `elo-davidson-intl-l12` | challenger |  |  |  |
| `elo-davidson-wc-l13` | historique | `elo-davidson-intl-l13` | challenger |  |  |  |
| `elo-davidson-wc-l14` | historique | `elo-davidson-intl-l14` | challenger |  |  |  |
| `elo-davidson-wc-negbin` | historique | `elo-davidson-intl-negbin` | challenger |  |  |  |
| `elo-davidson-wc-negbin-mle` | historique | `elo-davidson-intl-negbin-mle` | challenger |  |  |  |
| `elo-davidson-wc-poisson` | historique | `elo-davidson-intl-poisson` | challenger |  |  |  |
| `elo-davidson-wc-poisson-mle` | historique | `elo-davidson-intl-poisson-mle` | challenger |  |  |  |
| `elo-davidson-wc-poisson-v2` | historique | `elo-davidson-intl-poisson-v2` | challenger |  |  |  |
| `elo-davidson-wc-v1` | historique | `elo-davidson-intl-v1` | challenger |  |  |  |
| `elo-davidson-wc-v2` | historique | `elo-davidson-intl-v2` | challenger |  |  |  |
| `elo-davidson-wc-w24` | historique | `elo-davidson-intl-w24` | challenger |  |  |  |
| `elo-davidson-wc-w24t` | historique | `elo-davidson-intl-w24t` | challenger |  |  |  |

## zambie-super-league (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `recette-generique-v1-zambie-super-league` | autonome |  | champion | ✅ |  |  |
