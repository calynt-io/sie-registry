# REGISTRY — Sports Intelligence Engine (miroir public)

> ⚠️ **Miroir généré automatiquement depuis Supabase `model_registry` le 2026-08-10T16:44:27.968858+00:00.**
> La production **ne lit jamais ce fichier** — `export_predictions_public.py`
> interroge la table Supabase **en direct** (`is_champion = true`). Ce document
> est publié pour la **transparence du lecteur**, régénéré par `generer_registry_public.py`.
>
> 🔒 **Version publique** : les champs `label`/`notes` (détail de paramétrage, ablations) sont volontairement retirés.

**Total : 43 modèles enregistrés** — 5 champion(s) désigné(s), 38 challenger(s).

> ℹ️ **Renommage CdM→International (24/07/2026).** 19 clés `historique` (préfixe `-wc-`, sous lesquelles vivent les prédictions en base) sont appariées 1-pour-1 à 19 clés `canonique` (préfixe `-intl-`, identité post-renommage) via la table `models`. **Les deux sont porteuses** — aucune n'est un doublon supprimable. `autonome` = hors renommage (clubs, PL).

## bundesliga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-bundesliga` | autonome |  | champion | ✅ |  | `7e0a68f22f58…` |

## la-liga (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-la-liga` | autonome |  | champion | ✅ |  | `20bb2beec4a0…` |

## ligue-1 (1)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `poisson-mle-club-ligue-1` | autonome |  | champion | ✅ |  | `b65bb11644f1…` |

## premier-league (2)

| model_key | rôle clé | paire | statut | champion | marché | hash |
|---|---|---|---|---|---|---|
| `elo-davidson-v1` | autonome |  | challenger |  | 1X2 |  |
| `poisson-mle-club-pl` | autonome |  | champion | ✅ |  | `e1b165ad5b56…` |

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
