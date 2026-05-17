# Coupe 2026

Le thème de cette année est **"Winter is Coming"**. Les robots jouent le rôle d'écureuils qui doivent constituer leurs réserves avant l'hiver. Des humains ont ramassé des noisettes dans des caisses, et pendant leur pause-café, les robots ont un temps limité pour récupérer les noisettes et les cacher. C'est une course contre la montre !

Cette année, nous sommes arrivés 5ème aux qualifications de la Coupe Régionale d'Ile-de-France, puis **2ème à la Coupe de France** !

Le règlement: https://www.coupederobotique.fr/edition-2026/reglement-2026/

## Coupe de France

Nous sommes arrivés 5ème à l'issue des matchs de série. 

Le hasard nous a fait rencontrer Bot'Vives avec qui nous nous sommes entraînés au lab.

{{< youtube SrCPZ5dl2Qo >}}

### Phases finales

{{< mermaid >}}
graph LR
    subgraph R8["8ème de finale"]
        r1["Bot'Vives 137-98 Aspi'Nuts"]
        r2["Hivertaco 98-88 Labocesson 1"]
        r3["Les C. Circuits 92-73 LATTERE"]
        r4["Electrobot 132-64 Ingenium"]
        r5["Game Team 111-84 Academy AI"]
        r6["Labocesson 2 116-91 Firebot"]
        r7["Flybot 161-81 NOL Team"]
        r8["Les Vertaco 148-96 C'est La Team"]
    end

    subgraph QF["Quart de finale"]
        qf1["Hivertaco 111-74 Bot'Vives"]
        qf2["Electrobot 117-109 Les C. Circuits"]
        qf3["Game Team 111-91 Labocesson 2"]
        qf4["Flybot 141-46 Les Vertaco"]
    end

    subgraph SF["Demi-finale"]
        sf1["Electrobot 125-120 Hivertaco"]
        sf2["Flybot 144-91 Game Team"]
    end

    gf["🏆 Champion : Flybot<br/>🥈 Finaliste : Electrobot"]

    r1 --> qf1
    r2 --> qf1
    r3 --> qf2
    r4 --> qf2
    r5 --> qf3
    r6 --> qf3
    r7 --> qf4
    r8 --> qf4

    qf1 --> sf1
    qf2 --> sf1
    qf3 --> sf2
    qf4 --> sf2

    sf1 --> gf
    sf2 --> gf

    classDef electrobot fill:#4a90d9,stroke:#2c5f8a,color:#fff
    classDef champion fill:#ffd700,stroke:#b8860b,color:#333
    class r4,qf2,sf1 electrobot
    class gf champion
{{< /mermaid >}}

**Grande finale** :

| Match | Electrobot | Flybot |
|-------|-----------|--------|
| 1 | **120** | 76 |
| 2 | 91 | **107** |
| 3 | 108 | **135** |

*Flybot remporte la finale 2-1. Petite finale : Game Team 115 - 76 Hivertaco (3ème place).*

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

Sept jeunes cette année :

* Adrien B
* Adrien R
* Aram
* Baya
* Henri
* Liam
* Sao Mai

## Liens

Le code: https://github.com/electrobot-fr/coupe2026

## Photos

![photo](/2026/IMG_1211.jpg)
![photo](/2026/IMG_1148.jpg)
![photo](/2026/IMG_1157.jpg)

## Vidéos

### Qualifications Île-de-France

Matchs de série :

Match 1 :

{{< youtube hjGd6FJU3dA >}}

Match 2 :

{{< youtube P6Cp5sbT1AU >}}

Match 3 :

{{< youtube YNLZHhDteAY >}}

Phase finale :

{{< youtube XmAA3FU3t94 >}}

### Coupe de France

Matchs de série :

Match 1 :

{{< youtube UgqUfEEmgME >}}

Match 2 :

{{< youtube SrCPZ5dl2Qo >}}

Match 3 :

{{< youtube yCME4PVGO6o >}}

Match 4 :

{{< youtube NYOSEbJOgas >}}

8e de finale :

{{< youtube lB1n2ay3e0U >}}

Quart de finale :

{{< youtube vkktXAG2Vvg >}}

Demi-finale :

{{< youtube y5YNs8ZUiD0 >}}

Finale :

{{< youtube tMCiCoOS0R0 >}}

Remise des prix :

{{< youtube GGjdGDKJo1w >}}
