---
description: 用途： `WHERE` 指令中的邏輯關聯
---

# AND / OR

語法示範：

\(1\)　AND

```sql
SELECT * FROM GAME_LOG
WHERE SCORE > 90000 
    AND USER_ID LIKE '_w%';
```

![](../.gitbook/assets/image%20%2816%29.png)



\(2\)　OR

```sql
SELECT * FROM GAME_LOG
WHERE SCORE > 60000 
    AND (USER_ID LIKE '_w%' OR ID IN (1, 3, 4, 8, 10));
```

![](../.gitbook/assets/image%20%2828%29.png)



