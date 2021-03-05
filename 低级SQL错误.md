### 没有使用括号强调优先级
AND 优先级高于 OR
```sql
SELECT *
FROM table
WHERE a = 1 AND b = 2 OR c = 3
```
此段代码等价于  
```sql
SELECT *
FROM table
WHERE (a = 1 AND b = 2) OR c = 3
```

### FULL OUTER JOIN
FULL OUTER JOIN 通常是为了取全集，建议使用 UNION ALL 实现

### JOIN 字段类型不一致
常见错误发生在 BIGINT 和 STRING 类型关联时不做强制类型转换，最终会转换成 DOUBLE 类型关联，导致数据发散
