---
description: 用途：連接 2 段 SQL query ，根據相同欄位列出 2 張資料表紀錄
---

# -

語法示範：

\(1\)　UNION

> 會排除重複欄位中的值

```sql
SELECT USER_ID
FROM GAME_LOG
UNION
SELECT USER_ID
FROM PURCHASE_LOG;
```

