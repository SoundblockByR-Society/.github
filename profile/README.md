# Soundblock

## Description du Projet

Soundblock est une plateforme décentralisée de streaming musical est une application basée sur des smart contracts Ethereum qui permet aux utilisateurs de découvrir, écouter et partager de la musique de manière décentralisée. Les utilisateurs peuvent télécharger et publier leurs propres chansons sur la plateforme, tandis que les auditeurs peuvent écouter ces chansons en streaming. L'innovation principale de cette plateforme est d'introduire un modèle économique où chaque écoute d'une chanson entraîne un paiement automatique à l'artiste, permettant ainsi une rémunération directe et équitable des créateurs de musique.

## Démonstration

Vidéo: [https://youtu.be/RdCvt9zgg3M](https://youtu.be/RdCvt9zgg3M)

## Fonctionnalités Principales

Publication de Musique : Les artistes peuvent télécharger leurs chansons sur la plateforme en utilisant des smart contracts Ethereum.

Streaming Musical : Les auditeurs peuvent écouter de la musique en streaming depuis la plateforme sans avoir besoin de serveurs centralisés.

Gestion des Droits d'Auteur : Les smart contracts Ethereum assurent la gestion transparente des droits d'auteur et la rémunération des artistes pour leur travail. Chaque écoute d'une chanson entraîne un paiement automatique à l'artiste correspondant.

Rémunération Directe des Artistes : Les artistes reçoivent une rémunération directe et équitable à chaque écoute de leur musique, ce qui leur permet de gagner leur vie grâce à leur art.

Personnalisation des Pages d'Artiste : De par sa nature decentralisé les artistes pourrait trés bien personnaliser leur propre page qui utiliserait la plateforme, voire créer leur propre application basée sur notre backend, pour promouvoir leur musique et interagir avec leurs fans.

### Technologies Utilisées

Ce projet utilise les technologies suivantes :

Quasar Framework : Framework basé sur Vue.js pour le développement d'applications web et mobiles modernes. Il offre une large gamme de composants préfabriqués et facilite le développement rapide et efficace d'interfaces utilisateur attrayantes.

Express.js : Framework web minimaliste et flexible pour Node.js. Il est largement utilisé pour la création de serveurs back-end et d'API RESTful. Avec Express.js, il est facile de gérer les routes, les requêtes HTTP et les réponses.

Ethereum et Smart Contracts : Ethereum est une blockchain open-source qui prend en charge les contrats intelligents. Les contrats intelligents sont des programmes autonomes qui s'exécutent sur la blockchain Ethereum et qui peuvent être utilisés pour automatiser des processus et établir des accords numériques.

Hardhat : Hardhat est un framework de développement Ethereum qui simplifie la création, le test et le déploiement de smart contracts. Il offre un ensemble d'outils et de fonctionnalités pour faciliter le développement des contrats intelligents de manière efficace et sécurisée.

## Architecture

Soundblock est une application (quasi-)decentralisee. Elle se compose de trois élèments:

- Des smarts contracts sur Etherum: [https://github.com/SoundblockByR-Society/soundblock-sc](https://github.com/SoundblockByR-Society/soundblock-sc)
- Un Back-End: [https://github.com/SoundblockByR-Society/soundblock-backend](https://github.com/SoundblockByR-Society/soundblock-backend)
- Un Front-End: [https://github.com/SoundblockByR-Society/soundblock-front.git](https://github.com/SoundblockByR-Society/soundblock-front.git)

Le Back-end est nécessaire pour le streaming des oeuvres musicales des artistes et les interactions avec l'infrastructure de stockage (elle empêche les auditeurs de simplement accéder à l'oeuvre au format de fichier). C'est la seule partie centralisée. Elle pourrait se décentralisée avec des blockchains comme CHAINLINK et STORJ. Ce qui ferait de la plateforme un "Deezer"-like totalement décentralisé et appartenant aux artistes.
Cette partie ne gère aucune transaction de crypto-monnaie et n'est en réalite qu'une API REST qui sert de proxy.

## Installation

### Clonez ce référentiel sur votre machine locale.

```
git clone https://github.com/SoundblockByR-Society/soundblock-backend.git

git clone https://github.com/SoundblockByR-Society/soundblock-front.git

git clone https://github.com/SoundblockByR-Society/soundblock-sc.git
```

### Accédez au répertoire du projet.

```
cd ./soundblock-backend
```

### Installez les dépendances nécessaires en exécutant la commande suivante :

```
npm install
```

### Lancez le serveur en exécutant la commande suivante :

```
npm run dev
```

### Accédez au répertoire du smart contract.

```
cd ./soundblock-sc
```

### Installez les dépendances nécessaires en exécutant la commande suivante :

```
npm install
```

### Compilez et déployez les smart contracts Ethereum .

```
npx hardhat compile
```

### Démarrez le serveur de développement en exécutant la commande suivante :

```
npx hardhat node
```

### lancez le script de déploiement des contrats en exécutant la commande suivante :

```
npx hardhat run scripts/deploy.ts --network localhost
```

### Accédez au répertoire du frontend.

```
cd ./soundblock-front
```

### Installez les dépendances nécessaires en exécutant la commande suivante :

```
npm install
```

### Lancez le serveur de développement en exécutant la commande suivante :

```
quasar dev
```

## Utilisation

Accédez à l'application dans votre navigateur en ouvrant l'URL suivante : http://localhost:3000.

Explorez la plateforme, téléchargez de la musique, écoutez vos chansons préférées et partagez-les avec d'autres utilisateurs !
