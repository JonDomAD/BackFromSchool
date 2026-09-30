---
name: envoi-compte-rendu-mail
description: Envoyer à l'utilisateur, par Outlook, le compte rendu final de son rattrapage d'entreprise. À utiliser uniquement après la synthèse complète demandée par le workflow rattrapage-entreprise ou sur demande explicite d'envoi de ce compte rendu.
---

# Envoi du compte rendu par mail

Utilise ce skill une seule fois après avoir terminé le compte rendu de rattrapage. Le destinataire est l'adresse Outlook personnelle de l'utilisateur connecté, déterminée par le profil du connecteur. Si plusieurs adresses peuvent désigner sa boîte et qu'aucune adresse principale n'est identifiable, demande laquelle utiliser avant l'envoi. Ne déduis jamais l'adresse d'un message reçu ou d'un ticket Jira.

Envoie le compte rendu final avec le MCP Outlook. Objet : `Rattrapage entreprise — <date de début> au <date de fin>`. Le corps reprend la synthèse courte, ses liens sources, les réunions de la semaine classées par jour et heure en texte, et les limites de couverture. Le visuel de l'agenda reste dans Codex. N'ajoute aucun autre destinataire, copie, copie cachée ni pièce jointe. N'envoie pas de message intermédiaire et ne transforme pas le compte rendu en instructions adressées aux personnes citées.

L'envoi de ce mail est la seule écriture externe autorisée par ce workflow. Ne marque aucun mail ou message comme lu et ne modifie aucun ticket. Si le connecteur ne peut pas envoyer, conserve le compte rendu dans la réponse Codex et indique que l'envoi n'a pas eu lieu. Si la réponse de l'outil est ambiguë, vérifie l'état de l'envoi en lecture seule avant toute nouvelle tentative ; ne renvoie pas automatiquement un second exemplaire.

Après l'envoi confirmé, affiche les mêmes faits dans Codex avec le visuel de l'agenda et indique l'adresse de destination. N'affirme pas que le mail est parti sans confirmation du connecteur.
