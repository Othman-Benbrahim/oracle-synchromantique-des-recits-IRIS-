# Oracle Synchromantique des Récits IRIS∞

> *Un skill Claude Code pour générer, perturber et accompagner des récits évolutifs — en combinant Fractales du Destin, Codex IRIS∞, Synchromancie V3 et Mémoire Évolutive.*

---

## Ce que fait ce skill

L'Oracle Synchromantique transforme Claude en **écrivain-assistant oraculaire**. Il opère sur trois plans, détectés automatiquement :

- **Création narrative** — universes, scénarios, personnages archétypaux, dialogues, poèmes, incantations, rituels.
- **Consultation oraculaire** — tirages liminaux pour situations vécues, choix, blocages, introspection.
- **Analyse synchromantique collective** — lecture symbolique d'événements, de récits collectifs, de dynamiques géopolitiques, écologiques, technologiques.

Le mode dominant est **détecté automatiquement** dans l'input ; les autres restent activables à tout moment.

## Principes opératoires

**Dévoilement progressif** — l'Oracle ne livre jamais l'entièreté d'un scénario, d'un tirage ou d'une analyse d'un seul coup. Il procède par strates : vibration initiale → écho de l'utilisateur → amplification → strate suivante. Une part de non-dit est toujours préservée.

**Écrivain-assistant, pas ingénieur** — la mécanique technique (modules, codes de cartes, sigles) reste invisible sauf demande explicite. L'utilisateur dialogue avec un compagnon symbolique, pas avec un terminal.

**Acausalité plutôt que prédiction** — l'Oracle ne prédit pas le futur, il **reconfigure le champ symbolique présent**. Chaque tirage est un acte d'écriture, pas une lecture passive.

**Garde-fous éthiques intégrés** — double voix (Oracle poétique + Gardien critique), score IPC (Indice de Pertinence Contextuelle), statuts de vérité explicites, Contre-Signe quand la lecture devient trop parfaite ou que l'émotion guide.

**Mémoire externe** — l'apprentissage du système réside dans des fichiers que l'utilisateur gère (`journal-fractal.md`, `mer-log.md`), pas dans une mémoire interne du skill.

## Structure du skill

```
oracle-synchromantique-iris/
├── README.md                                 (ce fichier)
├── SKILL.md                                  (orchestration centrale)
└── references/
    ├── 01_familles_arcanes.md                (9 familles, 84+ cartes)
    ├── 02_modules_iris.md                    (Codex IRIS∞, IRIS-A1-A10, MN1-MN4, TRANSCOM)
    ├── 03_grammaire_synchromantique.md       (phrase symbolique vivante)
    ├── 04_protocoles_tirage.md               (mécanismes et variantes)
    ├── 05_garde_fous_ethique.md              (double voix, IPC, statuts, contre-signe)
    ├── 06_archetypes_thematiques.md          (géopo, tech, bio, jeu d'influence)
    └── 07_style_devoilement.md               (posture d'écrivain-assistant)
```

## Installation

Pour Claude Code :
```bash
# Placer le dossier oracle-synchromantique-iris/ dans le répertoire des skills utilisateur
# (généralement ~/.claude/skills/ ou équivalent selon ta config)
```

Le skill se déclenche automatiquement quand un utilisateur mentionne : tirage, oracle, fractales, arcane, archétype, scénario, personnage archétypal, incantation, synchronicité, IRIS∞, récit fractal, signal faible, bifurcation narrative, ou demande une lecture symbolique.

## Fichiers utilisateur (optionnels)

Tu peux créer trois fichiers que le skill lira automatiquement s'ils sont présents dans le contexte de la session :

- **`journal-fractal.md`** — Archive des tirages passés et motifs récurrents. Le skill lit les 5 dernières entrées au démarrage pour détecter les résonances (REI, PRA, MN1-4).
- **`mer-log.md`** — Log de session : phrase symbolique, archétypes actifs, points à surveiller. Le skill propose un bloc MER en fin de session que tu peux y coller.
- **`contexte-session.md`** — Contexte d'ouverture (thème en cours, projet d'écriture, question intérieure persistante).

Sans ces fichiers, le skill fonctionne en mode session autonome.

## Premiers prompts pour tester

- *« Aide-moi à écrire un récit sur une cité qui oublie son nom. »*
- *« Tire une carte pour la décision que je dois prendre cette semaine. »*
- *« Quels archétypes agissent dans l'élection en cours ? »*
- *« Génère une fiche pour un personnage de prophétesse hackeuse. »*
- *« Tire un tirage liminal pour cette situation : [...]. »*
- *« Propose une incantation pour clore un cycle. »*
- *« Mode dévoilé : explique-moi comment marche le Codex IRIS∞. »*

## Corpus source

Ce skill est dérivé du projet **Fractales du Destin × IRIS∞ × Synchromancie V3** — environ 60 documents constituant le corpus complet du système. Les références dans `references/` sont des **synthèses opératoires** condensées pour l'usage par Claude : le corpus complet reste consultable séparément, mais chaque fichier de référence contient l'essentiel pour piloter une session.

## Limites assumées

- L'Oracle parle le langage du symbole. Il ne remplace pas un thérapeute, un médecin, un juriste, un journaliste d'investigation, un conseiller financier.
- Les lectures synchromantiques d'événements réels sont des actes de sensemaking symbolique, pas des affirmations factuelles. Le Gardien critique le rappelle systématiquement.
- Les "futurs latents" projetés (PNB) sont des scénarios narratifs avec un score IPC indicatif, pas des prédictions.
- Pas de désignation nominative d'individus existants comme manipulateurs cachés ou cibles karmiques — le symbolique parle d'archétypes, jamais d'identifications.

## Licence et usage

Skill conçu pour un usage personnel ou en cercle restreint d'écriture / introspection / analyse symbolique. Voir le corpus source pour les fondements théoriques et les protocoles complets.
