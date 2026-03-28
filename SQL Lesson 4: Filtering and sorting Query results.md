# SQLBolt Exercise 4

## Table: movies

| id | title               | director       | year | length_minutes |
| -- | ------------------- | -------------- | ---- | -------------- |
| 1  | WALL-E              | Andrew Stanton | 2008 | 104            |
| 2  | A Bug's Life        | John Lasseter  | 1998 | 95             |
| 3  | Up                  | Pete Docter    | 2009 | 101            |
| 4  | Finding Nemo        | Andrew Stanton | 2003 | 107            |
| 5  | Cars 2              | John Lasseter  | 2011 | 120            |
| 6  | Monsters University | Dan Scanlon    | 2013 | 110            |
| 7  | Toy Story 2         | John Lasseter  | 1999 | 93             |
| 8  | Ratatouille         | Brad Bird      | 2007 | 115            |
| 9  | Monsters, Inc.      | Pete Docter    | 2001 | 92             |
| 10 | Brave               | Brenda Chapman | 2012 | 102            |
| 11 | Toy Story           | John Lasseter  | 1995 | 81             |
| 12 | Cars                | John Lasseter  | 2006 | 117            |
| 13 | The Incredibles     | Brad Bird      | 2004 | 116            |
| 14 | Toy Story 3         | Lee Unkrich    | 2010 | 103            |

---

## Task 1: List all directors of Pixar movies (alphabetically), without duplicates

```sql
SELECT DISTINCT director
FROM movies
ORDER BY director ASC;
```

---

## Task 2: List the last four Pixar movies released (most recent to least)

```sql 
SELECT * FROM movies
ORDER BY year DESC
LIMIT 4;
```

---

## Task 3: List the first five Pixar movies sorted alphabetically

```sql 
SELECT * FROM movies
ORDER BY title ASC
LIMIT 5;
```

---

## Task 4: List the next five Pixar movies sorted alphabetically

```sql 
SELECT * FROM movies
ORDER BY title ASC
LIMIT 5 OFFSET 5;
```
