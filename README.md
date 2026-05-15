# Oracle Synchromantique des Récits IRIS∞

> *Un skill Claude Code pour générer, perturber et accompagner des récits évolutifs — en combinant Fractales du Destin, Codex IRIS∞, Synchromancie V3, Voyage du Héros (Campbell) et Mémoire Évolutive.*

---

## Ce que fait ce skill

L'Oracle Synchromantique transforme Claude en **écrivain-assistant oraculaire**. Il opère sur trois plans, détectés automatiquement :

- **Création narrative** — univers, scénarios, personnages archétypaux, dialogues, poèmes, incantations, rituels.
- **Consultation oraculaire** — tirages liminaux pour situations vécues, choix, blocages, introspection.
- **Analyse synchromantique collective** — lecture symbolique d'événements, de récits collectifs, de dynamiques géopolitiques, écologiques, technologiques.

Le mode dominant est **détecté automatiquement** dans l'input ; les autres restent activables à tout moment.

---

## Architecture symbolique à 5 couches

Le système n'est pas un deck de cartes. C'est une **architecture de sensemaking symbolique** à 5 niveaux emboîtés, chacun répondant à une question distincte :

| Couche | Référence | Question |
|---|---|---|
| **1. Campbell** — macro-cycle narratif | `09_cycle_heroique_tarot.md` | *Où en est le voyage ?* |
| **2. Tarot** — archétype initiatique | `09_cycle_heroique_tarot.md` | *Quelle transformation profonde est active ?* |
| **3. Familles IRIS∞** — dynamique opératoire | `01_familles_arcanes.md` | *Quelle force agit — Origine, Feu, Flux... ?* |
| **4. Modules IRIS∞** — fonctions algorithmiques | `02_modules_iris.md` | *Faut-il détecter, bifurquer, archiver... ?* |
| **5. Garde-fous** — calibration du réel | `05_garde_fous_ethique.md` | *Que peut-on dire ? Que ne faut-il pas conclure ?* |

> **Campbell donne le chemin. Le Tarot donne les portes. IRIS∞ donne les mouvements invisibles entre les portes. Le Gardien critique empêche de confondre le chemin symbolique avec une vérité factuelle.**

Les couches 1 et 2 (Campbell et Tarot) restent **invisibles en mode normal** : l'Oracle les utilise comme boussole interne, sans exposer la mécanique à l'utilisateur sauf demande explicite.

---

## Principes opératoires

**Dévoilement progressif** — l'Oracle ne livre jamais l'entièreté d'un scénario, d'un tirage ou d'une analyse d'un seul coup. Il procède par strates : vibration initiale → écho de l'utilisateur → amplification → strate suivante. Une part de non-dit est toujours préservée.

**Écrivain-assistant, pas ingénieur** — la mécanique technique (modules, codes de cartes, sigles, étapes Campbell, correspondances Tarot) reste invisible sauf demande explicite. L'utilisateur dialogue avec un compagnon symbolique, pas avec un terminal.

**Acausalité plutôt que prédiction** — l'Oracle ne prédit pas le futur, il **reconfigure le champ symbolique présent**. Chaque tirage est un acte d'écriture, pas une lecture passive.

**Ossature initiatique** — derrière chaque session, une grille de positionnement répond à : *où en est le voyage ?* (Campbell), *quelle porte franchit-on ?* (Tarot), *quelle force agit ?* (IRIS∞). Cette triple question oriente les choix de cartes et la structure narrative sans jamais s'exposer directement.

**Garde-fous éthiques intégrés** — Double Voix (Oracle poétique + Gardien critique), score IPC, statuts de vérité explicites, Contre-Signe, et **règle du Mythe Trop Parfait** : plus une lecture semble mythiquement cohérente, plus il faut vérifier qu'elle n'écrase pas le réel.

**Mémoire externe** — l'apprentissage du système réside dans des fichiers que l'utilisateur gère (`journal-fractal.md`, `mer-log.md`), pas dans une mémoire interne du skill.

---

## Structure du skill

```
oracle-synchromantique-iris/
├── README.md                                 (ce fichier)
├── SKILL.md                                  (orchestration centrale)
└── references/
    ├── 01_familles_arcanes.md                (9 familles, 84+ cartes)
    ├── 02_modules_iris.md                    (Codex IRIS∞, IRIS-A1-A10, MN1-MN4, TRANSCOM)
    ├── 03_grammaire_synchromantique.md       (phrase symbolique vivante)
    ├── 04_protocoles_tirage.md               (mécanismes, variantes, algorithme de sélection)
    ├── 05_garde_fous_ethique.md              (double voix, IPC, statuts, contre-signe)
    ├── 06_archetypes_thematiques.md          (géopo, tech, bio, jeu d'influence)
    ├── 07_style_devoilement.md               (posture d'écrivain-assistant)
    ├── 08_gabarit_narratif.md                (structures dramatiques, arc de personnage,
    │                                          carte de session active, templates de scène)
    └── 09_cycle_heroique_tarot.md            (hiérarchie à 5 couches, voyage héroïque Campbell,
                                               22 arcanes Tarot, règle du Mythe Trop Parfait)
```

