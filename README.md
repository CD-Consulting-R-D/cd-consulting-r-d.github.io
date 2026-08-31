# cd-consulting-r-d.github.io

Depot racine du domaine **www.cd-consulting-rd.be**, servi par GitHub Pages
sous l'organisation [CD-Consulting-R-D](https://github.com/CD-Consulting-R-D).

**Statut : en construction** (aucun projet publie a ce jour).

## Role

Ce depot porte trois choses, et rien d'autre :

- **`CNAME`** — la liaison du domaine personnalise `www.cd-consulting-rd.be`
  a GitHub Pages. **Ce fichier ne se supprime jamais** : sans lui, le domaine
  cesse de repondre.
- **`index.html`** — une page « under construction » en anglais, autoportante
  (CSS embarque, zero ressource externe), qui annonce les chemins a venir.
- **`.gitattributes` / `.gitignore`** — fins de ligne LF normalisees et
  exclusions de securite (patron de service, regles N-3 et N-4).

## Projets annonces, servis un jour sous le domaine

| Chemin | Etat |
|---|---|
| `/knowledgebase` (topics : Computer Science and AI ; Finance Economics Law & Risk Datamart ; Philosophy) | annonce, non commence |
| `/KB-RISK` | annonce, non commence |
| `/KB-FIN` | annonce, non commence |
| `/KB-PHI` | annonce, non commence |
| `/KB-AI` | annonce, non commence |
| `/chatbot-knowledgebase` | annonce, non commence |

Aucun de ces chemins n'existe. Ils sont **nommes** par la page d'accueil, pas
servis : chacun fera l'objet de son propre mandat et, le cas echeant, de son
propre depot.

## Hors perimetre — nommement

- **Tout contenu de connaissance.** Les bases KB et le chatbot ne sont pas
  commences ; ce depot ne porte aucune donnee, aucun index, aucun corpus.
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
