# BackFromSchool

Un workflow Codex pour préparer, à la demande, un compte rendu de retour en entreprise après une période d'école.

## Utilisation

Dans ce projet, lancer le skill avec une date de début récente :

```text
$rattrapage-entreprise Fais mon rattrapage depuis le 24 septembre 2026.
```

La période va jusqu'au lancement et ne dépasse pas une semaine. Le compte rendu regroupe les mails et échanges Teams non lus, ainsi que les changements Jira sur les tickets dont l'utilisateur est assigné, créateur ou observateur.

Le point d'entrée est [rattrapage-entreprise](.agents/skills/rattrapage-entreprise/SKILL.md). Il s'appuie sur trois skills spécialisés : [Outlook non lus](.agents/skills/outlook-non-lus-retour/SKILL.md), [Teams non lus](.agents/skills/teams-non-lus-retour/SKILL.md) et [changements Jira](.agents/skills/jira-changements-concernes/SKILL.md). Cette séparation permet d'affiner chaque source sans alourdir la synthèse.

Le workflow nécessite des connecteurs MCP Outlook, Teams et Jira disponibles dans Codex. Il utilise uniquement des opérations de lecture.
