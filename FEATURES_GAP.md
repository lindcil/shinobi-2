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

## Manquant → NON porté (pour l’instant)
| Système | Raison |
|---|---|
| Réactions doubles/triples/quadruples (ext31/43) | dépend du système d’éléments/modes d’Éternel ; la base a ses propres réactions — à fusionner dans une prochaine étape |
| Constellations uniques (ext41/45) | à régénérer pour les IDs TECH de la base ; prochaine étape |
| Monde ouvert, maîtres, événements, routes PNJ (ext35/38/40) | architecture de carte différente (histoire/raid/tour de la base) |
| 9 bijū canon (ext32), 50 techniques secrètes (ext33), Susanoo/duo (ext36) | doublonneraient les systèmes de la base, noms canon contraires à sa politique de noms originaux |
| Spéciaux Hiruzen/Asuma/Naruto/Sasuke (ext42) | noms canon + dépendance aux modes d’Éternel |
| QoL d’Éternel (ext39), modes Créatif d’Éternel (ext44) | la base a déjà son panneau Créatif ; QoL lié aux modes d’Éternel |
