# 📘 Manuel d’utilisation — TAGSense
Lecteur RFID Zigbee ISO15693  
by THED&Co

---

## 📦 Contenu du colis

- 1× Lecteur RFID TAGSense
- 1× Câble d’alimentation USB Type-C
- 1× Adaptateur secteur USB Type-A
- 1× Carte RFID (portée jusqu’à 12 cm)

---

## ⚙️ Spécifications techniques

- **Protocole** : Zigbee
- **Norme RFID supportée** : ISO15693
- **Portée de lecture** : 0-12 cm
- **Alimentation** : 5V via USB Type-C
- **Boîtier** : PLA
- **Compatibilité** : Zigbee2MQTT, Home Assistant (via Z2M)
- **Dimensions lxLxh** : 93.6 × 43.6 × 15.5 mm

---

## 🧱 Installation physique

1. Choisissez un emplacement adapté : installez le TAGSense dans un lieu dégagé, sec et à l’abri des interférences électromagnétiques.
2. Fixation : utilisez les trous traversants pour une fixation stable sur une surface plane.
3. Branchement : connectez l’alimentation. Une LED s’allume brièvement pour indiquer la mise sous tension.
4. Démarrage : attendez 5 à 10 secondes pour le démarrage complet du module.

---

## 🔗 Procédure d’appairage Zigbee

1. Téléchargez l’external converter depuis :  
   [github.com/TLongstride/THED-Co](https://github.com/TLongstride/THED-Co) → Dossier TAGSense
2. Placez le fichier `TAGSense.js` dans le dossier `/external_converters/` de votre configuration Zigbee2MQTT.
3. Redémarrez Zigbee2MQTT.
4. Activez l’inclusion Zigbee dans votre coordinateur.
5. Branchez le module : une LED clignote lentement indiquant qu’il est prêt à s’appairer.
6. Le module apparaît sous le nom **TAGSense** dans l’interface Zigbee2MQTT.

---

## 🏠 Intégration dans Home Assistant
Pour l’addon Zigbee2MQTT de Home Assistant :

1. Accédez au répertoire `config/zigbee2mqtt`.
2. Créez un dossier nommé `external_converters` s’il n’existe pas déjà.
3. Copiez le fichier `TAGSense.js` dans le dossier `external_converters`.
4. Redémarrez Zigbee2MQTT.

Une fois intégré via Zigbee2MQTT, deux entités sont automatiquement créées :

- `binary_sensor.tagsense_presence` : détecte la présence ou l’absence d’un badge/tag RFID.
- `sensor.tagsense_uid` : expose l’UID du badge RFID détecté.

Utilisez ces entités dans vos automatisations Home Assistant :

- Déclencher des scénarios d’arrivée/départ.
- Déverrouiller une porte ou désactiver une alarme.
- Envoyer des notifications personnalisées.

---

## 🛠️ Blueprint Home Assistant

Ce blueprint simplifie l’intégration du TAGSense dans vos automatisations Home Assistant. Il permet de déclencher des actions spécifiques en fonction de la détection d’un badge RFID.

#### Fonctionnalités :
- Détection de présence ou d’absence d’un badge.
- Exécution d’automatisations personnalisées basées sur l’UID du badge.

#### Importation du Blueprint :
1. Cliquez sur le bouton ci-dessous pour importer directement le blueprint dans votre instance Home Assistant.
2. Configurez les paramètres selon vos besoins.

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?external_url=https://raw.githubusercontent.com/TLongstride/THED-Co/blueprints/fr/tagsense_blueprint.yaml)

## ⚠️ Conseils de sécurité et bonnes pratiques

- Ne pas exposer le module à l’eau ou à une forte humidité.
- Ne pas démonter le module lorsqu’il est alimenté.
- Évitez toute présence d’éléments métalliques entre le badge et le capteur.

---

## 📞 Support & documentation

- 📧 contact.thedco@gmail.com
- 🔗 [github.com/TLongstride](https://github.com/TLongstride)

---

🇬🇧 **English version available**  
Looking for the manual in English? Visit the GitHub repository and switch to the `User_Manual.md` file.

---

Produit imaginé, conçu et fabriqué avec soin par **THED&Co** — France 🇫🇷