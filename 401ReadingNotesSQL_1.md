---
layout: default
---


# Basic SQL

## #SELECT
- SELECT can select strings or numbers from database. Concatenation or calculation can be done inside select.
- e.g. SELECT 164/8, SELECT 'We'+'Are'
- e.g. SELECT * -> 'star' means 'all'
- If you select data but want to exclude a column, use two dashes ('--') with the column you don't want to selecct. 
  - SELECT column1, --column2 FROM table_name

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
