---
layout: default
title: SQL Games - SQL Island
---


## [SQL Island](https://sql-island.informatik.uni-kl.de/)

After the survived plane crash, you will be stuck on SQL Island for the time being. 
By making progress in the game, you will find a way to escape from this island.

> Show list of all villages

```sql
SELECT * 
FROM village
```

> Show list of all inhabitants

```sql
SELECT * 
FROM inhabitant
```

> Show list of all inhabitants which have job as butcher

```sql
SELECT * 
FROM inhabitant 
WHERE job = 'butcher';
```

> Show list of all inhabitants which are friendly

```sql
SELECT * 
FROM inhabitant 
WHERE state = 'friendly';
```

> Show list of all weaponsmiths which are friendly

```sql
SELECT *
FROM INHABITANT
WHERE state = 'friendly' AND job = 'weaponsmith';
```

> Show list of all smiths

```sql
SELECT *
FROM INHABITANT
WHERE state = 'friendly' AND job LIKE '%smith';
```

> Mayor registers Stranger into city

```sql
INSERT INTO inhabitant (name, villageid, gender, job, gold, state) 
VALUES ('Stranger', 1, '?', '?', 0, '?');
```

> Display personid of Stranger

```sql
SELECT personid
FROM inhabitant
WHERE name = 'Stranger';
```

> Display gold of Stranger 

```sql
SELECT gold
FROM inhabitant
WHERE personid = 20;
```

> Show list of items without any owner

```sql
SELECT *
FROM item
WHERE owner IS NULL;
```

> Update coffee cup ownership to Stranger  

```sql
UPDATE item 
SET owner = 20 
WHERE item = 'coffee cup';
```

> Update all owner-less items' ownership to Stranger  

```sql
UPDATE item 
SET owner = 20 
WHERE owner IS NULL;
```
