# Customize

{% tabs %}
{% tab title="Customize.lua" %}
```lua
Customize = {
    Locale = "en", -- en, fr, es, de, tr

    PlayerAvatarToken = "", -- https://discord.com/developers/applications // discord avatar
    DefaultAvatar = "./img/player.png",

    CommandANDKey = {
        command = "tdaily",
        key = "F5"
    },
    Time = 86400,   -- 3.600: 1 minutes - 86400: 24h

    ImagePathEnabled = true,-- When set to true, it will fetch the images from your inventory script

    Command = {
        Permission = 'admin',
        Command = 'addvip',
        Text = 'Add Vip Daily Reward',
        Description = {
            {name='Owner', help='ID'}
        }
    }
}

Customize.Gifts = {
    {
        day = "1",
        itemimg = "phone.png",
        itemname = "phone",
        amount = 2,
    },
    {
        day = "2",
        itemimg = "moneybag.png",
        itemname = "moneybag",
        amount = 1,
    },
    {
        day = "3",
        itemimg = "markedbills.png",
        itemname = "markedbills",
        amount = 1,
    },
    {
        day = "4",
        itemimg = "rolex.png",
        itemname = "rolex",
        amount = 2,
    },
    {
        day = "5",
        itemimg = "coffee.png",
        itemname = "coffee",
        amount = 1,
    },
}

Customize.GiftsPre = {
    {
        day = "1",
        itemimg = "itemhat.png",
        itemname = "hat",
        claimedpre = false, 
        amount = 1,
    },
    {
        day = "2",
        itemimg = "cash.svg",
        itemname = "200$",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "3",
        itemimg = "cash.svg",
        itemname = "700$",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "4",
        itemimg = "gloves.svg",
        itemname = "gloves",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "5",
        itemimg = "gold.svg",
        itemname = "gold",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "6",
        itemimg = "hat.svg",
        itemname = "hat",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "7",
        itemimg = "imagering.svg",
        itemname = "earring",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "8",
        itemimg = "jacket.svg",
        itemname = "jacket",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "9",
        itemimg = "mask.svg",
        itemname = "mask",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "10",
        itemimg = "neck.svg",
        itemname = "neck",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "11",
        itemimg = "pizza.svg",
        itemname = "pizza",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "12",
        itemimg = "shirt.svg",
        itemname = "shirt",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "13",
        itemimg = "sponge.svg",
        itemname = "sponge",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "14",
        itemimg = "sunglas.svg",
        itemname = "sun glasses",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "15",
        itemimg = "west.svg",
        itemname = "west",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "16",
        itemimg = "bag.svg",
        itemname = "bag",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "17",
        itemimg = "cash.svg",
        itemname = "1200$",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "18",
        itemimg = "cash.svg",
        itemname = "1700$",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "19",
        itemimg = "cash.svg",
        itemname = "2000$",
        claimedpre = false,
        amount = 1,
    },
    {
        day = "20",
        itemimg = "cash.svg",
        itemname = "2500$",
        claimedpre = false,
        amount = 1,
    },
}
```
{% endtab %}
{% endtabs %}

