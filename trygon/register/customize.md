# Customize

{% tabs %}
{% tab title="Customize.json" %}
{% code title="Customize.json" %}
```json
{
  "Lang": {
    "EntryHeader": "ENTRY",
    "Entry": "CREATE YOUR CHARACTER",
    "Subtitle": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam",
    "Info": "LOOK & INFO",
    "GenderHeader": "GENDER",
    "GenderSubtitle": "some text here",
    "RegisterHeader": "REGISTER",
    "RegisterSubtitle": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam",
    "FirstNameHeader": "FIRSTNAME",
    "FirstNameSubtitle": "some text here",
    "LastNameHeader": "LASTNAME",
    "LastNameSubtitle": "some text here",
    "HeightHeader": "HEIGHT",
    "HeightSubtitle": "some text here",
    "BirthdayHeader": "BIRTHDAY",
    "BirthdaySubtitle": "some text here",
    "RegisterConfirm": "REGISTER ",
    "RulesHeader": "RULES",
    "RulesSubtitle": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam"
  },
  "Nationality": "Nationality",
  "Social1": {
    "Link": "https://discord.gg/uzstore",
    "Image": "./img/discord.svg",
    "Name": "Discord",
    "Suptext": "some text here"
  },
  "Social2": {
    "Link": "https://www.youtube.com/@esckaybeden",
    "Image": "./img/youtube.svg",
    "Name": "Youtube",
    "Suptext": "follow"
  },
  "Rules": [
    {
      "Header": "RULE#1",
      "Text": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam"
    },
    {
      "Header": "RULE#2",
      "Text": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam"
    },
    {
      "Header": "RULE#3",
      "Text": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam"
    },
    {
      "Header": "RULE#3",
      "Text": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam"
    },
    {
      "Header": "RULE#3",
      "Text": "Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam"
    }
  ]
}
```
{% endcode %}
{% endtab %}

{% tab title="Customize.lua" %}


```lua
Customize = {
    Framework = "QBCore", -- QBCore | NewESX | ESX | OldQBCore (Write the framework you used as in the example)    
    Mysql = "oxmysql", -- oxmysql | ghmattimysql | mysql-async (Write the sql script you use as in the example)
    isSkipSpawnSelector = false, -- ignores the spawn selector screen and starts in last position
}
```
{% endtab %}
{% endtabs %}

