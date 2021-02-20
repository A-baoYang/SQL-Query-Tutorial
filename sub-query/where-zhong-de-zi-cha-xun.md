---
description: 用途：透過另一段 SQL query 進行 `WHERE` 指令篩選
---

# WHERE 中的子查詢

語法示範：

```sql
SELECT *
FROM PURCHASE_LOG
WHERE ITEM IN
(
    SELECT ITEM
    FROM ITEM_INFO
    WHERE DAMAGE > 30
);
```

![](../.gitbook/assets/image%20%2835%29.png)

