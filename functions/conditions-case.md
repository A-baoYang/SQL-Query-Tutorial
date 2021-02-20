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



\(2\)　也可在 CASE 判斷式中使用 `AND` `OR` 等邏輯運算符號

```sql
SELECT USER_ID, DATETIME, SCORE,
    CASE WHEN SCORE > 90000 THEN 'super-tier'
        WHEN SCORE > 50000 AND SCORE <= 90000 THEN 'front-tier'
        WHEN SCORE > 10000 AND SCORE <= 50000 THEN 'middle-tier'
        ELSE 'bottom-tier' END AS 'TIER'
FROM GAME_LOG
```

![](../.gitbook/assets/image%20%2831%29.png)

