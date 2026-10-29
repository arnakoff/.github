<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/arnakoff/.github/main/profile/assets/banner-dark.svg">
    <img alt="Arnakoff : des signaux sourcés pour repérer les arnaques, en France." src="https://raw.githubusercontent.com/arnakoff/.github/main/profile/assets/banner-light.svg" width="100%">
  </picture>
</p>

**Arnakoff** construit une API publique et open source pour aider à repérer les arnaques en France. On lui donne un site, une adresse e-mail, un numéro de téléphone, un IBAN ou un numéro SIREN ; elle répond avec des **signaux sourcés**, expliqués en français clair.

> [!NOTE]
> Le projet est en cours de construction : aucune version n'est encore en service.

## Le problème

Les informations utiles pour repérer une arnaque existent déjà, mais elles sont éparpillées : listes noires de l'AMF et de l'ACPR, registre des entreprises, annonces légales, âge des noms de domaine, plan de numérotation téléphonique. Personne ne consulte six sites avant de payer.

Arnakoff les réunit en un seul appel, pour que n'importe quelle application, extension ou bot puisse prévenir ses utilisateurs au bon moment.

## Nos principes

- **Des sources officielles, toujours citées.** Chaque signal indique d'où il vient et à quelle date il a été observé.
- **Des faits, pas des verdicts.** Arnakoff ne dit jamais qu'un site est « sûr », ni qu'une entreprise est une « arnaque » : il décrit ce que les sources publiques montrent.
- **Le respect de la vie privée.** Les adresses e-mail, numéros et IBAN vérifiés ne sont ni conservés en clair ni transmis à des tiers.
- **Un code ouvert et vérifiable.** Chacun peut lire comment les signaux sont calculés.

## Les dépôts

| Dépôt | Contenu | Licence |
|---|---|---|
| [`api`](https://github.com/arnakoff/api) | L'API, la synchronisation des sources et le serveur MCP (Go) | AGPL-3.0 |
| [`web`](https://github.com/arnakoff/web) | Le site et la documentation de l'API | MIT |

## Les sources prévues

[Liste noire de l'AMF](https://www.data.gouv.fr/datasets/listes-noires-des-entites-non-autorisees-a-proposer-des-produits-ou-services-financiers-en-france) · [Liste noire de l'ACPR](https://www.abe-infoservice.fr/liste-noire) · [SIRENE](https://recherche-entreprises.api.gouv.fr) · [BODACC](https://bodacc-datadila.opendatasoft.com) · RDAP · [Numérotation de l'ARCEP](https://www.arcep.fr)

## Signaler une faille

Utilise le [signalement privé de vulnérabilités](https://github.com/arnakoff/api/security/advisories/new) du dépôt `api`. Merci de ne pas ouvrir d'issue publique pour une faille de sécurité.

---

<sub>French anti-scam API built on official open data. Work in progress.</sub>
