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

![](../.gitbook/assets/image%20%2813%29.png)



\(2\)　選取符合項目之列：文字

```sql
SELECT * FROM GAME_LOG
WHERE USER_ID LIKE '_w%';
```

![](../.gitbook/assets/image%20%289%29.png)

```sql
SELECT * FROM GAME_LOG
WHERE USER_ID NOT LIKE '_w%';
```

![](../.gitbook/assets/image%20%2838%29.png)

\(3\)　選取符合項目之列：list

```sql
SELECT * FROM GAME_LOG
WHERE ID IN (1, 3, 6, 8);
```

![](../.gitbook/assets/image%20%2840%29.png)



\(4\)　選取符合項目之列：不等於符號 `<>`

```sql
SELECT * FROM GAME_LOG
WHERE USER_ID <> 'iwoehfieowe1232';
```

![](../.gitbook/assets/image%20%2837%29.png)



\(5\)　選取符合項目之列：空值 `NULL`

```sql
SELECT * FROM GAME_LOG
WHERE SCORE IS NULL;
```

![](../.gitbook/assets/image%20%2820%29.png)

```sql
SELECT * FROM GAME_LOG
WHERE SCORE IS NOT NULL;
```

![](../.gitbook/assets/image%20%287%29.png)

