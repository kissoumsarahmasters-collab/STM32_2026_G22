STM32 Projects – G22

Ce dépôt contient plusieurs projets réalisés avec la carte STM32 dans le cadre des travaux pratiques et du bureau d’étude.
## Projets réalisés: 
1. Ultrasonic sensor project (STM32 + Grove LCD)
   - Ultrasonic_LCD_Grove.zip
   - Rapport_Ultrason_Kissoum_Benmerieme.pdf
2. DHT11 Temperature & Humidity sensor (STM32 + Grove LCD)
   - Rapport_DHT11_Kissoum_Benmerieme.pdf
   - DHT11.zip
 3. Ruche connectée (STM32 + LoRa + Capteurs)

Ce projet a pour objectif de réaliser une ruche connectée capable de mesurer plusieurs paramètres physiques et d’envoyer les données à distance grâce à la communication LoRa.

### Capteurs utilisés
- Capteur de température et d’humidité (SHT31)
- Capteur de poids avec cellule de charge + HX711
- Capteur de présence PIR
- Afficheur LCD Grove RGB

### Fonctionnement
Le STM32 lit les données des capteurs :
- Température
- Humidité
- Poids de la ruche
- Détection de mouvement

Les données sont ensuite :
- Affichées sur l’écran LCD
- Envoyées par communication LoRa sous forme de trame
- Reçues par un autre module LoRa (récepteur)

### Communication LoRa
La communication entre les deux cartes STM32 se fait à l’aide de modules LoRa en utilisant des commandes AT.
Les trames sont envoyées en UART du STM32 vers le module LoRa, puis transmises par radio et reçues par un second module LoRa.

### Fichiers du projet
- RUCHE_TX.zip : Code de la carte émettrice (capteurs + envoi LoRa)
- RUCHE_RX.zip : Code de la carte réceptrice (réception LoRa + affichage)
- Rapport_BE_Kissoum_Benmerieme.pdf : Rapport complet du projet
- Diaporama_Ruche_Connectee : Présentation du projet

### Objectif pédagogique
Ce projet permet de mettre en œuvre :
- La programmation sur STM32
- La communication UART
- La communication radio LoRa
- L’acquisition de capteurs
- L’affichage sur écran LCD
- L’analyse de trames série avec oscilloscope (PicoScope)
