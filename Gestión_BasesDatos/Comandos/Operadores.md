OPERADORES LOGICOS : TRUE O FALSE

OPERADORES

```
SELECT *
FROM campo
WHERE description LIKE "%guide%"
```

OPERADORES AND

```
SELECT *
FROM campo
WHERE category = "Offensive Security" AND campo = "Bug bounty"
```

OPERADOR OR

```
SELECT *
FROM books
WHERE name LIKE "%Android%" OR name LIKE "%iOS%"
```

OPERADOR NOT

```
SELECT *
FROM books 
WHERE NOT description LIKE "%guide%"
```

OPERADOR BETWEEN

```
SELECT *
FROM books
WHERE id BETWEEN 2 AND 4;
```

