# Tuya Home Assistant Integration

<p align="center">
    <img src="https://images.tuyacn.com/app/hass/ha_tuya.png" width="70%">
</p>

This repo is the official home assistant integration for [Tuya Open API](https://developer.tuya.com/en/docs/cloud/?_source=github), maintained by the Tuya Developer Team.

## Supported Device Types

The following Home Assistant device types are currently supported.

- Light: Supports major graffiti wifi light devices
- Switch: Supports wifi switch devices

## Workflow

<img src="./imgs/hass_diagram1.png" width="60%"/>

<img src="https://images.tuyacn.com/app/hass/workflow.png" width="35%" />

## Sequence Diagram

<img src="https://images.tuyacn.com/app/hass/hass_diagram2.png" width="60%" />

## Installation

### 1. Home Assistant Installation
Refer to the [Home Assistant Installation](https://www.home-assistant.io/installation/) documentation to install **Home Assistant Core**.

### 2. tuya-home-assistant Installation
tuya-home-assistant support two ways to install
1. Home Assistant Custom Components Install
2. Install by [HACS](https://hacs.xyz/)

#### 2.1 Home Assistant Custom Components Install
Download tuya-home-assistant from github, unzip, copy to HomeAssistant configuration directory, e.g. ~/.homeassistant

<img src="https://images.tuyacn.com/smart/hass/hass_integrations_1.png" height="300" />

#### 2.2 Install by HACS
1. [HACS Install](https://hacs.xyz/docs/installation/installation/)
2. [HACS Initial Configuration](https://hacs.xyz/docs/configuration/basic)
3. HACS -> Integrations -> ... -> Custom repositories 
<img src="./imgs/hacs_install_custom.png" height="250" />
4. Input tuya-home-assistant github https url and select Integration in Category, click "Add"
<img src="https://images.tuyacn.com/app/hass/custom_repos.png" width="70%" />
5. Click "INSTALL"
<img src="./imgs/hacs_tuya_install.png" height="200"/>

#### 2.3 Restart Home Assistant

Configuration -> Server Controls -> RESTART

#### 2.4 Activate tuya-home-assistant

Configuration -> Integrations -> ADD INTEGRATION -> Tuya Integration

<img src="./imgs/hacs_tuya_set_up.png" height="200"/>

### 3. Enter your Tuya credential

Please get the Tuya credential info by following the **Configure Cloud Development Project** part in [Tuya IoT Platform Configuration Guide](https://github.com/tuya/tuya-android-iot-app-sdk-sample/blob/activator_tool/Tuya_IoT_Platform_Configuration_Guide.md).

<img src="./imgs/hacs_tuya_credential.png" height="300"/>

## Start
Refer to the **Home Assistant Core** tutorial for the startup process and run
**hass**

## Develop plugins, contribute code
Refer to [Contributing.md](./contributing.md)

## Issue feedback
You can give feedback on issues you encounter via **Github Issue** or via [**Ticket**](https://service.console.tuya.com)

## LICENSE
For more information, please refer to the [LICENSE](LICENSE) file
