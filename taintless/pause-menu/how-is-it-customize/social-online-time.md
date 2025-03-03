# Social/Online/Time

<figure><img src="../../../.gitbook/assets/Group 37792 (1).png" alt=""><figcaption><p>Social/Online/Time</p></figcaption></figure>

Follow the steps below to customize social/online/time.

#### 1. Configuring Social Media Links and Server Settings

In `Customize.lua`, you can also configure social media links and server settings:

```lua
Use24HourFormat = false,  -- true: 24-hour format, false: 12-hour format
ServerMaxOnline = 1200,   -- Maximum number of players that can be online

Socials = {  -- min: 0 - max: 3
    { icon = 'youtube.svg', link = 'https://www.youtube.com/@UZStoree' },
    { icon = 'discord.svg', link = 'https://discord.gg/uzstore' },
    { icon = 'store.svg', link = 'https://uzstore.tebex.io/' }
}
```

In the code snippet above:

* **Use24HourFormat**: Specifies whether to use a 24-hour or 12-hour clock format.
* **ServerMaxOnline**: Defines the maximum number of players that can be online at the same time.
* **Socials**: Allows you to add social media icons and links (minimum of 0 and maximum of 3).
  * **icon**: File path of an icon (resources/images/Socials).
  * **link**: The link you want to be opened.

#### 2. Test Your Customizations

After making all the adjustments, verify in-game that the information is displayed correctly. :heart:
