# Customize

{% tabs %}
{% tab title="Customize.lua" %}
```lua
Customize = {
    Framework = "QBCore", -- QBCore | ESX | NewESX | OldQBCore (Write the framework you used as in the example)
    Mysql = "oxmysql", -- oxmysql | ghmattimysql | mysql-async (Write the sql script you use as in the example)
    UIColor = "#58F1F3", -- Default ui color (just enter the color in hex!)
    VariableUIColor = true, -- ui color determines whether all ui will change color when color is set

    RepairPrice = 250,
    CustomFunction = function(Vehicle, Porps)
        --activated after the vehicle modification has been changed
    end,

    JobErrorNotify = function()
        print("you don't have this job")
    end,

    OpenCustoms = function()
        DisplayRadar(false) 
        --exports['uz_TrygonHud']:SetHudVisibility(false)
    end,

    CloseCustoms = function()
        DisplayRadar(true)
        --exports['uz_TrygonHud']:SetHudVisibility(true)
    end,

    Lang = {
        HeaderName = 'UZ',
        HeaderStore = 'CUSTOMS',
        Subtitle = 'designs your dream car',
        Max = 'MAX',
        Livery = 'Livery',
        RGBSelect = 'RGB SELECT',
        Buy = 'BUY',
        Lvl = 'lvl',
        Exit = 'Exit',
        Mechanic = 'Mechanic',
        ESC = 'ESC',
    },
}
```
{% endtab %}

{% tab title="RGB/Color " %}
```lua
CustomizeRGBColor = {
    ['Primary'] = true,
    ['Secondary'] = true,
    ['Xenon'] = true,
    ['Neon'] = true,
}

CustomizeColor = {
    {Label = "Chrome", ID = 120},
    {Label = "Black", ID = 0},
    {Label = "Carbon Black",  ID = 147},
    {Label = "Graphite",  ID = 1},
    {Label = "Anhracite Black",  ID = 11},
    {Label = "Black Steel",  ID = 2},
    {Label = "Dark Steel",  ID = 3},
    {Label = "Silver",  ID = 4},
    {Label = "Bluish Silver",  ID = 5},
    {Label = "Rolled Steel",  ID = 6},
    {Label = "Shadow Silver",  ID = 7},
    {Label = "Stone Silver",  ID = 8},
    {Label = "Midnight Silver",  ID = 9},
    {Label = "Cast Iron Silver",  ID = 10},
    {Label = "Red",  ID = 27},
    {Label = "Torino Red",  ID = 28},
    {Label = "Formula Red",  ID = 29},
    {Label = "Lava Red",  ID = 150},
    {Label = "Blaze Red",  ID = 30},
    {Label = "Grace Red",  ID = 31},
    {Label = "Garnet Red",  ID = 32},
    {Label = "Sunset Red",  ID = 33},
    {Label = "Cabernet Red",  ID = 34},
    {Label = "Wine Red",  ID = 143},
    {Label = "Candy Red",  ID = 35},
    {Label = "Hot Pink",  ID = 135},
    {Label = "Pfsiter Pink",  ID = 137},
    {Label = "Salmon Pink",  ID = 136},
    {Label = "Sunrise Orange",  ID = 36},
    {Label = "Orange",  ID = 38},
    {Label = "Bright Orange",  ID = 138},
    {Label = "Gold",  ID = 99},
    {Label = "Bronze",  ID = 90},
    {Label = "Yellow",  ID = 88},
    {Label = "Race Yellow",  ID = 89},
    {Label = "Dew Yellow",  ID = 91},
    {Label = "Dark Green",  ID = 49},
    {Label = "Racing Green",  ID = 50},
    {Label = "Sea Green",  ID = 51},
    {Label = "Olive Green",  ID = 52},
    {Label = "Bright Green",  ID = 53},
    {Label = "Gasoline Green",  ID = 54},
    {Label = "Lime Green",  ID = 92},
    {Label = "Midnight Blue",  ID = 141},
    {Label = "Galaxy Blue",  ID = 61},
    {Label = "Dark Blue",  ID = 62},
    {Label = "Saxon Blue",  ID = 63},
    {Label = "Blue",  ID = 64},
    {Label = "Mariner Blue", ID = 65},
    {Label = "Harbor Blue", ID = 66},
    {Label = "Diamond Blue", ID = 67},
    {Label = "Surf Blue", ID = 68},
    {Label = "Nautical Blue", ID = 69},
    {Label = "Racing Blue", ID = 73},
    {Label = "Ultra Blue", ID = 70},
    {Label = "Light Blue", ID = 74},
    {Label = "Chocolate Brown", ID = 96},
    {Label = "Bison Brown", ID = 101},
    {Label = "Creeen Brown", ID = 95},
    {Label = "Feltzer Brown", ID = 94},
    {Label = "Maple Brown", ID = 97},
    {Label = "Beechwood Brown", ID = 103},
    {Label = "Sienna Brown", ID = 104},
    {Label = "Saddle Brown", ID = 98},
    {Label = "Moss Brown", ID = 100},
    {Label = "Woodbeech Brown", ID = 102},
    {Label = "Straw Brown", ID = 99},
    {Label = "Sandy Brown", ID = 105},
    {Label = "Bleached Brown", ID = 106},
    {Label = "Schafter Purple", ID = 71},
    {Label = "Spinnaker Purple", ID = 72},
    {Label = "Midnight Purple", ID = 142},
    {Label = "Bright Purple", ID = 145},
    {Label = "Cream Purple", ID = 107},
    {Label = "Frost White", ID = 112},

    -- Matte
    {Label = "Black", ID = 12},
    {Label = "Gray", ID = 13},
    {Label = "Light Gray", ID = 14},
    {Label = "Ice White", ID = 131},
    {Label = "Blue", ID = 83},
    {Label = "Dark Blue", ID = 82},
    {Label = "Midnight Blue", ID = 84},
    {Label = "Midnight Purple", ID = 149},
    {Label = "Schafter Purple", ID = 148},
    {Label = "Red", ID = 39},
    {Label = "Dark Red", ID = 40},
    {Label = "Orange", ID = 41},
    {Label = "Yellow", ID = 42},
    {Label = "Lime Green", ID = 55},
    {Label = "Green", ID = 128},
    {Label = "Forest Green", ID = 151},
    {Label = "Foliage Green", ID = 155},
    {Label = "Olive Darb", ID = 152},
    {Label = "Dark Earth", ID = 153},
    {Label = "Desert Tan", ID = 154},
    
    -- Metals
    {Label = "Brushed Steel", ID = 117},
    {Label = "Brushed Black Steel", ID = 118},
    {Label = "Brushed Aluminum", ID = 119},
    {Label = "Pure Gold", ID = 158},
    {Label = "Brushed Gold", ID = 159},
}
```
{% endtab %}

