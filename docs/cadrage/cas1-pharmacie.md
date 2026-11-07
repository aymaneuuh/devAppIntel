# Fiche de cadrage : Ordonnances incomplètes en pharmacie

## Besoin en une phrase (obligatoire)

Détecter automatiquement les informations manquantes ou incorrectes dans une ordonnance afin d'aider le pharmacien à vérifier sa conformité avant la délivrance des médicaments.

## Utilisateur final (obligatoire)

Le pharmacien ou le préparateur en pharmacie chargé de vérifier les ordonnances et de sécuriser la délivrance des médicaments.

## Approche retenue (obligatoire)

Cocher une seule case :

- [x] Règles métier
- [ ] Machine learning
- [ ] RAG
- [ ] Modèle génératif seul

## Justification (obligatoire)

Les règles métier sont adaptées car (a) un jeu de données étiquetées n'est pas indispensable et (b) les champs obligatoires d'une ordonnance peuvent être vérifiés à partir de règles explicites. De plus, (d) une erreur peut avoir des conséquences sur la santé du patient, ce qui justifie une vérification humaine systématique.

## Données nécessaires et leur origine (obligatoire)

Les données nécessaires sont les champs d'une ordonnance : identité du patient, informations du prescripteur, médicaments prescrits, dosage et date. Elles proviennent des ordonnances et des règles officielles applicables, avec un accès limité aux données personnelles.

## Métrique de succès et seuil d'acceptation (obligatoire)

Atteindre au moins 95 % de détection des champs obligatoires manquants sur un jeu de test représentatif. Le système doit également limiter les fausses alertes à moins de 5 %.

## Conséquence d'une erreur et validation humaine prévue (obligatoire)

Une erreur peut entraîner une mauvaise interprétation de l'ordonnance ou une délivrance inadaptée. Le pharmacien doit obligatoirement vérifier les alertes et prendre la décision finale.

## Risques éthiques ou de confidentialité (obligatoire)

Les ordonnances contiennent des données personnelles et médicales sensibles. Leur traitement doit respecter la confidentialité, limiter les accès et garantir la protection des données des patients.

## Approche écartée et pourquoi (facultatif)

Le machine learning est écarté car les règles de vérification sont explicites et ne nécessitent pas forcément un historique d'ordonnances étiquetées. Un modèle génératif seul est également écarté en raison du risque d'erreurs non vérifiables.