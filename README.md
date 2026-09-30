# BackFromSchool

Un workflow Codex pour préparer, à la demande, un compte rendu de retour en entreprise après une période d'école.

## Utilisation

Dans ce projet, lancer le skill avec une date de début récente :

```text
$rattrapage-entreprise Fais mon rattrapage depuis le JJ/MM/AAAA.
```

La période va jusqu'au lancement et ne dépasse pas une semaine. Le compte rendu regroupe les mails et échanges Teams non lus, ainsi que les changements Jira sur les tickets dont l'utilisateur est assigné, créateur ou observateur. Il présente aussi les réunions Outlook de la semaine civile en cours, du lundi au dimanche, avec un visuel dans Codex.

Le point d'entrée est [rattrapage-entreprise](.agents/skills/rattrapage-entreprise/SKILL.md). Il s'appuie sur six skills spécialisés : [Outlook non lus](.agents/skills/outlook-non-lus-retour/SKILL.md), [Teams non lus](.agents/skills/teams-non-lus-retour/SKILL.md), [changements Jira](.agents/skills/jira-changements-concernes/SKILL.md), [agenda Outlook](.agents/skills/outlook-agenda-semaine/SKILL.md), [vue des réunions](.agents/skills/visuel-reunions-semaine/SKILL.md) et [envoi du compte rendu par mail](.agents/skills/envoi-compte-rendu-mail/SKILL.md).

Le workflow nécessite des connecteurs MCP Outlook, Teams et Jira disponibles dans Codex. La collecte utilise uniquement des opérations de lecture. Une fois le compte rendu terminé, l'agent envoie le bilan et la liste textuelle des réunions à la propre boîte Outlook de l'utilisateur ; le visuel hebdomadaire est affiché dans Codex.