{% tab title="Customs" %}
```lua
Customs = {
    {
        BlipPos = vector3(-74.97, -819.23, 325.56),             -- Represents NPC and Blip location
        BlipLabel = "Test Customs",                             -- Specifies the name to appear on the map
        BlipSprite = 643,                                       -- (https://docs.fivem.net/docs/game-references/blips/#blips)
        BlipDisplay = 4,                                        -- (https://docs.fivem.net/natives/?_0x9029B2F3DA924928)
        BlipScale = 0.8,                                        -- Sets icon size
        BlipColour = 18,                                        -- (https://docs.fivem.net/docs/game-references/blips/#blip-colors)
        BlipDisplay = true,                                  
        VehOpenCustoms = {                                      -- Location where the car will be picked up from the Customs
            [1] = vector3(-74.97, -819.23, 325.56),
        },
        Jobs = {'all'}
    },
    {
        BlipPos = vector3(318.44, -232.77, 53.37),              -- Represents NPC and Blip location
        BlipLabel = "Customs",                                  -- Specifies the name to appear on the map
        BlipSprite = 643,                                       -- (https://docs.fivem.net/docs/game-references/blips/#blips)
        BlipDisplay = 4,                                        -- (https://docs.fivem.net/natives/?_0x9029B2F3DA924928)
        BlipScale = 0.8,                                        -- Sets icon size
        BlipColour = 18,                                        -- (https://docs.fivem.net/docs/game-references/blips/#blip-colors)
        BlipDisplay = true,                                  
        VehOpenCustoms = {                                      -- Location where the car will be picked up from the Customs
            [1] = vector3(326.07, -241.48, 53.92),
            [2] = vector3(318.63, -232.05, 53.96),
            [3] = vector3(327.83, -212.17, 53.54),
        },
        Jobs = {'all'}
    },
}
```
{% endtab %}
{% endtabs %}

