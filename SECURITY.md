# Politique de sécurité

Arnakoff aide à repérer les arnaques : une faille chez nous peut nuire à celles et ceux qui comptent sur nous. Merci de prendre le temps de nous la signaler.

## Signaler une faille

**Ne publie pas la faille dans une issue, une discussion ou une pull request.**

1. **Canal principal** : le signalement privé de vulnérabilités de GitHub, dans l'onglet **Security** du dépôt concerné, bouton **Report a vulnerability** (par exemple [pour l'API](https://github.com/arnakoff/api/security/advisories/new)). Le [guide de GitHub](https://docs.github.com/fr/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability) explique la démarche.
2. **Si tu ne peux pas utiliser GitHub** : écris à [security@arnakoff.com](mailto:security@arnakoff.com).

Indique si possible :

- le composant et la version ou le commit concernés ;
- les étapes pour reproduire, et l'impact que tu as constaté ;
- toute idée de correctif.

## Périmètre

Dans le périmètre :

- l'API, la synchronisation des sources et le serveur MCP (dépôt [`api`](https://github.com/arnakoff/api)) ;
- le site et la documentation (dépôt [`web`](https://github.com/arnakoff/web)) ;
- l'image Docker publiée par le projet ;
- les services hébergés par Arnakoff, une fois en service.

Hors périmètre :

- le déni de service volumétrique, et tout test qui dégrade le service pour les autres ;
- l'ingénierie sociale, le hameçonnage ou toute action visant des personnes ;
- les failles des services tiers que nous utilisons (GitHub, Cloudflare, OVHcloud…) : signale-les directement à leur éditeur.

## Nos engagements

| Étape | Délai |
|---|---|
| Accusé de réception | 3 jours ouvrés |
| Première évaluation (gravité, périmètre) | 10 jours ouvrés |
| Correctif d'une faille critique ou haute | 30 jours |
| Correctif d'une faille moyenne ou basse | 90 jours |

Nous te tenons informé de l'avancement et te prévenons avant toute publication.

## Divulgation coordonnée

Nous publions un avis de sécurité GitHub une fois le correctif disponible, et te créditons si tu le souhaites. Merci d'attendre cette publication, ou au plus 90 jours après ton signalement, avant de rendre la faille publique. Nous pouvons convenir ensemble d'un autre délai.

## Protection des chercheurs de bonne foi

Nous n'engagerons aucune poursuite et ne demanderons aucune action contre toi si, dans tes recherches :

- tu agis de bonne foi et restes dans le périmètre ci-dessus ;
- tu n'accèdes qu'au strict nécessaire pour démontrer la faille, sans consulter, modifier, conserver ni divulguer de données personnelles ;
- tu ne dégrades pas le service et n'affectes pas les autres utilisateurs ;
- tu nous laisses le temps de corriger avant toute divulgation.

## Versions prises en charge

Les correctifs de sécurité sont publiés pour la dernière version mineure de chaque composant. Aucune version n'est encore publiée : d'ici là, seule la branche `main` est prise en charge.