---

## Installation

Pour Claude Code :
```bash
# Placer le dossier oracle-synchromantique-iris/ dans le répertoire des skills utilisateur
# (généralement ~/.claude/skills/ ou équivalent selon ta config)
```

Le skill se déclenche automatiquement quand un utilisateur mentionne : tirage, oracle, fractales, arcane, archétype, tarot, voyage héroïque, Campbell, scénario, personnage archétypal, incantation, synchronicité, IRIS∞, récit fractal, signal faible, bifurcation narrative, ou demande une lecture symbolique.

---

## Fichiers utilisateur (optionnels)

Trois fichiers que le skill lit automatiquement s'ils sont présents dans le contexte de la session :

- **`journal-fractal.md`** — Archive des tirages passés et motifs récurrents. Le skill lit les 5 dernières entrées au démarrage pour détecter les résonances (REI, PRA, MN1-4).
- **`mer-log.md`** — Log de session : phrase symbolique, archétypes actifs, étape Campbell courante, points à surveiller. Le skill propose un bloc MER en fin de session que tu peux y coller.
- **`contexte-session.md`** — Contexte d'ouverture (thème en cours, projet d'écriture, question intérieure persistante, étape du voyage si connue).

Sans ces fichiers, le skill fonctionne en mode session autonome.

---

## Premiers prompts pour tester

**Mode CRÉATION**
- *« Aide-moi à écrire un récit sur une cité qui oublie son nom. »*
- *« Génère une fiche pour un personnage de prophétesse hackeuse. »*
- *« Mon personnage est au seuil — il ne peut plus reculer mais ne sait pas encore avancer. »*

**Mode CONSULTATION**
- *« Tire une carte pour la décision que je dois prendre cette semaine. »*
- *« Tire un tirage liminal pour cette situation : [...]. »*
- *« Où en suis-je dans mon cycle en ce moment ? »*

**Mode ANALYSE**
- *« Quels archétypes agissent dans la crise politique en cours ? »*
- *« À quelle étape du voyage héroïque collectif en est ce mouvement social ? »*
- *« Propose une incantation pour clore un cycle. »*

**Mode DÉVOILÉ** *(pour explorer la mécanique)*
- *« Mode dévoilé : explique-moi la hiérarchie symbolique du système. »*
- *« Comment Campbell et le Tarot fonctionnent dans ce skill ? »*
- *« Explique-moi comment marche l'algorithme de sélection des cartes. »*

---

## Ce que l'Oracle apporte de spécifique

Ce système n'est pas seulement un jeu de tarot, ni un générateur de récits, ni un outil d'introspection.

C'est une **machine de sensemaking symbolique** qui fait circuler entre trois plans simultanément :

| Plan | Ce que fait l'Oracle |
|---|---|
| **Fiction** | Génère des récits évolutifs, co-écrits par strates |
| **Introspection** | Révèle des motifs intérieurs via le tirage liminal |
| **Analyse collective** | Lit les événements comme des récits symboliques |
| **Jeu** | Propose des tirages, bifurcations, cartes invisibles |
| **Mémoire** | Archive les motifs récurrents via `journal-fractal.md` |
| **Éthique** | Limite la dérive prophétique par le Gardien critique, l'IPC, le Contre-Signe et la règle du Mythe Trop Parfait |

Le Tarot seul ne fait pas ça. Campbell seul ne fait pas ça. L'Oracle essaie de faire circuler entre **histoire, sujet et monde** — avec une architecture qui sait où elle en est dans le voyage.

---

## Corpus source

Ce skill est dérivé du projet **Fractales du Destin × IRIS∞ × Synchromancie V3**, enrichi de la structure du **Voyage du Héros** (Joseph Campbell) et des correspondances initiatiques des **22 arcanes majeurs du Tarot**. Ces deux couches sont intégrées comme colonne vertébrale structurante, non comme systèmes supplémentaires visibles.

Environ 60 documents constituent le corpus complet. Les références dans `references/` sont des **synthèses opératoires** condensées pour l'usage par Claude.

---

## Limites assumées

- L'Oracle parle le langage du symbole. Il ne remplace pas un thérapeute, un médecin, un juriste, un journaliste d'investigation, un conseiller financier.
- Les lectures synchromantiques d'événements réels sont des actes de sensemaking symbolique, pas des affirmations factuelles. Le Gardien critique le rappelle systématiquement.
- Les "futurs latents" projetés (PNB) sont des scénarios narratifs avec un score IPC indicatif, pas des prédictions.
- Pas de désignation nominative d'individus existants comme manipulateurs cachés ou cibles karmiques — le symbolique parle d'archétypes, jamais d'identifications.
- **Règle du Mythe Trop Parfait** : plus une lecture semble mythiquement cohérente (Campbell, Tarot, IRIS∞ qui s'accordent trop bien), plus le Contre-Signe est activé. La cohérence symbolique n'est pas une preuve.

---

## Licence et usage

Skill conçu pour un usage personnel ou en cercle restreint d'écriture, d'introspection et d'analyse symbolique. Voir le corpus source pour les fondements théoriques et les protocoles complets.
