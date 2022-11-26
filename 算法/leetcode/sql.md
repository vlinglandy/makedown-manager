批量删除

```sql
DELETE FROM demo_order WHERE name IN ( SELECT name FROM
(SELECT name FROM demo_order WHERE name LIKE '%name%')t
)
```
