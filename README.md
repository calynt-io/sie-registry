# sie-registry

Depot public de transparence et d'antériorité du Sports Intelligence Engine (Calynt).

## Contenu
- `REGISTRY.md` / `registry.json` : miroir public de la table `model_registry` (modèles, compétition, statut, champion ou non, marché, date d'enregistrement, empreinte SHA-256 des gels quand elle existe).
- `anchors/cross-anchor-log.txt` : un SHA par jour du dépôt privé de prédictions, pour prouver l'antériorité sans rien révéler du contenu.

## Alimentation (automatique, aucune édition manuelle)
- Ancrage : workflow `sie-cross-anchor` de sie-engine, chaque jour vers 19:37 UTC.
- Miroir du registre : workflow `sie-registry-miroir` de sie-engine, chaque jour à 21:17 UTC. Il ne pousse que si le contenu a changé (les différences d'horodatage `generated_at` sont ignorées). Commits du bot, sans réécriture d'historique. En cas d'échec, une Issue est ouverte côté sie-engine.
- La source de vérité reste la base ; la production ne lit jamais ces fichiers.

## Ce qui n'est jamais publié
Les champs `label`, `notes`, `retired_at`, `replaced_by`, tout paramètre de moteur ou d'ablation, toute donnée privée. Les lignes de test sont exclues. Le générateur refuse de publier si un de ces champs apparaît.
