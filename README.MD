# ESPHome Configuration for SmartPlug T101_V1.1 (RTL8710BX)

This project provides the configuration and firmware for **ESPHome** to work with the **SmartPlug T101_V1.1**, which is based on the **RTL8710BX** chip. These smartplugs use Wi-Fi for communication and are compatible with platforms like **Home Assistant**.

## 🛠 Features

- **Wi-Fi Support**: Complete configuration for stable connectivity.
- **Control and Monitoring**:
  - Turn the plug on/off via Home Assistant.
  - Real-time power consumption monitoring.

## 📂 Project Structure

- `config.yaml`: Main configuration file for ESPHome tailored to the smartplug.
- `secrets.yaml`: File to store sensitive data such as Wi-Fi credentials (see the example file).

## 🔧 Flashing Details

### 🔑 Pin Connections
Pin functions can be found here:
[LibreTiny Documentation](https://docs.libretiny.eu/boards/generic-rtl8710bx-4mb-980k/#pin-functions)

#### Steps to Enter Download Mode:
1. Connect **GND** to the **GND of the UART controller**.
2. Keep the **3.3V** disconnected while keeping the other pins wired.
3. Connect **TX2** to **GND** (using a breadboard or similar setup).
4. Quickly connect the **3.3V**, then immediately reconnect **TX2** to the **RX** pin of the UART controller.

### 📸 Wiring Images

![Image 1](https://github.com/Romain-GUILLEMOT/SmartPlug-T101_V1.1-RTL8710BX-ESPHOME/blob/main/images/1.png?raw=true "Image 1")
![Image 2](https://github.com/Romain-GUILLEMOT/SmartPlug-T101_V1.1-RTL8710BX-ESPHOME/blob/main/images/2.png?raw=true "Image 2")
![Image 3](https://github.com/Romain-GUILLEMOT/SmartPlug-T101_V1.1-RTL8710BX-ESPHOME/blob/main/images/3.png?raw=true "Image 3")

### ⚙️ Recommended Software
Flashing only worked using **ITchiptool v4.7.0**. You can download this tool via the following link:
**[ITchiptool v4.7.0](https://github.com/libretiny-eu/ltchiptool/releases/tag/v4.7.0)**


### Help
If you need help, here are some links that were helpful during the process:

- [alonsoruibal](https://www.alonsoruibal.com/esphome-in-a-rtl8710bx-smart-plug/)
- [libratiny](https://docs.libretiny.eu/docs/platform/realtek-ambz/)
- [elektroda](https://www.elektroda.com/rtvforum/topic4032920.html)
- [bluemind](https://www.bluemind.org/converting-a-tuya-power-plug-to-esphome-device/)

---


# Configuration ESPHome pour SmartPlug T101_V1.1 (RTL8710BX)

Ce projet contient la configuration et le firmware **ESPHome** pour les prises connectées **SmartPlug T101_V1.1** basées sur la puce **RTL8710BX**. Ces smartplugs utilisent le Wi-Fi pour la communication et sont compatibles avec des plateformes comme **Home Assistant**.

## 🛠 Fonctionnalités

- **Support Wi-Fi** : Configuration complète pour une connexion stable.
- **Contrôle et suivi** :
  - Activation/Désactivation de la prise via MQTT ou Home Assistant.
  - Suivi de la consommation électrique en temps réel.

## 📂 Structure du projet

- `config.yaml` : Fichier principal contenant la configuration ESPHome pour le smartplug.
- `secrets.yaml` : Fichier pour stocker les informations sensibles comme les identifiants Wi-Fi (voir le fichier exemple).

## 🔧 Détails pour le flashage

### 🔑 Instructions de branchement
Les détails des fonctions des broches sont disponibles ici :
[Documentation LibreTiny](https://docs.libretiny.eu/boards/generic-rtl8710bx-4mb-980k/#pin-functions)

#### Procédure pour entrer en mode téléchargement :
1. Connectez le **GND** au **GND du contrôleur UART**.
2. Débranchez le **3.3V** tout en gardant la carte branchée sur les autres broches.
3. Connectez le **TX2** à **GND** (via une breadboard ou autre).
4. Branchez rapidement le **3.3V**, puis reconnectez immédiatement le **TX2** sur le port **RX** de la carte UART.

### 📸 Images de branchement

![Image 1](https://github.com/Romain-GUILLEMOT/SmartPlug-T101_V1.1-RTL8710BX-ESPHOME/blob/main/images/1.png?raw=true "Image 1")
![Image 2](https://github.com/Romain-GUILLEMOT/SmartPlug-T101_V1.1-RTL8710BX-ESPHOME/blob/main/images/2.png?raw=true "Image 2")
![Image 3](https://github.com/Romain-GUILLEMOT/SmartPlug-T101_V1.1-RTL8710BX-ESPHOME/blob/main/images/3.png?raw=true "Image 3")


### ⚙️ Logiciel recommandé
Le flash n'a fonctionné qu'avec **ITchiptool v4.7.0**. Vous pouvez télécharger cet outil via le lien suivant :
**[ITchiptool v4.7.0](https://github.com/libretiny-eu/ltchiptool/releases/tag/v4.7.0)**
 
### Help
Si vous avez besoin d’aide, voici quelques liens qui m’ont aidé durant le processus :

- [alonsoruibal](https://www.alonsoruibal.com/esphome-in-a-rtl8710bx-smart-plug/)
- [libratiny](https://docs.libretiny.eu/docs/platform/realtek-ambz/)
- [elektroda](https://www.elektroda.com/rtvforum/topic4032920.html)
- [bluemind](https://www.bluemind.org/converting-a-tuya-power-plug-to-esphome-device/)


#### This config is based on [this config](https://devices.esphome.io/devices/Digitaling-20A-Power-Monitor-RTL8710BX-t102-v1.1).