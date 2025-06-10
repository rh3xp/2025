---
layout: default
title: Python - List, Set, Tuples
---


## Lists

```python
lst = list()

# append is used to add elements in the list
lst.append("Mr.")
lst.append(["Parth", "Krishna"])
lst.extend(["is", "a", "developer"])
```

## Sets

```python
set_var = set()
set_var = {"Avengers", "IronMan", "Hitman"}
set_var2 = {"Avengers", "IronMan", "Hitman", "Hulk"}

# Only prints the difference of the set values
set_var2.difference(set_var)
# Updates set_var2 and removes all common values from set_var
set_var2.difference_update(set_var)

# Only prints the common values of the set
set_var2.intersection(set_var)
# Updates set_var2 and keeps only all common values from set_var
set_var2.intersection_update(set_var)
```

## Tuples

Only used when assignment is required for a one-off incident.
