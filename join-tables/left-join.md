---
description: 用途：根據指定欄位合併 2 張資料表，並保留 LEFT JOIN 指令左邊資料表所有紀錄；若右邊資料表的指定欄位參照不到值，則返回 `NULL`
---

# LEFT JOIN

語法示範：

\(1\)　

```sql
SELECT P.USER_ID, P.DATETIME, P.ITEM, I.DAMAGE, I.PRICE
FROM PURCHASE_LOG P
LEFT JOIN ITEM_INFO I
    ON P.ITEM = I.ITEM;
```

![](../.gitbook/assets/image%20%2814%29.png)

