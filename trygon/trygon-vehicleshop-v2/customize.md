# Customize

{% code fullWidth="false" %}
```lua
Settings = {
    Framework = 'qb-core', -- Specify the framework you're using: esx / qb-core / old-esx
    Mysql = 'oxmysql', -- Specify the SQL script you're using: oxmysql / ghmattimysql / mysql-async
    FuelSystem = 'LegacyFuel', -- Fuel system: LegacyFuel / ox-fuel / nd-fuel / frfuel / cdn-fuel / hyon_gas_station / x-fuel

    vehicleShop = {
        [1] = {
            ServerName = "uz Roleplay designs your dream car", -- The name of the server

             -- Other Coords
            BuySpawn = vector4(-10.6716, -1096.76, 26.183, 100.5), -- The coordinates where the car can be bought
            PressButton = vector3(-56.89, -1097.18, 27.42), -- The coordinates where the button is pressed to access the shop
            
            -- Ped Settings
            peds = {
                model = 'cs_milton', -- Ped model
                position = vector3(-56.89, -1097.18, 26.42), -- Ped position
                heading = 32.25, -- Ped heading (rotation)
            },

            -- Test Drive
            TestDrive = vector4(-1616.63, -2990.03, 13.52, 240.22), -- The coordinates where the test drive begins
            TestDrivePrice = 50, -- The price of the test drive
            TestDriveTime = 10, -- The duration of the test drive
         
            -- Showroom 
            showroomSpawn = vector4(-73.5, -822.0, 284.8, 201.5), -- The coordinates where the cars are displayed in the showroom
             
            ShowCamera = { -- The camera settings for the showroom view
                 posX = -67.0,
                 posY = -824.5,
                 posZ = 285.5,
                 rotX = -9.0,
                 rotY = 0,
                 rotZ = 74.0,
                 fov = 45.00
            },
     
            -- Blips
            blips = { -- The blip settings for the shop on the minimap
                Position = vector3(-56.89, -1097.18, 27.42), -- Blip coordinate
                Label = "Gallery", -- Blip name
                Sprite = 326, -- Blip Sprite
                Display = 4, -- Blip Display
                Scale = 0.7, -- Blip Scale
                Color = 0 -- Blip Color
            },

            Categories = { -- The list of categories for the cars
               {  id = 'sports',             label = "Sports" }, 
               {  id = 'sedans',             label = "Sedans" }, 
               {  id = 'compacts',           label = "Compacts" }, 
               {  id = 'sportsclassics',     label = "S. Classics" }, 
               {  id = 'super',              label = "Super" }, 
               {  id = 'tuners',             label = "Tuners" }, 
               {  id = 'coupes',             label = "Coupes" }, 
               {  id = 'motorcycles',        label = "motor" }, 
               {  id = 'muscle',             label = "Muscle" }, 
               {  id = 'offroad',            label = "Off-Road" }, 
               {  id = 'suvs',               label = "SUVs" }, 
               {  id = 'vans',               label = "Vans" },
               {  id = 'dlc',                label = "DLC" }
            },

            Cars = {
                -- motorcycles
                { label = 'Ruffian',     price = 99999,  model = 'ruffian',       categories = 'motorcycles' },
                { label = 'Hakuchou',    price = 20000,  model = 'hakuchou',      categories = 'motorcycles' },
                { label = 'PCJ 600',     price = 10000,  model = 'pcj',           categories = 'motorcycles' },
                { label = 'Nemesis',     price = 12000,  model = 'nemesis',       categories = 'motorcycles' },
                { label = 'Sanchez',     price = 18000,  model = 'sanchez',       categories = 'motorcycles' },
            
                -- offroad
                { label = 'Dubsta',          price = 70000,  model = 'dubsta3',       categories = 'offroad' },
                { label = 'Dubsta 2',        price = 70000,  model = 'dubsta2',       categories = 'offroad' },
                { label = 'Brawler',         price = 40000,  model = 'brawler',       categories = 'offroad' },
                { label = 'Dubsta 6x6',      price = 70000,  model = 'dubsta3',       categories = 'offroad' },
                { label = 'Dune Buggy',      price = 30000,  model = 'dune',          categories = 'offroad' },
                { label = 'Rebel',           price = 35000,  model = 'rebel',         categories = 'offroad' },
                { label = 'Ramp Buggy',      price = 60000,  model = 'dune3',         categories = 'offroad' },
        
                -- sport
                { label = 'Sentinel',        price = 50000,  model = 'sentinel',      categories = 'sport' },
                { label = 'Carbonizzare',    price = 90000,  model = 'carbonizzare',  categories = 'sport' },
                { label = 'Jester',          price = 80000,  model = 'jester',        categories = 'sport' },
                { label = 'Feltzer',         price = 75000,  model = 'feltzer2',      categories = 'sport' },
                { label = 'Elegy RH8',       price = 90000,  model = 'elegy2',        categories = 'sport' },

                -- super
                { label = 'Adder',           price = 100000, model = 'adder',         categories = 'super' },
                { label = 'Entity XF',       price = 95000,  model = 'entityxf',      categories = 'super' },
                { label = 'Osiris',          price = 110000, model = 'osiris',        categories = 'super' },
                { label = 'T20',             price = 135000, model = 't20',           categories = 'super' },
                { label = 'Reaper',          price = 125000, model = 'reaper',        categories = 'super' },
                
                -- muscle
                { label = 'Blade',           price = 35000,  model = 'blade',         categories = 'muscle' },
                { label = 'Sabre Turbo',     price = 40000,  model = 'sabregt',       categories = 'muscle' },
                { label = 'Phoenix',         price = 45000,  model = 'phoenix',       categories = 'muscle' },
                { label = 'Vigero',          price = 30000,  model = 'vigero',        categories = 'muscle' },
                { label = 'Gauntlet',        price = 50000,  model = 'gauntlet',      categories = 'muscle' },

                -- compacts
                { label = 'Blista Compact',  price = 45000,  model = 'blista2',       categories = 'compacts' },
                { label = 'Issi',            price = 40000,  model = 'issi2',         categories = 'compacts' },
                { label = 'Brioso R/A',      price = 35000,  model = 'brioso',        categories = 'compacts' },
                { label = 'Panto',           price = 30000,  model = 'panto',         categories = 'compacts' },
                { label = 'Rhapsody',        price = 32000,  model = 'rhapsody',      categories = 'compacts' },

                -- sedans
                { label = 'Warrener',        price = 55000,  model = 'warrener',      categories = 'sedans' },
                { label = 'Schafter',        price = 60000,  model = 'schafter2',     categories = 'sedans' },
                { label = 'Tailgater',       price = 50000,  model = 'tailgater',     categories = 'sedans' },
                { label = 'Fugitive',        price = 45000,  model = 'fugitive',      categories = 'sedans' },
                { label = 'Asterope',        price = 40000,  model = 'asterope',      categories = 'sedans' },
            },
        },
        [2] = {
            ServerName = "uz Roleplay designs your dream boat", -- The name of the server

            -- Orther Coords
            BuySpawn = vector4(-793.292297, -1429.279175, -0.476929, 144.566910),
            PressButton = vector3(-720.6, -1327.0, 2.6),

            -- Ped Settings
            peds = {
                model = 'cs_milton', -- Ped model
                position= vector3(-720.61590576172, -1327.0679931641, 1.6), -- Ped position
                heading = 312.25, -- Ped heading (rotation)
            },

            -- Test Drive 
            TestDrive = vector4(-793.292297, -1429.279175, -0.476929, 144.566910),
            TestDrivePrice = 50,
            TestDriveTime = 15, 

            -- Showroom 
            showroomSpawn = vector4(-716.794, -1344.95, -0.5, 201.5),
            ShowCamera = {
                posX = -725.602, -- -725.602, -1358.61, 0.1185
                posY = -1358.61,
                posZ = 7.0,
                rotX = -16.0,
                rotY = 0,
                rotZ = -35.0,
                fov = 45.00
            },

            -- -- Blips
            blips = { -- The blip settings for the shop on the minimap
                Position = vector3(-720.61590576172, -1327.0679931641, 1.5962907075882), -- Blip coordinate
                Label = "Boat Gallery", -- Blip name
                Sprite = 326, -- Blip Sprite
                Display = 4, -- Blip Display
                Scale = 0.7, -- Blip Scale
                Color = 0 -- Blip Color
            },

            Categories = {
                { id = 'jets',          label = 'Jets'           },
                { id = 'helicopters',   label = 'Helicopter'     },
                { id = 'smallplanes',   label = 'Small P.'   },
                { id = 'cargoplanes',   label = 'Cargo P.'   },
                { id = 'military',      label = 'Military'       },
                { id = 'seaplanes',     label = 'Sea P.'     },
                { id = 'vipjets',       label = 'VIP Jets'       },
                { id = 'fighter',       label = 'Fighter'        },
            },


            Cars = {
               -- Motorboats
               { label = 'Dinghy',          price = 50000,      model = 'dinghy',         categories = 'motorboats' },
               { label = 'Speeder',         price = 60000,      model = 'speeder',        categories = 'motorboats' },
               { label = 'Marquis',         price = 70000,      model = 'marquis',        categories = 'motorboats' },
               { label = 'Toro',            price = 80000,      model = 'toro',           categories = 'motorboats' },
               { label = 'Jetmax',          price = 90000,      model = 'jetmax',         categories = 'motorboats' },

               -- Sailboats     
               { label = 'Squalo',          price = 200000,     model = 'squalo',          categories = 'sailboats' },
               { label = 'Suntrap',         price = 400000,     model = 'suntrap',         categories = 'sailboats' },
               { label = 'Dinghy2',         price = 100000,     model = 'dinghy2',         categories = 'sailboats' },
             
               -- Speedboats    
               { label = 'Speeder',         price = 60000,      model = 'speeder',         categories = 'speedboats' },
               { label = 'Seashark',        price = 80000,      model = 'seashark',        categories = 'speedboats' },
               { label = 'Jetmax',          price = 90000,      model = 'jetmax',          categories = 'speedboats' },
             
               -- Jet Ski   
               { label = 'Seashark',        price = 80000,      model = 'seashark',        categories = 'jetski' },
               { label = 'Speeder',         price = 60000,      model = 'speeder',         categories = 'jetski' },
               { label = 'Dinghy',          price = 50000,      model = 'dinghy',          categories = 'jetski' },
            },
        },
        [3] = {
            ServerName = "uz Roleplay designs your dream air", -- The name of the server
            -- Orther Coords
            BuySpawn = vector4(-724.73791503906, -1443.9154052734, 5.0005226135254, 142.22235107422),
            PressButton = vector3(-700.19, -1401.16, 6.5),

            -- Ped Settings
            peds = {
                model = 'cs_milton', -- Ped model
                position=  vector3(-700.19, -1401.16, 5.5), -- Ped position
                heading = 140.35, -- Ped heading (rotation)
            },
             
            -- Test Drive 
            TestDrive = vector4(-953.64, -3356.34, 13.94, 57.88),
            TestDrivePrice = 50,
            TestDriveTime = 10, 
 
             -- Showroom 
            showroomSpawn = vector4(-724.68, -1443.85, 5.0, 141.13),
            ShowCamera = {
                posX = -738.22,
                posY = -1442.64,
                posZ = 8.0,
                rotX = -10.0,
                rotY = 0.0,
                rotZ = -96.0,
                fov = 85.00
            },

            -- Blips
            blips = {
                Position = vector3(-700.09, -1401.23, 5.5),
                Label = "Air Shop",
                Sprite = 326,
                Display = 4,
                Scale = 0.5,
                Color = 4,
            },

            Cars = {
                -- Jets
                { label = 'Hydra',           price = 3000000,   model = 'hydra',          categories = 'jets' },
                { label = 'Lazer',           price = 2500000,   model = 'lazer',          categories = 'jets' },
                { label = 'Besra',           price = 2000000,   model = 'besra',          categories = 'jets' },
            
                -- Helicopters
                {  label = 'Buzzard',        price = 1500000,   model = 'buzzard',        categories = 'helicopters' },
                {  label = 'Savage',         price = 2000000,   model = 'savage',         categories = 'helicopters' },
                {  label = 'Cargobob',       price = 2500000,   model = 'cargobob2',      categories = 'helicopters' },
                {  label = 'Volatus',        price = 1800000,   model = 'volatus',        categories = 'helicopters' },
                {  label = 'Maverick',       price = 1200000,   model = 'maverick',       categories = 'helicopters' },
            
                -- Small Planes
                { label = 'Mammatus',        price = 800000,    model = 'mammatus',      categories = 'smallplanes' },
                { label = 'Dodo',            price = 900000,    model = 'dodo',          categories = 'smallplanes' },
                { label = 'Velum',           price = 1000000,   model = 'velum',         categories = 'smallplanes' },
                { label = 'Duster',          price = 600000,    model = 'duster',        categories = 'smallplanes' },
                
                -- Cargo Planes 
                { label = 'Titan',           price = 4000000,   model = 'titan',         categories = 'cargoplanes' },
                { label = 'Bombushka',       price = 5500000,   model = 'bombushka',     categories = 'cargoplanes' },
                { label = 'MILJET',          price = 6000000,   model = 'miljet',        categories = 'cargoplanes' },
                
                -- Military 
                { label = 'Buzzard Attack',  price = 2000000,   model = 'buzzard2',      categories = 'military' },
                { label = 'Savage',          price = 2200000,   model = 'savage',        categories = 'military' },
                
                -- Sea Planes   
                { label = 'Dodo',            price = 900000,    model = 'dodo',          categories = 'seaplanes' },
                { label = 'Seabreeze',       price = 1000000,   model = 'seabreeze',     categories = 'seaplanes' },
                { label = 'Tula',            price = 1500000,   model = 'tula',          categories = 'seaplanes' },
                { label = 'Duster',          price = 600000,    model = 'duster',        categories = 'seaplanes' },
                
                -- VIP Jets 
                { label = 'SuperVolito',     price = 15000000,   model = 'supervolito',   categories = 'vipjets' },
                { label = 'Nimbus',          price = 18000000,   model = 'nimbus',        categories = 'vipjets' },
                { label = 'Valkyrie',        price = 20000000,   model = 'valkyrie',      categories = 'vipjets' },
                
                -- Fighter  
                { label = 'Hydra',           price = 3000000,   model = 'hydra',         categories = 'fighter' },
                { label = 'Pyro',            price = 4000000,   model = 'pyro',          categories = 'fighter' },
            
            },
            

            Categories = {
                { id = 'motorboats',    label = 'Motorboats'     },
                { id = 'sailboats',     label = 'Sailboats'      },
                { id = 'speedboats',    label = 'Speedboats'     },
                { id = 'jetski',        label = 'Jet Ski'        },
            },
        },
    }
}

desing = {
    background = {
        boxShadow1 = '#62D9AC',
        boxShadow2 = '#28AA79',
    },

    header = {
        TextUP = {
            textColor = 'linear-gradient(104.75deg, #00FF94 2.61%, #24D88C 103.29%)',
            textShadow = '#00FF94',
        },
        TextDown = {
            textColor = '#AEFFDD',
            textShadow = 'rgba(174, 255, 221, 0.56)',
        }
    },    

    features = {
        mainColor = '#25F1A5',
        otherColor = 'rgba(174, 255, 221, 0.95)',
        boxColor = '#25F1A5',
        boxColor2 = '#25F1A5',

        iconShadow = 'rgba(99, 180, 222, 0.7)',
        boxShadow2 = '#25F1A5',
        boxShadow3 = 'rgba(37, 241, 165, 0.50)',
        boxShadow4 = 'rgba(37, 241, 165, 0.20)',
    },

    liverySelect = {
        mainColor = '#25F1A5',
        textColor = 'rgba(37, 241, 165, 0.91)',
        textColor2 = 'rgba(174, 255, 221, 0.95)',
        textShadow2 = 'rgba(37, 241, 165, 0.56)',
        textShadow3 = 'rgba(174, 255, 221, 0.56)',
        svgShadow1 = '#D7D7D7',
        svgShadow2 = '#D9D9D9',
        svgShadow3 = '#0B3324',
        svgShadow4 = '#60D9AC',
    },

    categoreis = {
        mainColor = '#00FF94',
        svgShadow1 = '#002918',
        textShadow = 'rgba(0, 255, 148, 0.45)',
    },

    testDrive = {
        mainColor = '#25F1A5',
        textColor = 'rgba(37, 241, 165, 0.91)',
    },

    exitButton = {
        backgroundColor = 'rgba(0, 255, 148, 0.06)',

        textColor = 'rgba(0, 255, 148, 0.82)',
        textColor2 = 'rgba(0, 255, 148, 0.91)',

        textShadow = 'rgba(0, 255, 148, 0.56)',
        textShadow2 = '#00FF94',
    },

    carsList = {
        scrollbackgroundColor = 'rgba(0, 255, 148, 0.91)',

        backgroundColor1 = '#00FF94',
        backgroundColor2 = '#002918',

        textColor = '#00FF94',
        textColor2 = '#AEFFDD',

        textShadow = 'rgba(0, 255, 148, 0.45)',
        textShadow2 = 'rgba(174, 255, 221, 0.56)',
    },

    money = {
        backgroundColor = '#00FF94',
        backgroundColor2 = '#5200A5',

        boxShadow1 = '#002918',
        boxShadow2 = '#00FF94',
        boxShadow3 = '#5200A5',
        boxShadow4 = '#200040',
        boxShadow5 = '#7F00FF',


        textColor = 'rgba(174, 255, 221, 0.95)',
        textColor2 = '#00FF94',
        textColor3 = 'rgba(174, 255, 221, 0.95)',
        textColor4 = '#5200A5',

        textShadow = 'rgba(174, 255, 221, 0.56)',
        textShadow2 = 'rgba(0, 255, 148, 0.45)',
        textShadow3 = 'rgba(174, 255, 221, 0.56)',
        textShadow4 = 'rgba(0, 255, 148, 0.56)',
        textShadow5 = 'rgba(82, 0, 165, 0.56)',
    },
}

CustomizeMarker = {
    Marker = true,
    MarkerDistance = 3.0, -- 20.0
    MarkerDrawTextDistance = 3.0,
    MarkerNuiOpenDistance = 2.0,

    ShopOpenDrawText = function(ShopPosition)
        local text = "~y~[E] -~g~ ~g~OPEN "        
        local onScreen, _x, _y = World3dToScreen2d(ShopPosition.x, ShopPosition.y, ShopPosition.z)
        local px, py, pz = table.unpack(GetGameplayCamCoords())
        SetTextScale(0.40, 0.40)
        SetTextFont(4)
        SetTextProportional(1)
        SetTextColour(255, 255, 255, 215)
        SetTextEntry("STRING")
        SetTextCentre(1)
        AddTextComponentString(text)
        DrawText(_x, _y)
        local factor = (string.len(text)) / 370
        DrawRect(_x, _y + 0.0125, 0.015 + factor, 0.03, 41, 11, 41, 90)
    end,

    ShopOpen = function()
        if IsControlJustPressed(0, 38) then
            return true
        end
    end
}

SetCarkeys = function(Plate)
    -- Your Carkey Events
    TriggerEvent("vehiclekeys:client:SetOwner", Plate)
end

DisplayHud = function(truefalse)
    if truefalse then
        -- exports['uz_TrygonHud']:SetHudVisibility(true)  -- Hud Export
    else

        -- exports['uz_TrygonHud']:SetHudVisibility(false) --  Hud Export
    end
end


randomCharacter = function(length)
    local res = ""
    for i = 1, length do
        res = res .. string.char(math.random(97, 122))
    end
    return res
end

randomNumber = function(length)
    local res = ""
    for i = 1, length do
        res = res .. string.char(math.random(48, 57))
    end
    return res
end

Plate = function()
    return string.upper(randomNumber(2) .. randomCharacter(3) .. randomNumber(3))
end

SendMessage = function(message, isError, part, source)
    if part == "client" then
        if Settings.Framework == "esx" or  Settings.Framework == "old-esx" then
            TriggerEvent("esx:showNotification", message)
        else
            TriggerEvent("QBCore:Notify", message, isError)
        end
    elseif part == "server" then
        if Settings.Framework == "esx" or  Settings.Framework == "old-esx" then
            TriggerClientEvent("esx:showNotification", source, message)
        else
            TriggerClientEvent('QBCore:Notify', source, message, isError)
        end
    end
end
  
GetFramework = function()
    local Get = nil
    if Settings.Framework == "old-esx" then
        while Get == nil do
            TriggerEvent('esx:getSharedObject', function(Set) Get = Set end)
            Citizen.Wait(0)
        end
    end
    if Settings.Framework == "esx" then
        Get = exports['es_extended']:getSharedObject()
    end
    if Settings.Framework == "qb-core" then
        Get = exports["qb-core"]:GetCoreObject()
    end
    return Get
end
  
ExecuteSql = function(query)
    local IsBusy = true
    local result = nil
    if Settings.Mysql == "oxmysql" then
        if MySQL == nil then
            exports.oxmysql:execute(query, function(data) 
                result = data 
                IsBusy = false 
            end)
        else
            MySQL.query(query, {}, function(data) 
                result = data 
                IsBusy = false 
            end)
        end
    elseif Settings.Mysql == "ghmattimysql" then
        exports.ghmattimysql:execute(query, {}, function(data) 
            result = data 
            IsBusy = false 
        end)
    elseif Settings.Mysql == "mysql-async" then
        MySQL.Async.fetchAll(query, {}, function(data) 
            result = data 
            IsBusy = false 
        end)
    end
    while IsBusy do
        Citizen.Wait(0)
    end
    return result
end
```
{% endcode %}
