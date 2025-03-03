---
description: Please import the SQL below into your database
---

# SQL Installation

```sql
CREATE TABLE IF NOT EXISTS `uzstore_trygonhud` (
  `owner` varchar(65) DEFAULT NULL,
  `color` int(11) DEFAULT 2,
  `type` longtext DEFAULT 'mph',
  `customcolor` text DEFAULT '[]',
  `maptype` text DEFAULT 'rectangle',
  `stress` int(11) DEFAULT 0,
  UNIQUE KEY `owner` (`owner`)
) ENGINE=InnoDB DEFAULT CHARSET=UTF8MB4;
```



## **How to install SQL ?**

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}

