# cd-consulting-r-d.github.io

Depot racine du domaine **www.cd-consulting-rd.be**, servi par GitHub Pages
sous l'organisation [CD-Consulting-R-D](https://github.com/CD-Consulting-R-D).

**Statut : en construction** (un projet publie a ce jour : `/KB-RISK`).

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
| `/KB-RISK` | en ligne — base de connaissance risque, une entree (BKL-CDC-003) |
| `/KB-FIN` | annonce, non commence |
| `/KB-PHI` | annonce, non commence |
| `/KB-AI` | annonce, non commence |
| `/chatbot-knowledgebase` | annonce, non commence |

`/KB-RISK` existe et sert une premiere entree (BKL-CDC-003) ; les cinq autres
chemins n'existent pas encore. Ils sont **nommes** par la page d'accueil, pas
servis : chacun fera l'objet de son propre mandat et, le cas echeant, de son
propre depot.

## Hors perimetre — nommement

- **Tout contenu de connaissance au-dela de KB-RISK.** Les bases KB-FIN,
  KB-PHI, KB-AI et le chatbot ne sont pas commences ; ce depot ne porte que le
  contenu audite et publie de `/KB-RISK`, aucune autre donnee brute.
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
