---
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

# Changelog



<details>

<summary>v1.6.5</summary>

🤿 Core Update:

* **codem-appearance Integration:** Updated the [`uz_core`](../../information/uzcore.md) system to support **codem-appearance** for managing player character appearance.



**Changelog**:

* **DefaultSpawn and LastLocation Functions Added:** Issues with directing players to the default spawn point for those not using the spawn selector have been resolved.

- **Removed Previous Version Check:** The previous version check mechanism has been removed. It has been replaced with the new version checking system.



**Date:** 08.09.2024

</details>

***

<details>

<summary>v1.6.0</summary>

🤿 Core Update:

* **Unified Script Compatibility**: With [`uz_core`](../../information/uzcore.md), all uz scripts are now seamlessly compatible with your swerver.
* **Multi-language Support**: Newly added languages include English (en), French (fr), Spanish (es), German (de), and Turkish (tr).



**Changelog**:

* **Framework Customization**: Automatically detect the framework with `detectFramework()`. Supports QBCore, ESX.
* **SQL Integration**: Choose between `oxmysql`, `ghmattimysql`, `mysql-async`, or let the system auto-select with `nil`.
* **Local Settings**: Available locales are now en, fr, es, de, tr.
* **Inventory Systems**: Automatically detect inventory type with `detectInventory()`
* **Appearance Modules**: Detect skin management system with `detectApparance()`

</details>

***

<details>

<summary>v1<em>.5.0 -</em> <strong>Logout</strong> and <strong>setchar</strong> commands have been added</summary>

**Files Changed**:

* All Files
* Customize.lua

**Update**:

* ✈️ **Logout:** Allows the player to log out from the character.
* 📊 **Setchar:** Allows you to change the max character slots.

**Changelog:**

{% code title="🤿 Customize.lua" %}
```lua
Command = {
    ['logout'] = {
        Permission = 'admin',
        Command = 'logout',
        Text = 'Logout (Admin Only)',
        Description = {}
    },
    ['setchar'] = {
        Permission = 'admin',
        Command = 'logout',
        Text = 'Set Character Slots',
        Description = {
            {name='Owner', help='CitizenID or License'},
            {name='Slot', help='New Max Slot'}
        }
    }
}
```
{% endcode %}

&#x20;

</details>

***

<details>

<summary>v1<em>.4.0</em></summary>

**Files Changed**:

* All Files
* Customize.lua

**Update**:

* 🛠️ **CustomUIFunction:** Now added! This feature lets you disable the display of your HUD script if needed.
* 🧵 **SkinSql:** Added to ensure compatibility with clothing scripts that we don't currently support.
* 🖼️ **Custom Image:** You can now change the photos in character selection from the resources/img folder.
* 🗃️ **Fixes:** We've reorganized the code structure (spawn and create) and added a skip create ped option to prevent issues in case of SQL corruption.

</details>

***

<details>

<summary>v1.3.0 </summary>

**Files Changed**:

* All Files
* Customize.lua

Update:

* 👗 Compatibility for **tgiann-clothing** has been added

</details>

***

<details>

<summary>v1.2.0 </summary>

**Files Changed**:

* All Files
* Customize.lua

Update:

* 👗 **Fix**: Issues with illenium-appearance have been resolved

</details>

***

<details>

<summary>v1.1.0</summary>

**Files Changed**:

* All Files
* Customize.lua

Update:

* 🏠 **Fix**: The new character creation errors and **joaat** error for those not using **qb-apartments** have been fixed&#x20;

</details>
