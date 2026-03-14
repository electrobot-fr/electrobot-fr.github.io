# Coupe 2026

Le thème de cette année est **"Winter is Coming"**. Les robots jouent le rôle d'écureuils qui doivent constituer leurs réserves avant l'hiver. Des humains ont ramassé des noisettes dans des caisses, et pendant leur pause-café, les robots ont un temps limité pour récupérer les noisettes et les cacher. C'est une course contre la montre !

Le règlement: https://www.coupederobotique.fr/edition-2026/reglement-2026/

## Composants du robot

Le robot principal est télécommandé via une télécommande fabriquée avec un Arduino Uno (joysticks et boutons), reliée sans fil au robot par un pont ESP32 → ESP-NOW → ESP32-C3.

Le robot est composé de:
* 4 moteurs pas à pas pilotés par un ESP32 avec la bibliothèque FastAccelStepper
* 4 roues mecanum (déplacement omnidirectionnel)
* 4 pompes à vide, 4 électrovannes et 4 tapis roulants contrôlés par des modules PCA9685 (I2C) via un ESP32
* Un ESP32-C3 comme récepteur sans fil (ESP-NOW)
* Un afficheur TM1637 sur la télécommande
* Plusieurs convertisseurs DC-DC LM2596

Le PAMI est un petit robot autonome basé sur un ESP32-C3, déclenché par une tirette. Après un countdown de 85 secondes affiché sur un écran OLED, il exécute une séquence de déplacements pré-programmée (différente selon l'équipe Jaune ou Bleu) avec 2 moteurs pas à pas et un servo.

## Participants

Huit jeunes cette année :

* Adrien B
* Adrien R
* Aram
* Baya
* Henri
* Liam
* Mina
* Sao Mai

## Liens

Le code: https://github.com/electrobot-fr/coupe2026

## Vidéos
