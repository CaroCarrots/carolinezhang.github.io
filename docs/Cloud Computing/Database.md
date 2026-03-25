# What is a Database?
A collection of information organised so that it can easily be accessed and managed.
## Transaction

```SQL
BEGIN;

UPDATE accounts SET balance = balance - 100 WHERE id = A;
UPDATE accounts SET balance = balance + 100 WHERE id = B;

COMMIT;
```

 If something crashes after the first update
 - Without transaction -> money disappears
 - With transaction -> rollback -> nothing changes