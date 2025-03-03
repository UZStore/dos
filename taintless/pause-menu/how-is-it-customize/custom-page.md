# Custom Page



<figure><img src="../../../.gitbook/assets/Frame 1000005713.png" alt=""><figcaption><p>Custom Page</p></figcaption></figure>

### Custom Pages Configuration

#### 1. Defining Custom Pages in Customize.lua

You can define custom pages by editing the `CustomPage` section in the `Customize.lua` file.

```lua
CustomPage = {  -- event (client side)
    { color = '#FBCA79', text = 'GAME SHOP',   background = 'GameShop.png',   event = '' },
    { color = '#00f37a', text = 'Vip Cars',    background = 'VipCarShop.png', event = '' },
    { color = '#77CDCC', text = 'Weapon Shop', background = 'WeaponShop.png', event = '' },
}
```

In the code snippet above:

* **color**: Defines the text color for the button.
* **text**: The label displayed on the button (e.g., **GAME SHOP**, **VIP Cars**, **Weapon Shop**).
* **background**: The background image for the button (resources/images/CustomPage).
* **event**: Event to be triggered when the button is clicked (currently left empty; you can define a client-side event here).

#### 2. Adding Events for Custom Pages

To make these buttons interactive, you need to add a client-side event. For example, if you want the **GAME SHOP** button to open the game shop interface, you should define an event in your client-side script and then add the event name to the **event** field.

Here's an example of defining a client-side event:

```lua
RegisterNetEvent('OpenGameShop', function()
    -- Code to open the game shop interface
    print('Game Shop opened')
end)
```

You would then update the `CustomPage` entry like this:

```lua
CustomPage = {
    { color = '#FBCA79', text = 'GAME SHOP', background = 'GameShop.png', event = 'OpenGameShop' },
    -- Other entries remain unchanged
}
```

{% hint style="info" %}
Note: Remember, event names must be the same.
{% endhint %}

#### 3. Customizing Button Appearance

* **Button Color**: The color attribute allows you to define how each button looks, allowing you to differentiate each custom page visually. Make sure the colors fit well with your overall design for better user experience.
* **Background Image**: The background image can be customized to visually represent the purpose of the button. For instance, using an image that represents in-game items for the **Game Shop**.

#### 4. Testing Your Custom Pages

After making changes, ensure to test each button in the game to verify that the correct event is triggered and the visuals are displayed as expected. This step is crucial to ensure that the user experience is smooth and there are no issues with accessing in-game features. :heart:
