# sie-registry

Depot public de transparence et d'antériorité du Sports Intelligence Engine (Calynt).

## Contenu
- `REGISTRY.md` / `registry.json` : miroir public de la table `model_registry` (modèles, compétition, statut, champion ou non, marché, date d'enregistrement, empreinte SHA-256 des gels quand elle existe, description générique).
- `anchors/cross-anchor-log.txt` : un SHA par jour du dépôt privé de prédictions, pour prouver l'antériorité sans rien révéler du contenu.

## Champs publiés (par modèle)
- `model_key`, `competition_key`, `status`, `is_champion`, `market`, `registered_at`, `key_role` (et la clé appariée `canonical_key` / `historical_key`), `hash` (empreinte SHA-256 du gel, quand elle existe).
- `famille` : famille du modèle, issue d'une table de correspondance explicite (jamais d'un texte libre). Familles actuelles :
  - Elo
  - Elo + Poisson sélections
  - Poisson coupes
  - Poisson-MLE club
  - Poisson-MLE générique
  - Projection de classement
- `type` : `champion` ou `challenger`.
- `date_gel` : date du gel (AAAA-MM-JJ), seulement quand elle est enregistrée ; sinon absente.
- `description` : gabarit fixe « <famille> — <compétition> (<champion|challenger>) », le nom de la compétition étant son nom officiel d'affichage.

## Alimentation (automatique, aucune édition manuelle)
- Ancrage : workflow `sie-cross-anchor` de sie-engine, chaque jour vers 19:37 UTC.
- Miroir du registre : workflow `sie-registry-miroir` de sie-engine, chaque jour à 21:17 UTC. Il ne pousse que si le contenu a changé (les différences d'horodatage `generated_at` sont ignorées). Commits du bot, sans réécriture d'historique. En cas d'échec, une Issue est ouverte côté sie-engine.
- Ce README est lui aussi généré par le script du miroir.
- La source de vérité reste la base ; la production ne lit jamais ces fichiers.

## Ce qui n'est jamais publié
Les champs `label`, `notes`, `retired_at`, `replaced_by`, tout paramètre de moteur, résultat d'ablation ou de test, toute donnée privée. Les lignes de test sont exclues. Le générateur applique une liste noire de motifs sur chaque champ descriptif et refuse de publier si l'un d'eux en contient un.
