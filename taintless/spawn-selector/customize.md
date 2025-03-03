---
cover: ../../.gitbook/assets/Thumbnail - (youtube izleme yüzdesi daha fazla).webp
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

# Customize



{% hint style="info" %}
{% code title="export/Event" %}
```lua
exports["uz_SpawnSelector"]:OpenSpawnSelector(islastCoords)
TriggerClientEvent('uz_SpawnSelector:OpenSpawnSelector', islastCoords)
```
{% endcode %}
{% endhint %}

{% tabs %}
{% tab title="Customize.lua" %}
{% code title="Customize/Customize.lua" %}
```lua
Customize = {  
  UIColor = '#FBCA79',  -- The main color of the interface (in HEX format). You can change it to use different colors
  FontAwesomeIcon = false,  -- `true` for FontAwesome icons, `false` for custom images. - You can select FontAwesome icons from: https://fontawesome.com/search?ic=free
  ApartmentIcon = 'Apartments.png',  -- The image file/FontAwesome name used as the apartment icon.

  CustomUIFunction = function()
    -- hud display
  end,

  Locations = {
    ["legion"] = {
      icon = 'tree.png',
      subtext = 'Legion Square Subtext',
      coords = vector4(187.36, -849.91, 31.17, 21.17),
      label = "Legion Square",
    },
  
    ["policedp"] = {
      coords = vector4(407.93, -1115.05, 29.44, 81.82),
      subtext = "policedp",
      icon = "Satellite.png",
      label = "Police Department",
    },
  
  
    ["motel"] = {
      coords = vector4(327.56, -205.08, 53.08, 163.5),
      subtext = "Motels",
      icon = 'Apartments.png',
      label = "Motels",
    },


    ["fuel"] = {
      coords = vector4(173.12, 6632.54, 31.72, 185.54),
      subtext = "Paleto Bay Fuel Station",
      icon = 'FuelStation.png',
      label = "Fuel Station",
    },

    ["shop"] = {
      coords = vector4(-1501.33, 1519.84, 115.29, 167.96),
      subtext = "24/7 Shop",
      icon = 'Shops.png',
      label = "Leisure Shop",
    },

    ["hardware"] = {
      coords = vector4(54.22, -1738.72, 29.56, 57.36),
      subtext = "Hardware Store",
      icon = 'SuperMarket.png',
      label = "Super Market",
    },
  }
}


ApartmentsFunction = function(appaYeet)
  local configData = LoadResourceFile('qb-apartments', 'config.lua')
  local configFunc = load(configData)
  configFunc()    
  TriggerServerEvent("apartments:server:CreateApartment", appaYeet, Apartments.Locations[appaYeet].label, true)
end
```
{% endcode %}
{% endtab %}
{% endtabs %}

