---
description: Please import the SQL below into your database
---

# SQL Installation



```sql
CREATE TABLE IF NOT EXISTS `es_playerlist` (
  `license` varchar(150) DEFAULT NULL,
  `name` varchar(50) DEFAULT NULL,
  `tasks` longtext DEFAULT NULL,
  `profile` longtext DEFAULT NULL,
  `level` varchar(50) DEFAULT NULL,
  `xp` int(50) DEFAULT NULL,
  `avatar` longtext DEFAULT NULL,
  `border` varchar(50) DEFAULT NULL,
  `color` varchar(50) DEFAULT NULL,
  `tac` longtext DEFAULT NULL,
  `rewards` longtext DEFAULT NULL,
  `earnings` int(50) DEFAULT NULL,
  `rank` longtext DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8;
```

## **How to install SQL ?**

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

