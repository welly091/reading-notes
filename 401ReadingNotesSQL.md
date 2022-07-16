---
layout: default
---


# Basic SQL

## #SELECT
- SELECT can select strings or numbers from database. Concatenation or calculation can be done inside select.
- e.g. SELECT 164/8, SELECT 'We'+'Are'
- e.g. SELECT * -> 'star' means 'all'

## #FROM
- FROM means from specific database.

## #ORDER BY
- Sort the selected data by specific order in specific column.
- DESC-> descending ; ASC -> ascending

## #LIMIT
- Choose how many data we want to select.
- e.g. SELECT * FROM students LIMIT 3  -> only choose three data from student table.

## #OFFSET
- The position you want to start in data
- e.g. SELECT * FROM students LIMIT 5 OFFSET 2 -> Starts from 3rd data to 8th data.


## What is schema?
> Schema = tables + relationships


![psql Schema Shortcuts](https://i.imgur.com/eeJQQ7T.jpg)


# Mid-Level SQL

## #WHERE
- WHERE can have conditions followed by it which is either true or false. 
- e.g. SELECT * FROM studens WHERE name = 'Brenda'

## #AND
- If you have multiple conditions that are all needed to be matched, AND can be put after WHERE to connect to conditions.

## #OR
- Multiple conditions that only either one needs to be matched, use OR after WHERE.

## #NOT
- Opposite to AND, select the data only when the condition(s) is not matched.

## Math Operators
- = equal
- < less than
- \> greater than
- <= less than or equal
- \>= greater than or equal
- != not equal
- <> not equal

## String Operators
- LIKE : a string matches a pattern
  - _ : matches any single character
  - % : matches any number of characters
- ILIKE : case insensitive version of LIKE (in other word, don't care about upper/lower case)
- SIMILAR TO : a string matches a reges pattern

## NULL
- IS NULL : matches NULL values
- IS NOT NULL : matches all non NULL values

## Aggregate Function()
### COUNT()
- Count selected items
- DISTINCT : 
  - Add DISTINCT clause to eliminate the repetitive appearance. 
  - e.g. COUNT(DISTINCT expr,[expr...])
### AS
- Give a new key word for selected item
