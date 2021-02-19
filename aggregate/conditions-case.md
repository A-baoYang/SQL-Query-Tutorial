---
description: 用途： 根據不同條件將欄位內的值做分類，另存一欄
---

# Conditions: CASE

語法示範：

\(1\)　

```sql
SELECT USER_ID, DATETIME, SCORE,
    CASE WHEN SCORE > 50000 THEN 'front-tier'
        WHEN SCORE > 10000 THEN 'middle-tier'
        ELSE 'bottom-tier' END AS 'TIER'
FROM GAME_LOG
```

![](../.gitbook/assets/image%20%286%29.png)



