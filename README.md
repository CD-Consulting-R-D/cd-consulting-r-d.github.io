# cd-consulting-r-d.github.io

Depot racine du domaine **www.cd-consulting-rd.be**, servi par GitHub Pages
sous l'organisation [CD-Consulting-R-D](https://github.com/CD-Consulting-R-D).

**Statut : en construction** (un chapitre publie a ce jour : `/KB-RISK`, servi depuis son propre depot depuis le 08/09/2026).

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
| `/KB-RISK` | en ligne — base de connaissance risque, deux entrees (BKL-CDC-003, BKL-CDC-004) ; depuis le 08/09/2026 servie par le depot [`KB-RISK`](https://github.com/CD-Consulting-R-D/KB-RISK) (site de projet GitHub Pages sous le domaine), plus par un dossier de ce depot |
| `/KB-FIN` | depot [`KB-FIN`](https://github.com/CD-Consulting-R-D/KB-FIN) cree le 08/09/2026, Pages non active, aucune entree |
| `/KB-PHI` | depot [`KB-PHI`](https://github.com/CD-Consulting-R-D/KB-PHI) cree le 08/09/2026, Pages non active, aucune entree |
| `/KB-AI` | depot [`KB-AI`](https://github.com/CD-Consulting-R-D/KB-AI) cree le 08/09/2026, Pages non active, aucune entree |
| `/chatbot-knowledgebase` | annonce, non commence |

Chaque chapitre `KB-*` vit dans son propre depot de l'organisation et est servi comme
site de projet GitHub Pages sous le domaine (`https://www.cd-consulting-rd.be/<KB>/`) :
ce depot racine ne porte plus aucun contenu de connaissance, seulement l'accueil qui
pointe vers les chapitres. `/knowledgebase` et `/chatbot-knowledgebase` restent annonces,
non commences.

## Hors perimetre — nommement

- **Tout contenu de connaissance.** Les entrees vivent dans les depots de chapitre
  (`KB-RISK` en ligne ; `KB-FIN`, `KB-PHI`, `KB-AI` crees, vides) ; ce depot ne porte
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
