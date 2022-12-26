# Démarrer un nouveau projet Symfony

Cette configuration répond à mes besoins et mes pratiques. Elle ne se veut pas être une règle absolue.

## Installation du "back"

* Installation de Symfony "Skeleton"

```bash
composer create-project symfony/skeleton nomDuProjet
cd nomDuProjet
```

* Installation des dépendances de développement

**Dans le repertoire du projet**

```bash
composer require profiler maker --dev
```

* Installation des dépendances

Les besoins classiques sont : Base de données (orm), formulaire et validation (form + validation), annotation et Twig (annotation + twig), 
sécurité (security)

```bash
composer require orm-pack form validation annotation twig security
```

* Si besoin de mail

```bash
composer require mailer messenger
```

## La partie "Front" avec Symfony

* A minima, webpack

```bash
composer require webpack-encore
yarn install --force
```

* Stimulus

