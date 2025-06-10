---
layout: default
title: SQL Games - SQL Murder Mystery
---

# [SQL Murder Mystery](https://mystery.knightlab.com/)


### DB SCHEMA

![SQL Murder Mystery Schema](https://mystery.knightlab.com/schema.png)

```sql
SELECT * FROM crime_scene_report
WHERE date='20180115' AND city='SQL City' AND type='murder'

SELECT * FROM person
WHERE (name LIKE '%Annabel%' AND address_street_name='Franklin Ave') OR (address_street_name='Northwestern Dr');

```
