# Installation et Démarrage du Projet

Ce document explique comment installer Node.js 20, installer les dépendances du projet et démarrer l'API avec `npm run api`.

## 1. Installation de Node.js 20

Avant de commencer, assurez-vous d'avoir Node.js 20 installé sur votre machine.

### **Vérifier la version de Node.js**

Ouvrez un terminal et exécutez la commande suivante :

```sh
node -v
```

Si la version affichée est `v20.x.x`, vous pouvez passer à l'étape suivante. Sinon, suivez les instructions ci-dessous pour installer Node.js 20.

### **Installer Node.js 20**

- **Windows / MacOS / Linux** :

  1. Rendez-vous sur le site officiel : [https://nodejs.org/](https://nodejs.org/)
  2. Téléchargez la version **LTS** (recommandée) en version 20.x.x
  3. Installez le programme en suivant les instructions.
  4. Vérifiez l'installation avec `node -v`.

- **Via nvm (Node Version Manager) sur Linux/Mac** :

  1. Installez `nvm` si ce n'est pas déjà fait :
     ```sh
     curl -fsSL https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.4/install.sh | bash
     ```
  2. Fermez et rouvrez votre terminal, puis installez Node.js 20 :
     ```sh
     nvm install 20
     nvm use 20
     ```
  3. Vérifiez avec `node -v`.

## 2. Installation des dépendances du projet

Une fois Node.js 20 installé, accédez au répertoire du projet et exécutez :

```sh
npm install
```

Cette commande installera toutes les dépendances listées dans `package.json`.

## 3. Démarrer l'API

Une fois les dépendances installées, vous pouvez démarrer l'API avec la commande suivante :

```sh
npm run api
```

Cette commande exécutera le script défini dans `package.json`, permettant ainsi de lancer l'API.

### **Vérifier que l'API fonctionne**

Si tout est correct, vous devriez voir un message indiquant que le serveur est en cours d'exécution. Vous pouvez tester l'API en accédant à l'URL suivante dans votre navigateur ou via Postman :

```
http://localhost:3000
```

## 4. Problèmes Courants et Solutions

- **Problème : Commande **``** ne fonctionne pas**

  - Assurez-vous d'être dans le bon dossier de votre projet.
  - Supprimez le dossier `node_modules` et `package-lock.json`, puis réessayez :
    ```sh
    rm -rf node_modules package-lock.json
    npm install
    ```

- **Problème : L'API ne démarre pas**

  - Vérifiez le fichier `package.json` et assurez-vous que la commande `npm run api` est bien configurée.
  - Regardez les logs d'erreur dans le terminal pour plus d'informations.

## Conclusion

Félicitations ! 🎉 Vous avez installé Node.js 20, installé les dépendances et démarré l'API avec `npm run api`. Vous pouvez maintenant aller sur le projet [Treeslink](https://treeslink-test.netlify.app/) !

