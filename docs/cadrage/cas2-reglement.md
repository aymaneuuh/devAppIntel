# Fiche de cadrage : Questions sur le règlement intérieur

## Besoin en une phrase (obligatoire)

Permettre aux utilisateurs de poser des questions sur le règlement intérieur et d'obtenir des réponses précises basées sur les documents officiels.

## Utilisateur final (obligatoire)

Les employés, les étudiants ou les membres d'une organisation qui souhaitent comprendre les règles et les procédures du règlement intérieur.

## Approche retenue (obligatoire)

Cocher une seule case :

- [ ] Règles métier
- [ ] Machine learning
- [x] RAG
- [ ] Modèle génératif seul

## Justification (obligatoire)

Le RAG est adapté car (b) les réponses peuvent être vérifiées à partir des passages du règlement intérieur et des sources citées. Le système n'a pas besoin d'un grand jeu de données étiquetées (a), et son coût par requête reste raisonnable (c) grâce à la recherche ciblée dans les documents.

## Données nécessaires et leur origine (obligatoire)

Les données nécessaires sont les règlements intérieurs, les procédures officielles, les notes de service et leurs éventuelles mises à jour. Ces documents proviennent des responsables de l'organisation et doivent être régulièrement actualisés.

## Métrique de succès et seuil d'acceptation (obligatoire)

Obtenir au moins 90 % de réponses correctes sur un ensemble de questions de test. Au moins 95 % des réponses fournies doivent être accompagnées d'une référence pertinente au document source.

## Conséquence d'une erreur et validation humaine prévue (obligatoire)

Une réponse incorrecte peut induire l'utilisateur en erreur concernant ses droits ou ses obligations. Les réponses doivent mentionner leurs sources et les cas ambigus ou importants doivent être vérifiés auprès d'un responsable.

## Risques éthiques ou de confidentialité (obligatoire)

Le système doit éviter de divulguer des documents confidentiels ou des informations personnelles. Il faut également prévenir les réponses inventées et tenir compte des versions obsolètes du règlement.

## Approche écartée et pourquoi (facultatif)

Un modèle génératif seul est écarté car il peut produire des informations incorrectes sans référence fiable. Les règles métier seules ne permettent pas de répondre facilement à toutes les formulations possibles des utilisateurs.