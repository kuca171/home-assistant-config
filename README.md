# Kuca home-assistant-config

[![GitHub last commit](https://img.shields.io/github/last-commit/kuca171/home-assistant-config)](https://github.com/kuca171/home-assistant-config/commits/main)
[![HA Version](https://img.shields.io/badge/Running%20Home%20Asssistant-2024.9.2%20-green)](https://github.com/home-assistant/core/releases/tag/2024.9.2)
[![HA Community](https://img.shields.io/badge/HA%20community-forum-green)](https://community.home-assistant.io/u/kuca171/summary)

![alt tag](docs/img//mydashboard.png)

Mé konfigurační soubory pro [Home Assistant](https://home-assistant.io/).

# Obsah

- [Použité zařízení](#použité-zařízení)
- [Hacs integrace a témata](#hacs-integrace-a-témata)


# Použité zařízení

<!-- start-table -->

<table>
  <thead>
    <tr>
      <th>Server</th>
      <th>Počet kusů </th>
      <th>OS</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Raspberry Pi 4 Model B - 2GB RAM</td>
      <td>1</td>
      <td>Debian GNU/Linux 11 (bullseye)</td>
    </tr>
    <tr>
      <td>Verbatim Vx500 SSD 120GB</td>
      <td>1</td>
      <td></td>
    </tr>
    <tr>
      <td>Home Assistant SkyConnect</td>
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
      <td><a href="https://github.com/rospogrigio/localtuya/"><s>local tuya</s></a><br /><a href="https://esphome.io/">ESPHome</a></td>
    </tr>
    <tr>
      <td>LEDVANCE SMART+ CL A60 E27 Tunable white</td>
      <td>1</td>
      <td><a href="https://www.zigbee2mqtt.io/devices/4058075729001.html#ledvance-4058075729001">Zigbee2mqtt</a></td>
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
      <td><a href="https://github.com/rospogrigio/localtuya/"><s>local tuya</s></a><br /><a href="https://esphome.io/">ESPHome</a></td>
    </tr>
  </tbody>
  <thead>
    <tr>
      <th>ESP</th>
      <th>Počet kusů</th>
      <th>Použitá integrace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>ESP32 + BME280</td>
      <td>1</td>
      <td><a href="https://esphome.io/">ESPHome</a></td>
    </tr>
    <tr>
      <td>ESP32 (Bluetooth proxy)</td>
      <td>1</td>
      <td><a href="https://esphome.io/">ESPHome</a></td>
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
      <td><a href="https://github.com/rospogrigio/localtuya/"><s>local tuya</s></a><br /><a href="https://github.com/make-all/tuya-local">Tuya local</a></td>
    </tr>
    <tr>
      <td>Pračka Beko Beyond FWUE 87262 CSH4B0</td>
      <td>1</td>
      <td><a href="https://github.com/home-assistant-HomeWhiz/home-assistant-HomeWhiz">HomeWhiz</a></td>
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
      <td><a href="https://github.com/home-assistant-HomeWhiz/home-assistant-HomeWhiz">HomeWhiz</a></td>
    </tr>
    <tr>
      <td><a href="https://github.com/make-all/tuya-local">Tuya Local</a></td>
    </tr>
  </tbody>
</table>

<!-- end-table -->
