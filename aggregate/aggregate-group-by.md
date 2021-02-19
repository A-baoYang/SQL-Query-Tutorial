---
description: 用途：對分組資料個別進行總和運算
---

# Aggregate: GROUP BY

語法示範：

\(1\)　`SUM()`

```sql
SELECT SUM(SCORE) AS SCORE_SUM
FROM GAME_LOG;
```

![](../.gitbook/assets/image%20%2831%29.png)

```sql
SELECT USER_ID, SUM(SCORE) AS SCORE_SUM
FROM GAME_LOG
GROUP BY USER_ID;
```

![](../.gitbook/assets/image%20%2833%29.png)



\(2\)　`AVG()`

```sql
SELECT USER_ID, AVG(SCORE) AS SCORE_AVG
FROM GAME_LOG
GROUP BY USER_ID;
```

![](../.gitbook/assets/image%20%285%29.png)



\(3\)　`MAX()`

```sql
SELECT USER_ID, MAX(SCORE) AS SCORE_MAX
FROM GAME_LOG
GROUP BY USER_ID;
```

![](../.gitbook/assets/image%20%2815%29.png)



\(4\)　`MIN()`

```sql
SELECT USER_ID, MIN(SCORE) AS SCORE_MIN
FROM GAME_LOG
GROUP BY USER_ID;
```

![](../.gitbook/assets/image%20%2821%29.png)



