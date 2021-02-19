---
description: 用途：篩選資料表中欄位的特定值
---

# WHERE

語法示範：

\(1\)　選取符合項目之列：數值

```sql
SELECT * FROM GAME_LOG
WHERE SCORE > 90000;
```

![](../.gitbook/assets/image%20%283%29.png)



\(2\)　選取符合項目之列：文字

```sql
SELECT * FROM GAME_LOG
WHERE USER_ID LIKE '_w%';
```

![](../.gitbook/assets/image%20%284%29.png)



\(2\)　選取符合項目之列：list

```sql
SELECT * FROM GAME_LOG
WHERE ID IN (1, 3, 6, 8);
```

![](../.gitbook/assets/image%20%285%29.png)

