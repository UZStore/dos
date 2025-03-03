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

# 🚧Trygon Garage

{% content-ref url="../../trygon/trygon-garage/" %}
[trygon-garage](../../trygon/trygon-garage/)
{% endcontent-ref %}

***

<details>

<summary>v2.1.0</summary>

* added: Interact (qb-target, ox\_target, drawtext)
* new version controller
* Files Changed: `client.lua`, `Customize.lua`, `fxmanifest.lua`

</details>

***

<details>

<summary>v2.0.0</summary>



* **Language Integration**: Languages have been expanded in `uz_garage` to improve user interface experiences. (en, fr, es, de, tr)
* **Fuel Management**: Integrated fuel features in both `uz_garage`.
* **New Compatibility**: `uz_core` is now available, offering new functionalities.
* **Garage Open**: You can now open the garage menu even if you don't have a car in your garage.



🚀 These updates aim to enhance functionality and user experience across our systems!

</details>

***

<details>

<summary>v1.7.0 ESX issues have been resolved, and framework selection has been adjusted</summary>



</details>

***

<details>

<summary>v1.6.0 The code structure has been organized, optimized &#x26; version control has been added</summary>



</details>

***

<details>

<summary>v1.5.0 </summary>

Added 'ModificationSave' (optionally registers vehicle modifications when you put the vehicles in the garage)

```javascript
ModificationSave = true,
```

</details>

***

<details>

<summary>v1.4.0 Many garage locations have been added ready for use</summary>



</details>

***

<details>

<summary>v1.3.0</summary>

The notify message that will be sent when all vehicle spawn areas are full.

```lua
CarNotSpawnNotift = function()
    print('All designated locations are full.')
end,
```

</details>

***

<details>

<summary>v1.2.0 </summary>

If there is a vehicle at the spawn location, the vehicle will spawn at the next designated location. (there is no limit on the number of designated locations and you can add as many as you want)

```lua
VehSpawnPos = {
    [1] = vector4(127.67, 6590.31, 31.4, 267.53),
    [2] = vector4(132.97, 6585.3, 31.54, 273.22)
},
```

</details>

***

<details>

<summary>v1.1.0 Damage record</summary>



</details>
