---
description: 用途：根據指定欄位合併 2 張資料表，並保留 2 張資料表所有紀錄；若雙邊有任一資料表的指定欄位參照不到值，則返回 `NULL`
---

# FULL JOIN

語法示範：

\(1\)　

```sql
SELECT P.USER_ID, P.DATETIME, P.ITEM, I.DAMAGE, I.PRICE
FROM PURCHASE_LOG P
FULL JOIN ITEM_INFO I
    ON P.ITEM = I.ITEM;
```

