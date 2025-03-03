---
description: Please import the SQL below into your database
cover: ../../.gitbook/assets/webp-multicharacter.webp
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# SQL Installation

```sql
CREATE TABLE IF NOT EXISTS `uz_multichar` (
  `owner` varchar(65) DEFAULT NULL,
  `maxchar` int(11) DEFAULT 1,
  UNIQUE KEY `owner` (`owner`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci;

CREATE TABLE IF NOT EXISTS `uz_multichar_tebex` (
  `tebex` varchar(255) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COLLATE=utf8_general_ci;
```
