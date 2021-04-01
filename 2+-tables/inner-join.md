---
description: 用途：根據指定欄位合併 2 張資料表
---

# INNER JOIN

語法示範：

\(1\)　assign merge column with `ON`

```sql
SELECT P.USER_ID, P.DATETIME, P.ITEM, I.DAMAGE, I.PRICE
FROM PURCHASE_LOG P
INNER JOIN ITEM_INFO I
    ON P.ITEM = I.ITEM;
```

![](../.gitbook/assets/image%20%2823%29.png)



\(2\)　assign merge column with `USING`

> 只有當 2 張資料表合併參照的欄位名稱一致才能使用

```sql
SELECT USER_ID, DATETIME, ITEM, DAMAGE, PRICE
FROM PURCHASE_LOG
INNER JOIN ITEM_INFO
    USING(ITEM);
```

![](../.gitbook/assets/image%20%2827%29.png)



\(3\)　Self-join

> 同一張資料表，自己和自己合併

```sql
SELECT G1.USER_ID, G1.DATETIME AS TIMING, G1.SCORE, G2.DATETIME AS NEXT_TIMING, G2.SCORE
FROM GAME_LOG G1
INNER JOIN GAME_LOG G2
    ON G1.USER_ID = G2.USER_ID
    AND G1.DATETIME < G2.DATETIME;
```

![](../.gitbook/assets/image%20%2810%29.png)

