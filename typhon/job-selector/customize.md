# Customize

{% tabs %}
{% tab title="Customize.lua" %}
```lua
Customize = {
    Framework = "QBCore", -- QBCore | ESX (Write the framework you used as in the example)    

    SetJobNotify = function(Header, Text)
        -- (client side only)
    end,

    Lang = {
        ['Draw3DText'] = '[E] Job Selector',                        -- client
        ['servername'] = "LABOR",                                   -- ui
        ['exchange'] = "EXCHANGE",                                  -- ui
        ['title'] = "Get your dream job and make lots of money!",   -- ui
        ['currentwork'] = "Currrent work",                          -- ui
        ['salary'] = "Salary",                                      -- ui
        ['closemenu'] = "Close menu"                                -- ui
    },

    JobSelector = {
        {
            Pos = vector3(-269.27, -955.52, 31.22),                 -- Represents NPC and Blip location
            NpcHash = "a_m_m_tranvest_01",                             -- (https://docs.fivem.net/docs/game-references/ped-models/)
            NpcHeading = 206.84,                                    -- Represents the npc's view direction
            Blip = "Job Selector",                                  -- Specifies the name to appear on the map
            BlipSprite = 357,                                       -- (https://docs.fivem.net/docs/game-references/blips/#blips)
            BlipDisplay = 4,                                        -- (https://docs.fivem.net/natives/?_0x9029B2F3DA924928)
            BlipScale = 0.5,                                        -- Sets icon size
            BlipColour = 18,                                        -- (https://docs.fivem.net/docs/game-references/blips/#blip-colors)
        },
        {
            Pos = vector3(160.31, -769.84, 259.75),                 -- Represents NPC and Blip location
            NpcHash = "a_m_y_business_01",                             -- (https://docs.fivem.net/docs/game-references/ped-models/)
            NpcHeading = 330.13,                                    -- Represents the npc's view direction
            Blip = "Job Selector",                                  -- Specifies the name to appear on the map
            BlipSprite = 357,                                       -- (https://docs.fivem.net/docs/game-references/blips/#blips)
            BlipDisplay = 4,                                        -- (https://docs.fivem.net/natives/?_0x9029B2F3DA924928)
            BlipScale = 0.5,                                        -- Sets icon size
            BlipColour = 18,                                        -- (https://docs.fivem.net/docs/game-references/blips/#blip-colors)
        },
    },

    Jobs = {
        {
            JobHeader = 'Taxi Driver',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 50,
            Image = '../images/taxi.svg',
            job = 'taxi'
          },
          {
            JobHeader = 'Bus Driver',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 75,
            Image = '../images/bus.svg',
            job = 'buss'
          },
          {
            JobHeader = 'Tow truck driver',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 120,
            Image = '../images/towtruck.svg',
            job = 'tow'
          },
          {
            JobHeader = 'Farmer',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 150,
            Image = '../images/farmer.svg',
            job = 'Farmers'
          },
          {
            JobHeader = 'Garbage driver',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 150,
            Image = '../images/garbage.svg',
            job = 'garbage'
          },
          {
            JobHeader = 'Trucker',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 95,
            Image = '../images/trucker.svg',
            job = 'trucker'
          },
          {
            JobHeader = 'Postman',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 150,
            Image = '../images/postman.svg',
            job = 'postman'
          },
          {
            JobHeader = 'Wood Cutting',
            JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
            Price = 270,
            Image = '../images/wood.svg',
            job = 'wood'
          }
    }
}
```
{% endtab %}

{% tab title="Jobs" %}
{% code title="Customize.lua" %}
```lua
Jobs = {
  {
    JobHeader = 'Taxi Driver',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 50,
    Image = '../images/taxi.svg',
    job = 'taxi'
  },
  {
    JobHeader = 'Bus Driver',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 75,
    Image = '../images/bus.svg',
    job = 'buss'
  },
  {
    JobHeader = 'Tow truck driver',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 120,
    Image = '../images/towtruck.svg',
    job = 'tow'
  },
  {
    JobHeader = 'Farmer',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 150,
    Image = '../images/farmer.svg',
    job = 'Farmers'
  },
  {
    JobHeader = 'Garbage driver',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 150,
    Image = '../images/garbage.svg',
    job = 'garbage'
  },
  {
    JobHeader = 'Trucker',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 95,
    Image = '../images/trucker.svg',
    job = 'trucker'
  },
  {
    JobHeader = 'Postman',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 150,
    Image = '../images/postman.svg',
    job = 'postman'
  },
  {
    JobHeader = 'Wood Cutting',
    JobSubtext = 'There should be a description in a couple of lines, so that the user understands what this work will give them. There should be a description in a couple of lines',
    Price = 270,
    Image = '../images/wood.svg',
    job = 'wood'
  }
}
```
{% endcode %}
{% endtab %}
{% endtabs %}

