# cd-consulting-r-d.github.io

Depot racine du domaine **www.cd-consulting-rd.be**, servi par GitHub Pages
sous l'organisation [CD-Consulting-R-D](https://github.com/CD-Consulting-R-D).

**Statut : en construction** (deux chapitres publies a ce jour : `/KB-RISK` et `/KB-FIN`, chacun servi depuis son propre depot depuis le 08/09/2026).

## Role

Ce depot porte trois choses, et rien d'autre :

- **`CNAME`** — la liaison du domaine personnalise `www.cd-consulting-rd.be`
  a GitHub Pages. **Ce fichier ne se supprime jamais** : sans lui, le domaine
  cesse de repondre.
- **`index.html`** — la page d'accueil « Knowledge Base » en anglais, autoportante
  (CSS embarque, zero ressource externe), qui pointe vers la derniere entree
  publiee et annonce les chemins a venir.
- **`.gitattributes` / `.gitignore`** — fins de ligne LF normalisees et
  exclusions de securite (patron de service, regles N-3 et N-4).

## Projets annonces, servis un jour sous le domaine

| Chemin | Etat |
|---|---|
| `/knowledgebase` (topics : Computer Science and AI ; Finance Economics Law & Risk Datamart ; Philosophy) | annonce, non commence |
| `/KB-RISK` | en ligne — base de connaissance risque, trois entrees ; depuis le 08/09/2026 servie par le depot [`KB-RISK`](https://github.com/CD-Consulting-R-D/KB-RISK) (site de projet GitHub Pages sous le domaine), plus par un dossier de ce depot |
| `/KB-FIN` | en ligne depuis le 08/09/2026 — finance, economie, droit et datamart risque, une entree ; servie par le depot [`KB-FIN`](https://github.com/CD-Consulting-R-D/KB-FIN) (site de projet GitHub Pages sous le domaine) |
| `/KB-PHI` | en ligne depuis le 09/09/2026 — philosophie, deux entrees (dossier Searle, The Mystery of Consciousness, 1997 : synthese et rapport detaille, en francais) ; servie par le depot [`KB-PHI`](https://github.com/CD-Consulting-R-D/KB-PHI) (site de projet GitHub Pages sous le domaine) |
| `/KB-AI` | depot [`KB-AI`](https://github.com/CD-Consulting-R-D/KB-AI) en ligne depuis le 09/09/2026, 1 entree (resume 2026 AI Barometer BE) |
| `/KB-DEV` | en ligne depuis le 09/09/2026 — developpement logiciel, trois entrees ; servie par le depot [`KB-DEV`](https://github.com/CD-Consulting-R-D/KB-DEV) (site de projet GitHub Pages sous le domaine) |
| `/KB-ECON` | en ligne depuis le 10/09/2026 — economie et modelisation economique, une entree (Agent-based Computational Economics, corpus 2001-2005 actualise 2026) ; servie par le depot [`KB-ECON`](https://github.com/CD-Consulting-R-D/KB-ECON) (site de projet GitHub Pages sous le domaine) |
| `/chatbot-knowledgebase` | annonce, non commence |

Chaque chapitre `KB-*` vit dans son propre depot de l'organisation et est servi comme
site de projet GitHub Pages sous le domaine (`https://www.cd-consulting-rd.be/<KB>/`) :
ce depot racine ne porte plus aucun contenu de connaissance, seulement l'accueil qui
pointe vers les chapitres. `/knowledgebase` et `/chatbot-knowledgebase` restent annonces,
non commences.

## Hors perimetre — nommement

- **Tout contenu de connaissance.** Les entrees vivent dans les depots de chapitre
  (`KB-RISK`, `KB-FIN`, `KB-AI`, `KB-PHI` et `KB-DEV` en ligne) ; ce depot ne porte
  que l'accueil, aucune donnee brute.
- **Toute fonction serveur.** Site statique pur : pas de Netlify, pas de
  Supabase, pas de build, pas de dependance, pas de `node_modules`.
- **Tout secret.** Ce depot n'en manipule aucun et n'a aucune variable de
  plateforme.
- **Le DNS et le certificat.** Ils vivent chez le registrar (Infomaniak) et
  chez GitHub ; ce depot n'en porte que le `CNAME`. Le plan de saisie est
  tenu hors depot par le proprietaire.
- **La collecte de donnees.** Aucun formulaire, aucun cookie, aucun script,
  aucune mesure d'audience.

## Notes de tenue

- Branche servie : **`master`**, seule branche. Publier, c'est pousser sur
  `master` — tout commit pousse est une mise en ligne.
- Encodage : UTF-8 **sans BOM**, fins de ligne **LF**.
- La page ne charge **aucune** ressource distante : elle s'ouvre a l'identique
  hors ligne. Les seuls liens sortants sont volontaires et pointent vers
  `www.cdatso.be` (prototypes) et l'organisation GitHub.
