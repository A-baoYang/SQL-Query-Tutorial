---
description: 用途：連接 2 段 SQL query ，根據相同欄位列出 2 張資料表紀錄；EXCEPT 則會排除 SELECT 欄位的紀錄有交集的部分
---

# EXCEPT

語法示範：

\(1\)　

```sql
SELECT USER_ID
FROM GAME_LOG
EXCEPT
SELECT USER_ID
FROM PURCHASE_LOG;
```

![](../.gitbook/assets/image%20%2832%29.png)

