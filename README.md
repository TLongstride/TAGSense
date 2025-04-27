# TAGSense

This repository gathers all the resources for the **TAGSense** (Zigbee ISO 15693 RFID reader).

## User Manual

The user manual for TAGSense is available in the following languages:

- **French**: [Mode d'emploi (French User Manual)](docs/fr/Mode_d_emploi.md)
- **English**: [User Manual (English)](docs/en/User_Manual.md)

## Repository Contents

- **User Manual**: User documentation for installation, configuration, and usage of TAGSense.
- **External Converter for Zigbee2MQTT**: External converter file for integrating TAGSense with Zigbee2MQTT ([Zigbee2MQTT/TAGSense.js](Zigbee2MQTT/TAGSense.js)).
- **Technical Resources**: Schematics, technical notes, configuration examples, etc.

## Technical Data

List of the tested tag:

- **RFID card**  
  *Reading distance: up to 12 cm*
- **Flexible RFID tag**  
  *Reading distance: up to 7 cm*
- **Blue key fob**  
  *Reading distance: upcomming soon*
- **50×50 mm chip**  
  *Reading distance: upcomming soon*

All ISO 15693 tags are compatible.

## Using the Zigbee2MQTT Converter

To integrate TAGSense with Zigbee2MQTT:

1. Copy the [`Zigbee2MQTT/TAGSense.js`](Zigbee2MQTT/TAGSense.js) file into the `external_converters` folder of your Zigbee2MQTT installation.
2. Restart Zigbee2MQTT.

For Zigbee2MQTT Home Assistant Addon:

1. Navigate to the `config/zigbee2mqtt` directory.
2. Create a folder named `external_converters` if it does not already exist.
3. Copy the `TAGSense.js` file into the `external_converters` folder.
4. Restart Zigbee2MQTT.

## 🛠️ Home Assistant Blueprint

Simplify the integration of TAGSense into your Home Assistant automations with this blueprint. It enables triggering specific actions based on RFID badge detection.

The blueprint is available in **French** :

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://github.com/TLongstride/TAGSense/blob/main/blueprints/fr/TAGSense.yaml)

The blueprint is available in **English** :

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https://github.com/TLongstride/TAGSense/blob/main/blueprints/en/TAGSense.yaml)

## Where to Buy

You can purchase TAGSense on [Tindie](https://www.tindie.com/products/38459/).

## Images

Find product and usage images in the [docs/images](docs/images) folder.

## Video

Watch the TAGSense reader in action on [YouTube](https://www.youtube.com/channel/UCya3AObZp-ZwquD5AgKnOvw).

## About

- **Manufacturer**: THED&Co
- **Description**: Zigbee-connected ISO 15693 RFID reader

## Useful Links

- [Zigbee2MQTT Documentation](https://www.zigbee2mqtt.io/)
- [ISO 15693 RFID Standard](https://en.wikipedia.org/wiki/ISO/IEC_15693)

---

For any questions or suggestions, feel free to open an issue or contact us at [contact.thedco@gmail.com](mailto:contact.thedco@gmail.com).

