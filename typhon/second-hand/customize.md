# Customize

{% tabs %}
{% tab title="Shared.lua" %}
```lua
Config.Framework = 'QBCore'  -- QBCore or ESX
Config.SQL = "ghmattimysql" -- "oxmysql" or "mysql-async" or "ghmattimysql"

Config.Locale = "en" -- tr

Config.UseTarget = false
Config.TargetExport = "qb-target"

Config.PlayerAvatarToken = "OTg3ODA5NTQwMTk4MjY5MDI5.GM9Lg2.v7Q8-WYO9VpEK7-oGXwert2_EDkg2kefNb_SlY"
Config.DefaultAvatar = "./assets/img/profil.png"


Config.Cam = {
    NuiCarViewSpawnPosition = vector4(-37.26872, -1054.309, -43.37314, 32.1),
    NuiCarViewCameraPosition = {
        posX = -41.36324,
        posY = -1052.294,
        posZ = -43.01,
        rotX = -15.0,
        rotY = 0.0,
        rotZ = 252.063,
        fov = 85.00
    },
}

Config.SpawnVehicle = vector4(697.12, 234.94, 92.76, 140.02)

Config.Location = {
    ['keys'] = 'E',
    ['label'] = 'Second Hand Vehicle Dealer',
    ['coords'] = vector4(688.74, 238.58, 93.48, 144.27),
    ['ped'] = 'mp_m_shopkeep_01',
    ['scenario'] = 'WORLD_HUMAN_STAND_MOBILE',
    ['radius'] = 1.5,
    ['targetIcon'] = 'fas fa-car',
    ['targetLabel'] = 'Open Second Hand Vehicle Dealer',
    ['showblip'] = true,
    ['blipsprite'] = 227,
    ['blipscale'] = 0.6,
    ['blipcolor'] = 0,
}

Config.SalesArea = {
    ['keys'] = 'E',
    ['label'] = 'Second Hand Vehicle Dealer',
    ['coords'] = vector4(700.33, 228.1, 92.58, 239.36),
    Size   = {x = 1.5, y = 1.5, z = 1.0},
    Color  = {r = 50, g = 200, b = 50},
    DrawDistance = 10,
    Type   = 1

}
```
{% endtab %}
{% endtabs %}

