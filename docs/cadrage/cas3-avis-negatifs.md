# Fiche de cadrage : Priorisation des avis négatifs

## Besoin en une phrase (obligatoire)

Identifier et classer automatiquement les avis clients négatifs afin de permettre aux équipes de traiter en priorité les réclamations les plus importantes.

## Utilisateur final (obligatoire)

Les équipes du service client, les responsables qualité et les gestionnaires de la relation client.

## Approche retenue (obligatoire)

Cocher une seule case :

- [ ] Règles métier
- [x] Machine learning
- [ ] RAG
- [ ] Modèle génératif seul

## Justification (obligatoire)

Le machine learning est adapté car (a) des avis clients étiquetés peuvent être utilisés pour entraîner un modèle de classification et (c) le traitement automatique permet de gérer un grand volume d'avis à faible coût par requête. Le modèle peut également apprendre des formulations variées difficiles à couvrir uniquement avec des règles métier.

## Données nécessaires et leur origine (obligatoire)

Les données nécessaires sont les avis clients historiques, leur texte, leur date et leur catégorie de priorité. Elles proviennent des plateformes d'avis et des historiques du service client, après anonymisation des informations personnelles.

## Métrique de succès et seuil d'acceptation (obligatoire)

Atteindre un score F1 d'au moins 0,80 sur les catégories de priorité et un rappel d'au moins 90 % pour les avis négatifs prioritaires. Les performances doivent être évaluées sur des données qui n'ont pas servi à entraîner le modèle.

## Conséquence d'une erreur et validation humaine prévue (obligatoire)

Un avis urgent mal classé peut retarder le traitement d'une réclamation importante. Les équipes du service client doivent pouvoir vérifier les priorités proposées et modifier la classification si nécessaire.

## Risques éthiques ou de confidentialité (obligatoire)

Les avis peuvent contenir des informations personnelles ou des propos sensibles. Il faut anonymiser les données, éviter les biais de classification et ne pas prendre de décision importante concernant un client uniquement sur la base du modèle.

## Approche écartée et pourquoi (facultatif)

Les règles métier sont écartées comme approche principale car elles détectent difficilement toutes les expressions et nuances du langage naturel. Le RAG n'est pas nécessaire car le besoin principal est la classification et non la recherche d'informations dans des documents.