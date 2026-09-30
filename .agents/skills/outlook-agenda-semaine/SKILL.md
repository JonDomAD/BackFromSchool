---
name: outlook-agenda-semaine
description: Lire les réunions du calendrier professionnel Outlook de l'utilisateur pour la semaine civile en cours. À utiliser pour préparer la vue des réunions lors d'un retour en entreprise, notamment le lundi ou le jeudi.
---

# Agenda Outlook de la semaine

Détermine la semaine civile en cours dans le fuseau horaire de l'utilisateur, du lundi 00:00 au lundi suivant 00:00. Si le fuseau n'est pas fourni par le calendrier, utilise Europe/Paris. La semaine de l'agenda est indépendante de la date de début du rattrapage des mails et de Jira.

Avec le MCP Outlook/Microsoft 365, lis le calendrier professionnel de l'utilisateur connecté et récupère les occurrences réelles des réunions sur toute la semaine, y compris les réunions récurrentes. Vérifie la pagination. Retiens les invitations et réunions auxquelles l'utilisateur participe ou qu'il organise ; écarte les événements annulés, refusés, rappels et simples plages de disponibilité. Marque les invitations provisoires comme telles. Déduplique les occurrences exposées par plusieurs calendriers ou résultats.

Pour chaque réunion, relève le jour, l'heure locale de début et de fin, le titre, le statut de réponse, le lieu ou lien de participation et le lien vers l'événement lorsqu'ils sont disponibles. Respecte la confidentialité des événements privés : n'expose pas leur titre ou leurs participants si le connecteur les masque. Repère les chevauchements et distingue les réunions déjà passées de celles qui restent à venir au moment du lancement, particulièrement lorsque le retour a lieu un jeudi.

Utilise uniquement des opérations de lecture ; ne réponds pas aux invitations et ne modifie aucun événement. Si la connexion, la liste des calendriers ou les occurrences récurrentes sont inaccessibles, indique précisément la limite. Rends une liste normalisée et le nombre de réunions retenues pour le skill de visualisation ; n'invente aucun horaire ou lien.
