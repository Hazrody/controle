# WorkBox 
## Simple Définition :
`Workbox est un ensemble de modules permettant de simplifier le service worker d'un point de vue 'routing' et 'caching'.
Chaque module disponible aborde un aspect spécifque de développement du 'service worker', l'objectif est de rendre aussi simple possible l'utilisation du service worker en permettant une flexibilité pour répondre au mieux au exigences des applications.
src:https://developer.chrome.com/docs/workbox/what-is-workbox/ `

## Listes des fonctionnalités offertes
### Gestion du cache
Fourniture de stratégie de mise en cache. (ex : Requête réseau et API, etc...)
### Gestion des erreurs
Fourniture des stratégies pour gérer les erreurs de réseau et requête.
### Utilisation hors ligne
Permet d'utiliser l'application hors ligne en fournissant des solutions de mise/gestion de cache pour les ressources dynamiques.
### Intégration avec les frameworks JS
Intégration facile avec les frameworks JavaScript.
### Gestion des mises à jour
Pour gérer les mises à jour du cache automatiquement pour les fichiers statiques.
### Préchargement
Permet de précharger des ressources importantes pour améliorer la performance et la rapidité d'une application.
### Analytics 
Permet de faire du 'monitoring' en utilisant Google Analytics et d'autres outils de suivi d'analyse.

Source : https://web.dev/learn/pwa/workbox/

## Méthodes de cache et utilisations possibles
### Présentation
Les méthodes de cache sont des outils puissants permettant aux applications d'être moins dépendantes des conditions réseau. Grâce à une bonne utilisations des caches, nous pouvons rendre nos application Web disponible même hors ligne et de répondre à des requêtes rapidement peu importe nos conditions réseaux.
Pour faire cela le `service worker` utilise l'`API de stockage de cache` => https://developer.mozilla.org/fr/docs/Web/API/CacheStorage.

### Utilisations possibles
1. Mise en cache des ressources minimales pour l'interface utilisateur. (Exemple: Page HTML,CSS,Image utilisée, fichier js de l'interface, police web, etc... )
2. Eviter les messages d'erreur lorsque la page ne peut pas charger par exemple. 
3. Stocker les données à la première utilisation.

Source: https://web.dev/learn/pwa/caching/

## Uses cases à intégrer dans le projet doctoliberal

1. La gestion de cache : Par exemple pour l'interface, les rendez-vous du jours lors du premier appel,etc... 
2. Le module background sync: Pour effectuer une demande réseau fiable même si l'utilisateur est hors ligne
3. Etc....
