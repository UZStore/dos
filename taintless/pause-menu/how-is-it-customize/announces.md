---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Announces

<figure><img src="../../../.gitbook/assets/PROJECT ANNOUNCES (1).png" alt=""><figcaption><p>Announces</p></figcaption></figure>

### Announces Overview

Announcements are used to communicate important messages to players, such as server updates, events, or general announcements. The announce system can include text, headers, dates, and optionally images to make your messages more engaging.

#### 1. Structure of Announces in `Announces.json`

The announcements are defined in the `Announces.json` file. Each announcement includes several key elements:

```json
[
    {
        "text": "Lorem ipsum dolor sit amet consectetur. Penatibus ullamcorper dui suscipit fringilla dis magna. Et viverra tellus vitae id congue tellus lorem. Pharetra feugiat nunc facilisi vitae pellentesque integer. Hendrerit orci rutrum odio.",
        "date": "05.09.2024",
        "header": "Welcome to the server!",
        "photo": ""
    }
]
```

In the example above, each announce includes:

* **text**: The main content of the announcement.
* **date**: The date of the announcement, formatted as `dd.mm.yyyy`.
* **header**: A title for the announcement, used to grab the player's attention.
* **photo**: The photo of the person who made the announcement.

### 2. Adding New Announces

To add a new announce, use the command:

```sh
/addAnnounce Header Text
```

#### Command Customize:

{% code title="Customize.lua" %}
```lua
Command = {
    Permission = 'admin',
    Command = 'addAnnounce',
    Text = 'New Announce',
    Description = {
        {name='Header', help='Header'},
        {name='Text', help='Text'},
    }
}
```
{% endcode %}

* **Command**: The command required for the announce, such as `/addAnnounce`.
* **Permission**: The authorization level required to use the command (e.g., `admin`).
* **Text**: Description of the command.
* **Description**: Command syntax helper.
  * **Header**: The title of the announcement.
  * **Text**: The content of the announcement.

#### Adding Announcements Manually:

1. Open the `Announces.json` file.
2. Copy an existing announcement object.
3. Modify the `text`, `date`, `header` and `photo` fields as needed:

```json
{
    "text": "Join us for an exciting new event happening this weekend. There will be exclusive rewards!",
    "date": "10.10.2024",
    "header": "Weekend Event Announcement!",
    "photo": "https://i.imgur.com/3taJXrA.jpeg"
}
```

### 5. Testing Your Announces

After updating the `Announces.json` file, ensure that the changes are displayed correctly:

{% hint style="info" %}
Note: Announcements will be updated automatically without the need for any manual server reload
{% endhint %}

* **Verify the Output**:
  * Ensure the text displays correctly without being truncated.
  * Check that the photo, if included, loads properly.
  * Confirm that the date and header are formatted correctly.

### Summary

* **Edit the `Announces.json` file** to create or update announcements, or use the specified command to add a new announcement in-game.
* **Include text, date, header, and photo** to make your announcements effective. The photo is automatically set, ensuring each announcement is visually engaging.
* Test each announcement to ensure it displays correctly in-game.

Using these guidelines, you can create clear and effective announcements that keep your player community informed and engaged. :heart:
