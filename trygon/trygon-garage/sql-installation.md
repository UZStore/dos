---
description: Please import the SQL below into your database
---

# SQL Installation



{% hint style="info" %}
Please make sure you have installed the correct framework, otherwise the script may not work properly
{% endhint %}

{% tabs %}
{% tab title="QBCore" %}
```sql
CREATE TABLE IF NOT EXISTS `player_vehicles` (
    `id` int(11) NOT NULL AUTO_INCREMENT,
    `license` varchar(50) DEFAULT NULL,
    `citizenid` varchar(50) DEFAULT NULL,
    `vehicle` varchar(50) DEFAULT NULL,
    `hash` varchar(50) DEFAULT NULL,
    `mods` text CHARACTER SET utf8mb4 COLLATE utf8mb4_bin DEFAULT NULL,
    `plate` varchar(15) NOT NULL,
    `fakeplate` varchar(50) DEFAULT NULL,
    `garage` varchar(50) DEFAULT 'pillboxgarage',
    `fuel` int(11) DEFAULT 100,
    `engine` float DEFAULT 1000,
    `body` float DEFAULT 1000,
    `state` int(11) DEFAULT 1,
    `damage` text DEFAULT NULL,
    `depotprice` int(11) NOT NULL DEFAULT 0,
    `drivingdistance` int(50) DEFAULT NULL,
    `status` text DEFAULT NULL,
    PRIMARY KEY (`id`),
    KEY `plate` (`plate`),
    KEY `citizenid` (`citizenid`),
    KEY `license` (`license`)
) ENGINE=InnoDB AUTO_INCREMENT=1;
```
{% endtab %}

{% tab title="ESX" %}
```sql
CREATE TABLE IF NOT EXISTS `owned_vehicles` (
    `owner` varchar(60) COLLATE utf8mb4_unicode_ci NOT NULL,
    `plate` varchar(12) COLLATE utf8mb4_unicode_ci NOT NULL,
    `vehicle` longtext COLLATE utf8mb4_unicode_ci DEFAULT NULL,
    `type` varchar(20) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT 'car',
    `job` varchar(50) CHARACTER SET utf8 DEFAULT '',
    `stored` tinyint(1) NOT NULL DEFAULT 0,
    `state` int(11) DEFAULT 1,
    `damage` text COLLATE utf8mb4_unicode_ci DEFAULT NULL,
    PRIMARY KEY (`plate`),
    KEY `owner` (`owner`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci;
```
{% endtab %}
{% endtabs %}



## **How to install SQL ?**

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

