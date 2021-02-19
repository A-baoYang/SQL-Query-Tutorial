---
description: 用途：連接 2 段 SQL query ，根據相同欄位列出 2 張資料表紀錄；INTERSECT 只取 SELECT 欄位的紀錄有交集的部分
---

# INTERSECT

語法示範：

\(1\)　

```sql
SELECT USER_ID
FROM GAME_LOG
INTERSECT
SELECT USER_ID
FROM PURCHASE_LOG;
```

![](../.gitbook/assets/image%20%2833%29.png)

```sql
SELECT *
FROM GAME_LOG
INTERSECT
SELECT *
FROM PURCHASE_LOG;
```

![](../.gitbook/assets/image%20%2835%29.png)

