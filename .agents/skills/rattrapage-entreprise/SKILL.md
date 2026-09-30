---
name: rattrapage-entreprise
description: Produire dans Codex un compte rendu de retour en entreprise à partir des éléments non lus Outlook et Teams et des changements Jira concernant l'utilisateur, sur une période qu'il indique. À utiliser pour un rattrapage manuel après une période d'école.
---

# Rattrapage entreprise

Prépare un compte rendu en français pour un alternant qui revient en entreprise. L'utilisateur lance ce workflow manuellement et donne une date de début. Si cette date manque, demande-la avant toute consultation. Couvre la période allant de cette date à l'instant du lancement, dans la limite d'une semaine ; si la date est plus ancienne, demande une date dans cette limite. Indique les bornes effectivement utilisées dans le compte rendu.

## Sources

Utilise uniquement les connecteurs MCP disponibles et des opérations de lecture. N'envoie aucun message, ne marque aucun élément comme lu, ne modifie aucun ticket et ne crée aucun contenu dans les applications connectées. Si un outil de consultation change implicitement l'état « non lu », évite-le et signale la limite.

- **Outlook :** parcours toutes les boîtes auxquelles l'utilisateur a accès, sauf les corbeilles et éléments supprimés. Retiens uniquement les mails encore non lus dont la réception tombe dans la période. Lis le contenu nécessaire pour comprendre le sujet, les demandes et les échéances.
- **Teams :** parcours les conversations, canaux et notifications accessibles. Retiens uniquement les éléments encore non lus sur la période. Relis le contexte utile du fil sans présenter les anciens messages déjà lus comme de nouveaux éléments à rattraper.
- **Jira :** identifie les tickets dont l'utilisateur est actuellement assigné, créateur ou observateur. Retiens tous leurs changements intervenus pendant la période, qu'une notification ait été lue ou non : statut, attribution, priorité, échéance, description, commentaires et autres modifications utiles. Déduplique les tickets présents dans plusieurs catégories.

Si un connecteur est absent, échoue, ne permet pas de couvrir toutes les boîtes ou ne permet pas de vérifier l'état « non lu » ou l'historique Jira, indique précisément la couverture manquante. Ne présente jamais une recherche partielle comme exhaustive. N'invente ni éléments ni liens.

## Synthèse

Regroupe les messages et changements qui concernent un même sujet, même s'ils viennent de plusieurs canaux. Évalue l'importance à partir des échéances proches, demandes adressées à l'utilisateur, blocages, décisions, changements de priorité et conséquences possibles pour son travail. N'attribue pas une urgence sans indice dans les sources.

Rends un texte court en puces :

1. **À traiter en priorité :** sujets importants et action concrète attendue, si elle est établie.
2. **Autres sujets à rattraper :** faits et décisions utiles, regroupés par sujet.
3. **Couverture :** période, nombres d'éléments examinés par canal lorsque disponibles, et limites éventuelles.

Pour chaque sujet, donne une phrase ou deux et un lien vers les messages ou tickets sources lorsque le connecteur en fournit. Distingue une action demandée explicitement d'une action seulement suggérée. Si aucun élément pertinent n'est trouvé, dis-le clairement sans fabriquer de résumé.
