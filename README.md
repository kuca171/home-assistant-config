# Kuca home-assistant-config

[![GitHub last commit](https://img.shields.io/github/last-commit/kuca171/home-assistant-config)](https://github.com/kuca171/home-assistant-config/commits/main)
[![HA Version](https://img.shields.io/badge/Running%20Home%20Asssistant-2022.5.3%20-green)](https://github.com/home-assistant/core/releases/tag/2022.5.3)
[![HA Community](https://img.shields.io/badge/HA%20community-forum-green)](https://community.home-assistant.io/u/kuca171/summary)

Mé konfigurační soubory pro [Home Assistant](https://home-assistant.io/).

### Do budoucna plánuji

- [x] Přechod z [auto backup](https://github.com/jcwillox/hass-auto-backup) na Home Assistant Google Drive Backup
- [x] Přidání dalších žárovek
- [x] Migrace z SD na SSD disk
- [ ] Automatické hydroponické pěstování koriandru (rozpracováno - připravuji repozitář s projektem)  
- [ ] Přidání LED pásků (rozpracováno -> Wemos d1 mini) 
- [ ] Přidání zásuvek
- [ ] Solární venkovní meteostanice (rozpracováno -> Wemos d1 mini + BME280)

# Obsah

- [Použité zařízení](#použité-zařízení)
- [Doplňky](#doplňky)
- [Hacs integrace a témata](#hacs-integrace-a-témata)
- [Automatizace](#automatizace)

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
      <td><s>Samsung EVO Plus microSDXC 64GB MB-MC64HA/EU</s></td>
      <td><s>1</s></td>
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
      <th>Senzory</th>
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ESP32 + BME280</td>
      <td>1</td>
      <td><a href="https://github.com/esphome/esphome">ESPhome</a></td>
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
      <td><a href="https://github.com/esphome/esphome">ESPhome</a></td>
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
      <td><a href="https://github.com/esphome/esphome">ESPhome</a></td>
    </tr>
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
      <td><s><a href="https://github.com/hassio-addons/addon-phpmyadmin">phpMyAdmin</a></s></td>
    </tr>
    <tr>
      <td><a href="https://github.com/hassio-addons/addon-ssh">SSH & Web Terminal</a></td>
    </tr>
    <tr>
      <td><s><a href="https://github.com/hassio-addons/addon-vscode/">Studio Code Server</a></s></td>
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
      <td><s><a href="https://github.com/jcwillox/hass-auto-backup">Auto backup</a></s></td>
    </tr>
    <tr>
      <td><a href="https://github.com/bruxy70/Garbage-Collection/">Garbage Collection</a></td>
    </tr>
    <tr>
      <td><s><a href="https://github.com/basnijholt/lovelace-ios-themes">iOS Themes</a></s></td>
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

- ~~[Automatická záloha](#automatická-záloha) (1 automatizace)~~ 
- [Fronted - vzhled](#fronted---vzhled) (~~3 automatizace~~ 1 automatizace)

## ~~Automatická záloha~~

~~Použité rozšíření z HACS - [Auto backup](https://github.com/jcwillox/hass-auto-backup).~~

~~Automatická záloha probíhá každou středu ve 2:00.~~

## Fronted - vzhled 

Pro nastavení témat z HACS. 

### Frontend: změna tématu 2

Nastaví téma Home-Assistant.

*používá:*
- [input_select.theme](https://github.com/kuca171/home-assistant-config/blob/master/include/inputs/input_selects.yaml)

### ~~Frontend: tmavý mód~~

~~Přepne se téma Home Assistant na tmavý mód při západu slunce a ve 20h.~~

~~*používá:*~~
~~- [input_boolean.dark_mode](https://github.com/kuca171/home-assistant-config/blob/master/include/input_booleans.yaml)~~

   
### ~~Frontend: světlý mód~~

~~Přepne se téma Home Assistant na světlý mód při východu slunce a v 6h.~~

~~*používá:*~~
- ~~[input_boolean.dark_mode](https://github.com/kuca171/home-assistant-config/blob/master/include/input_booleans.yaml)~~

### ~~Frontend: změna tématu~~

~~Nastaví téma Home-Assistant.~~

~~*používá:*~~
- ~~[input_boolean.dark_mode](https://github.com/kuca171/home-assistant-config/blob/master/include/input_booleans.yaml)~~
- ~~[input_boolean.theme_alternative](https://github.com/kuca171/home-assistant-config/blob/master/include/input_booleans.yaml)~~
- ~~[input_select.theme](https://github.com/kuca171/home-assistant-config/blob/master/include/input_selects.yaml)~~
