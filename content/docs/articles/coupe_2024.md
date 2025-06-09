# Coupe 2024

Pour notre première participation à la Coupe de France, nous sommes arrivés 37ème sur 49.

Les équipes devaient imaginer des robots capables de permettre à une serre martienne de produire de la nourriture pour une expédition humaine sur Mars.

![game](/game2024.jpg)



## Composants du robot

Notre robot est composé de:
* 4 moteurs DC jaunes 
* 4 roues mecanum
* Un Arduino Mega
* 2 ponts en H L298N
* Des servos (standard et micro)
* Une batterie Parkside et un [support imprimé en 3D](https://www.thingiverse.com/thing:4445077)
* Plusieurs convertisseurs DC-DC LM2596
* Un afficheur TM1637

La pince est une adaptation de ce modèle trouvé sur [Thingiverse](https://www.thingiverse.com/thing:1015238).

La télécommande est fabriquée en bois découpé au laser. Il s’agit d’une [boîte générée](https://boxes.hackerspace-bamberg.de/) en ligne. Elle est reliée au robot par un câble Ethernet (utilisé pour une liaison série), ainsi qu’une paire de câbles pour l’alimentation.

Côté code, voici quelques bibliothèques intéressantes :

* [SerialTransfer](https://github.com/PowerBroker2/SerialTransfer) : permet une communication série fiable.
* [TM1637Display](https://github.com/avishorp/TM1637) : pour afficher le score sur un petit module à 4 chiffres, en utilisant seulement 4 fils et 3 lignes de code.

## Participants

Quatre jeunes cette année :

* Adrien Bailly
* Adrien Rose
* Henri Joubert
* Stanislas Adam

![team](/team2024.png)

## Liens

Le code: https://github.com/electrobot-fr/coupe2024

Le règlement: https://github.com/electrobot-fr/coupe2024/blob/main/Eurobot2024_Rules_JR_FR_FINAL.pdf

## Vidéos

{{< youtube WoJPhy2j6gk >}}

