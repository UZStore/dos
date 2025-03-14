---
description: Player Details
---

# Player Details

<figure><img src="../../../.gitbook/assets/Group 37790.png" alt=""><figcaption><p>Player Details</p></figcaption></figure>

Follow the steps below to customize player details.

#### 1. Defining Player Details in Customize.lua

Edit the `PlayerDetails` section in the `Customize.lua` file to adjust how you want to display player details.

```lua
PlayerDetails = {
    icon = 'money.svg',  -- icon file path (resources/images/PlayerDetails)
    header = 'Money',    -- header (e.g., "Money")
    event = 'GetMoney'   -- event to be called (defined in server/function.lua)
}
```

In the code snippet above:

* **icon**: File path of an icon.
* **header**: The name of the displayed header.
* **event**: The event or function name to be called to fetch the relevant data.

{% hint style="info" %}
Note: The **GetMoney** function name must match the event name that we added to `PlayerDetails`.
{% endhint %}

#### 2. Defining the Function in server/function.lua

Add the relevant function to the `server/function.lua` file to define how to obtain player details on the server side.

```lua
GetMoney = function(Player, data)
    return '$ ' .. Player?.PlayerData?.money?.cash
end
```

In the code snippet above:

* The **GetMoney** function is written to return the player's cash. This function retrieves the **money** data from the `Player` object and displays it.
* The function takes two parameters: **Player** and **data**.
  * **Player**: Represents the player object and sends the player details.
  * **data**: Sends the content of **PlayerDetails** (icon, header, event).

#### 3. Test Your Customizations

After making all the adjustments, verify in-game that the information is displayed correctly. If you encounter any errors, review your **event** functions or **PlayerDetails** settings again.

