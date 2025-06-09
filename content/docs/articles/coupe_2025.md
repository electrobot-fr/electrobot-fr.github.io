# Coupe 2025

Cette année, nous sommes arrivés 5ème à la Coupe Régionale d'Ile-de-France et 7ème sur 49 à la Coupe de France.

## Composants du robot

Notre robot est composé de:
* 4 moteurs JGB37-520 333rpm
* 4 roues mecanum
* Un ESP32 qui fait une [pont 2.4GHz](https://github.com/electrobot-fr/coupe2025/blob/main/serial2serial/src/bridge.ino) entre la télécommande et le robot (la liaison est toujours série)
* Un Arduino Mega et un sensor shield (pour brancher les servos facilement)
* Un Arduino Uno pour la commande des moteurs
* Un CNC shield v3 et des TMC2209 pour commander les moteurs pas à pas
* Une pompe à vide, une électrovanne, un [manipulateur](https://fr.aliexpress.com/item/1005006009299791.html) et des ventouses trouvés sur Aliexpress
* Des [modules mosfet](https://fr.aliexpress.com/item/1005006457613501.html) pour contrôler la pompe et l'électrovanne (12V) avec un Arduino
* Une [pince pour les boites de conserve](https://www.printables.com/model/1154981-halbach-array-magnet-gripper/files) faite par l'équipe Karibous
* 2 ponts en H L298N
* Des servos (standard et micro)
* Une batterie Parkside et un [support imprimé en 3D](https://www.thingiverse.com/thing:4445077)
* Plusieurs convertisseurs DC-DC LM2596
* Un afficheur TM1637

Dans la télécommande, il y a un ESP32 pour la communication sans fil et un Arduino qui s'occupe des boutons.

Les PAMIs sont réalisés avec des moteurs pas à pas [17HE08-1004S](https://www.omc-stepperonline.com/fr/e-serie-nema-17-bipolar-1-8deg-17ncm-24-07oz-in-1a-42x42x23mm-4-fils-17he08-1004s), un CNC shield v3 et un Arduino Uno.

Cette année, nous avons beaucoup utilisé la découpeuse laser. Pour la conception, nous avons tout fait avec Fusion 360 et surtout ce petit outil pour faire les [jointures](https://github.com/FlorianPommerening/FingerJoints).

## Participants

Sept jeunes cette année :

* Adrien B
* Adrien R
* Alexandre
* Henri
* Liam
* Mina
* Thomas

![team](/team2025.1.jpg)
![photo](/2025/PXL_20250419_094654783.jpg)
![team](/mascotte.jpg)

## Liens

Le code: https://github.com/electrobot-fr/coupe2025

Le règlement: https://github.com/electrobot-fr/coupe2025/blob/main/Eurobot2025_Rules.pdf

## Photos

Prototype de base roulante

![photo](/2025/IMG_0852.jpg)

Avec la télécommande

![photo](/2025/IMG_0920.jpg)

L'ascenceur et les pinces

![photo](/2025/IMG_0925.jpg)

Le stand et le robot à la Coupe d'IDF

![photo](/2025/PXL_20250419_084221866.jpg)
![photo](/2025/PXL_20250419_101002633.MP~2.jpg)

Installation lors des matchs

![photo](/2025/PXL_20250419_141300579.jpg)

## Vidéos

PAMI en cours de conception:

{{< video src="/pami.mp4" width=300px >}}

Ascenceur et ventouses

{{< video src="/2025/IMG_0899.mp4" width=300px >}}

Le robot roule !

{{< video src="/2025/IMG_0958.mp4" width=300px >}}
{{< video src="/2025/IMG_1025.mp4" >}}
