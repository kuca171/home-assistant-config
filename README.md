# Kuca home-assistant-config

[![GitHub last commit](https://img.shields.io/github/last-commit/kuca171/home-assistant-config)](https://github.com/kuca171/home-assistant-config/commits/main)
[![HA Version](https://img.shields.io/badge/Running%20Home%20Asssistant-2024.1.2%20-green)](https://github.com/home-assistant/core/releases/tag/2024.1.2)
[![HA Community](https://img.shields.io/badge/HA%20community-forum-green)](https://community.home-assistant.io/u/kuca171/summary)

![alt tag](www/mydashboard.png)

Mé konfigurační soubory pro [Home Assistant](https://home-assistant.io/).

# Obsah

- [Použité zařízení](#použité-zařízení)
- [Doplňky](#doplňky)
- [Hacs integrace a témata](#hacs-integrace-a-témata)
- [Automatizace](#automatizace)
- [Další projekty](#další-projekty)

# Použité zařízení

<!-- start-table -->

<table>
  <thead>
    <tr>
      <th>Server</th>
      <th>Počet kusů </th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Raspberry Pi 4 Model B - 2GB RAM</td>
      <td>1</td>
      <td></td>
    </tr>
    <tr>
      <td>Verbatim Vx500 SSD 120GB</td>
      <td>1</td>
      <td></td>
    </tr>
  </tbody>
  <thead>
    <tr>
      <th>Světla</th> 
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Solight LED SMART WIFI RGB žárovka (wz432)</td>
      <td>3</td>
      <td><a href="https://github.com/rospogrigio/localtuya/">local tuya</a></td>
    </tr>
  </tbody>
  <thead>
    <tr>
      <th>Zásuvky</th> 
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Zásuvková lišta - LEDVANCE MULTI POWER SOCKET EU</td>
      <td>1</td>
      <td><a href="https://github.com/rospogrigio/localtuya/">local tuya</a></td>
    </tr>
  </tbody>
  <thead>
    <tr>
      <th>Senzory</th>
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ESP32 + BME280</td>
      <td>1</td>
      <td><a href="https://github.com/kuca171/FoxHomeIoT-ESP">FoxHomeIoT</a></td>
    </tr>
  </tbody>
  <thead>
    <tr>
      <th>Kamery</th>
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ESP32-cam</td>
      <td>1</td>
      <td>Postupná migrace -> FoxHomeIoT</td>
    </tr>
  </tbody>
  <thead>
    <tr>
      <th>Ostatní</th>
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Odvlhčovač vzduchu Concept OV2220 Perfect Air Smart</td>
      <td>1</td>
      <td><a href="https://github.com/rospogrigio/localtuya/">local tuya</a></td>
    </tr>
  </tbody>
</table>
<!-- end-table -->

# Doplňky

Použité doplňky [Supervisora](https://www.home-assistant.io/getting-started/):

<!-- start-table -->

<table>
  <thead>
    <tr>
      <th>Název doplňku</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/home-assistant/addons/tree/master/configurator">File editor</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/sabeechen/hassio-google-drive-backup">Home Assistant Google Drive Backup</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/hassio-addons/addon-grafana/">Grafana</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/hassio-addons/addon-influxdb/">InfluxDB</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/home-assistant/addons/tree/master/mariadb">MariaDB</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/home-assistant/addons/tree/master/mosquitto">Mosquitto broker</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/hassio-addons/addon-node-red">Node-RED</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/hassio-addons/addon-ssh">SSH & Web Terminal</a></td>
    </tr>
  </tbody>
</table>

<!-- end-table -->

# Hacs integrace a témata

Použité integrace a témata vzhledu z [HACS](https://hacs.xyz/):

<!-- start-table -->

<table>
  <thead>
    <tr>
      <th>Název</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/bruxy70/Garbage-Collection/">Garbage Collection</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/rospogrigio/localtuya/">local tuya</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/thecode/ha-rpi_gpio">Raspberry Pi GPIO custom integration</a></td>
    </tr>
  </tbody>
</table>

<!-- end-table -->

# Automatizace

- [Frontend: změna tématu](#frontend-změna-tématu) 
- [Notifikace odpadky - směs](#notifikace-odpadky---směs) 
- [Notifikace odpadky - papír](#notifikace-odpadky---papír)
- [Notifikace odpadky - plasty](#notifikace-odpadky---plasty)
- [Odvlhčovač - večerní vypnutí](#odvlhčovač---večerní-vypnutí)
- [Odvlhčovač - ranní spuštění](#odvlhčovač---ranní-spuštění)
- [Notifikace - odvlhčovač plná nádrž](#notifikace---odvlhčovač-plná-nádrž)

## Frontend: změna tématu 

Nastaví téma Home-Assistant.

```yaml
- id: change_thema
  alias: 'Frontend: změna tématu'
  trigger:
  - platform: state
    entity_id: input_select.theme
  - platform: homeassistant
    event: start
  action:
    service: frontend.set_theme
    data:
      name: '{{ states.input_select.theme.state }}'
```

## Notifikace odpadky - směs

Notifikace zaslaná na mobilní telefon o vyvezení popelnice.

```yaml
- id: '1666183776295'
  alias: Notifikace odpadky - směs
  description: Notifikace na vyvyzení popelnice
  trigger:
  - platform: time
    at: '20:00:00'
  condition:
  - condition: state
    entity_id: sensor.general_waste
    attribute: days
    state: 0
  action:
  - service: notify.mobile_app_redmi_note_8_pro
    data:
      title: Odpadky
      message: Směs
  mode: single
```

## Notifikace odpadky - papír

Notifikace zaslaná na mobilní telefon o vyvezení popelnice.

```yaml
- id: '1666183903283'
  alias: Notifikace odpadky - papír
  description: Notifikace na vyvezení popelnice
  trigger:
  - platform: time
    at: '20:00:00'
  condition:
  - condition: state
    entity_id: sensor.paper
    attribute: days
    state: 0
  action:
  - service: notify.mobile_app_redmi_note_8_pro
    data:
      title: Odpadky
      message: Papír
  mode: single
```

## Notifikace odpadky - plasty

Notifikace zaslaná na mobilní telefon o vyvezení popelnice.

```yaml
- id: '1666184054627'
  alias: Notifikace odpadky - plasty
  description: Notifikace na vyvezení popelnice
  trigger:
  - platform: time
    at: '20:00:00'
  condition:
  - condition: state
    entity_id: sensor.plastic
    attribute: days
    state: 0
  action:
  - service: notify.mobile_app_redmi_note_8_pro
    data:
      message: Plasty
      title: Odpadky
  mode: single
```

## Odvlhčovač - večerní vypnutí

Každodenní večerní vypnutí odvlhčovače.

```yaml
- id: '1676470917777'
  alias: Odvlhčovač - večerní vypnutí
  description: Vypnutí odvlhčovače každý večer
  trigger:
  - platform: time
    at: '20:00:00'
  condition: []
  action:
  - type: turn_off
    device_id: 1f286535060b37794deddf2cf4e02b47
    entity_id: switch.odvlhcovac_ov2220
    domain: switch
  mode: single
```

## Odvlhčovač - ranní spuštění

Každodenní ranní spuštění odvlhčovače.

```yaml
- id: '1676470978930'
  alias: Odvlhčovač - ranní spuštění
  description: Spuštění odvlhčovače každé ráno
  trigger:
  - platform: time
    at: 07:00:00
  condition: []
  action:
  - type: turn_on
    device_id: 1f286535060b37794deddf2cf4e02b47
    entity_id: switch.odvlhcovac_ov2220
    domain: switch
  mode: single
```

## Notifikace - odvlhčovač plná nádrž

Notifikace na plnou nádrž odvlhčovače.

```yaml
- id: '1676471091438'
  alias: Notifikace - odvlhčovač plná nádrž
  description: ''
  trigger:
  - platform: state
    entity_id:
    - binary_sensor.odvlhcovac_ov2220_nadrz
    attribute: raw_state
    from: 0
    to: 8
  condition: []
  action:
  - device_id: 6cf5d71fbaab6cc9446e7b7d8fe2750f
    domain: mobile_app
    type: notify
    message: Plná nádrž
    title: Odvlhčovač
  mode: single
```

# Další projekty

**- Jak integrovat Ledvance zásuvkovou lištu do Home Assistant -> https://github.com/kuca171/hassio-localtuya-device-configuration**

**- Jak integrovat Odvlhčovač vzduchu Concept OV2220 Perfect Air Smart do Home Assistant -> https://github.com/kuca171/hassio-localtuya-device-configuration**
