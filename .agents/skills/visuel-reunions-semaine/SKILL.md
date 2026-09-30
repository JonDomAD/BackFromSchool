---
name: visuel-reunions-semaine
description: Transformer les réunions vérifiées de la semaine en une vue hebdomadaire lisible dans Codex, avec les prochaines réunions et conflits visibles. À utiliser après la lecture de l'agenda Outlook, sans consulter ni modifier le calendrier.
---

# Vue des réunions de la semaine

À partir des seules réunions vérifiées par le skill de lecture d'agenda, produis dans Codex un visuel compact de la semaine civile, du lundi au dimanche, en heure locale. Affiche les jours, les heures et la durée des réunions. Distingue clairement les réunions passées, celles à venir, les invitations provisoires et les chevauchements. Un jour vide doit rester identifiable. Le lundi et le jeudi de retour en entreprise, mets en évidence les prochaines réunions sans effacer le reste de la semaine.

Utilise une visualisation intégrée à la conversation lorsque cette capacité est disponible et adaptée à une vue hebdomadaire ; suis alors les instructions du skill de visualisation disponible dans l'environnement. Sinon, rends une grille ou un tableau Markdown lisible sur écran étroit. Garde un équivalent textuel court, classé par jour et heure, pour l'accessibilité et pour le mail final. Les liens d'événement restent cliquables lorsqu'ils sont disponibles.

Ne consulte pas de source supplémentaire et ne crée ni ne modifie d'événement. Si l'agenda est inaccessible, affiche simplement « Agenda indisponible » avec la cause connue ; ne dessine pas une semaine vide qui suggérerait qu'aucune réunion n'est prévue.
