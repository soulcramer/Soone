# BACKEND INFO

## Commandes Node depuis le Node.js command prompt :
-npm install sails -g //installe sails au niveau de l'installation NodeJs de la machine
-cd soone-backend
-npm install
-sails lift //lancer le serveur


## Configuration initiale du projet
-sails new "soone-backend" //création du projet, ne pas reproduire
-2 //le projet a été créé en mode empty, ne pas reproduire

## Lancement des tests unitaires
-cd soone-backend
-npm test //script configuré dans package.json

## Lancement des tests semi auto
-cd soone-backend
-Dans package.json, remplacer "custom-tests" par :
    "custom-tests": "node ./node_modules/mocha/bin/mocha test/lifecycle.test.js test/api/**/*.test.manual.js"
-Dans test/lifecycle.test.js, mettre le token de l'application
-npm test