---
description: >-
  🚀 These updates aim to enhance functionality and user experience across our
  systems!
cover: ../../.gitbook/assets/Frame 18470.png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🏆〡Trygon Hud V2.5

{% content-ref url="../../trygon/trygon-hud-v2.5/" %}
[trygon-hud-v2.5](../../trygon/trygon-hud-v2.5/)
{% endcontent-ref %}

***

<details>

<summary>v2.5.0</summary>

* :fuelpump: **Fuel:** `uz_core`fuel adjustment.

</details>

***

<details>

<summary>v2.4.0 <strong>uz_core</strong> dependency added &#x26; <strong>Stress whitelist</strong> issue fixed</summary>



</details>

***

<details>

<summary>v2.3.0 General bug fixes and code structure improvement</summary>



</details>

***

<details>

<summary>v2.2.0 </summary>

Changed files:

All files.

Features:&#x20;

* **Sounds:** Seat belt warning sounds in vehicles such as motorbikes have been switched off.
* **Engine Damage:** Added Engine Damage feature upon request. (Customize.lua > Display > VehicleEngineDamage)
* **Toggle Engine:** Start/Stop engine feature added. (Customize.lua > Display > ToggleEngine)
* **Other:** Edited `mp_f_freemode_01` for ESX.

</details>

***

<details>

<summary>v2.1.0</summary>



Changed files:

All files.

Features:&#x20;

* **StreetDisplay:** StreetDisplay problem, caused by the new speed indicator, has been fixed
* **ServerName:** The ability to turn off and on ServerName upon request has been added **(Customize.lua > Display > SpeedometerTextDisplay)**
* **ESX - Money;** The issue of displaying 0 as the initial login money in ESX has been resolved
* **Color;** The issue of the color menu remaining on the screen when the settings were closed during color adjustment has been resolved

</details>

***

<details>

<summary>v2.0.0 Health bugs fixed</summary>



</details>

***

<details>

<summary>v1.9.0 <strong>Customize.lua > SpeedometerText</strong> error fixed</summary>



</details>

***

<details>

<summary>v1.8.0</summary>



Changed files:

All files.

Features:&#x20;

* **Resmon:** Resmon (ms) values have been improved
* **Sounds:** Seatbelt sounds have been made a little softer
*   **Seatbelt;** Seatbelt system has been edited

    > _**qb-core:**_ smallresources dependency is now introduced for qb-core _**esx:**_ You need to do **esx\_cruisecontrol > config.lua** _**HudResource = 'TrygonHudV2.5'**_
*   **Resolutions:**&#x43;ompatibility has been brought for almost all resolutions, some of them are;

    > 4320p (8K): 7680x4320 2160p (4K): 3840x2160 1440p (2k): 2560x1440 1080p (HD): 1920x1080 720p (HD): 1280x720 480p (SD): 854x480 360p (SD): 640x360

</details>

***

<details>

<summary>v1.7.0</summary>

New Speedometer Added

<img src="../../.gitbook/assets/image (1).png" alt="" data-size="original">

</details>

***

<details>

<summary>v1.6.0 fixed seat belt warning sound and esx job issues</summary>



</details>

***

<details>

<summary>v1.5.0</summary>

Changed files:

All files.

Features:&#x20;

money & status positions edited\
5/6. fixed voice part of status\
radial style appearance slightly revised

</details>

***

<details>

<summary>v1.4.0</summary>

added warning sound when seat belt is not fastened - added bank money (fixed some minor bugs in esx)

```lua
SeatbeltAlertSound = false, -- true | false
```

</details>

***

<details>

<summary>v1.3.0</summary>

Changed Files:&#x20;

All files.

Features:

The first stable v2 version for v2.5 and v3 updates has been released. v2 is different from previous versions of v2 in that many features that are in v1 but not in v2 are in v2 and are much more optimized and completely coded from scratch. (new designs and features will be added in the next updates)

</details>

***

<details>

<summary>v1.2.0</summary>

Fixed errors in **ServerName** and added **VehHudText** for easier editing

```lua
Config.VehHudText = "uz-rp"
```

</details>

***

<details>

<summary>v1.1.0</summary>

Changed Files:&#x20;

All files.

Features:

* **Resolution improvements** (1366x768 - 2560x1440) have been applied to panel settings, reset, and all reset. 📏
* **PlayerData events** have been updated for players who were having issues with the HUD not refreshing. 🔄
* **Bug review:** All detected bugs have been reviewed, and we are in the process of fixing them. 🛠️
* **Support:** If you encounter any issues, please inform us by creating a ticket and tagging us. 📝
* **Team effort:** We are working to provide you with a better experience. 🌟

</details>

***
