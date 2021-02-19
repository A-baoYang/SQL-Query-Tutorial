---
description: 用途：對分組後的資料列進行篩選
---

# GROUP BY with HAVING

語法示範：

\(1\)

```sql
SELECT USER_ID, SUM(SCORE) AS SCORE_SUM
FROM GAME_LOG
GROUP BY USER_ID
HAVING SCORE_SUM > 50000;
```

![](../.gitbook/assets/image%20%2817%29.png)



