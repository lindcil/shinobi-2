# Shinobi 2 : matrice des écarts (base : nouveau fichier, « Shinobi Éternel » GAME_VERSION 6)

## Déjà présent dans la base (on garde SA version, sans doublon)
Modes à stades (Bête + manteaux, pupilles solaire/lunaire/céleste/miroir/néant/anneaux, Ermite), roue de techniques, combos de chakra C (Ruée/Permutation/renforcée/Éveil), signes (SEAL_HANDS) + fusions (paires + 2 triples), clashs/ruées, esquive parfaite, rémanences, keyposes ZZZ amont (M1_KEYS, course ninja, lunge), voies/évolutions de techniques, rôles, sous-catégories (techSub), ultimes de build, histoire Acte I, raid/raid héroïque, saison de la tour, coop en ligne, équipement/uniques, clans, succès, musique, cinématiques, biomes village/désert de verre, panneau Créatif, notes de patch + roadmap en jeu, guide. Bijū : version de la base (noms originaux).

## Manquant → porté
| Système Éternel II v4.6.1 | État | Fichier |
|---|---|---|
| Rig v4.6 (squelette hiérarchique FK + IK 2 os, orientation unique, test 8 directions) | porté, adapté aux poses de la base (ninjaPose → cibles) | src/10_rig.js |
| Smears en croissant ZZZ (v4.6.1), ressort des cheveux | porté | src/10_rig.js |
| Poussée anti-chevauchement joueur/cible | porté (désactivé pendant les saisies) | src/10_rig.js |
| Réduction des flashs (option, activée par défaut) + impact frames réservées aux grands moments | porté, adapté à G.flashA | src/20_flash.js |

| Réactions triples/quadruples/quintuple + dōjutsu | porté v7.1, fusionné avec les doubles de la base | src/30_reactions.js |
| Constellations uniques (461) | porté v7.1 | src/40_const.js |

| 9 bijū canon (fusion avec BEASTS, kits canon, Bijūdama) | porté v8 | src/50_biju.js |
| 63 techniques secrètes canon (moteur ext33) | porté v8 (défis d’Arène remplacés par éliminations/réactions) | src/51_secrets.js |
| Susanoo 4 stades + noms canon des pupilles | porté v9 (fusionné avec l’armure spectrale des stades 5–8) | src/52_susanoo.js |
| Ultimes en duo | porté v9 (sans QTE : déclenchement automatique près d’un allié) | src/52_susanoo.js |
| Spéciales Hiruzen/Asuma/Naruto/Sasuke/Itachi/Madara/Kakashi (28) | porté v10 | src/53_specials.js |
| Monde ouvert, maîtres, 17 modes appris, 30 événements, PNJ/routes, apprivoisement | porté v11 (carte propre au mode « monde », modes convertis au format de stades de la base) | src/54_world.js |
| Modes Créatif d’Éternel (choc de Bijūdama, simulateur de boss, labos réactions/ultimes, créateur de moveset + simulation, maîtrise max) | porté v12 dans le panneau Créatif existant | src/55_crea_qol.js |
| QoL : C + E/F stade max, transitions à l’encre | porté v12 | src/55_crea_qol.js |

## Volontairement non repris (Shinobi 2 a déjà l’équivalent — pas de doublon)
| Système Éternel | Équivalent conservé dans Shinobi 2 |
|---|---|
| Système de modes ext3a–3d (u.md) | MODES à stades de la base (les modes d’Éternel sont convertis dedans) |
| Sceaux + fusions ext42, chocs QTE | SEAL_HANDS / FUSE_PAIR / FUSE_TRIPLE, clashs et ruées de la base |
| Katana dorsal ext42 | kenjutsu et lames de la base |
| Filtres par tags ext33b | sous-catégories techSub de la base |
| Arène de personnages ext33c (duels Naruto/Sasuke…) | défis convertis en éliminations/réactions ; PvP de la base |
| QTE de synchronisation des duos | duo déclenché automatiquement (pas de QTE) |
| Progression accélérée ext39 | équilibrage de la base conservé |
