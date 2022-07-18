# UNION
- UNION: only keeps unique records
- UNION ALL: keeps all records, including duplicates

e.g. 

student table:
| First_Name  | Last_Name |
| ------------- | ------------- |
| Joe  | Hash  |
| Marry  | Wang  |
| Frank | Plum  |
| Tom  | Louis  |

facebook table:
| First_Name  | Last_Name |
| ------------- | ------------- |
| Kim | Carol  |
| Frank | Plum  |
| Gary  | Washington  |
| David | Lee |


  **SELECT * FROM students UNION SELECT * FROM teachers** :
 
| First_Name  | Last_Name |
| ------------- | ------------- |
| Joe  | Hash  |
| Marry  | Wang  |
| Frank | Plum  |
| Tom  | Louis  |
| Kim | Carol  |
| Gary  | Washington  |
| David | Lee |


**SELECT * FROM students UNION ALL SELECT * FROM teachers** :
| First_Name  | Last_Name |
| ------------- | ------------- |
| Joe  | Hash  |
| Marry  | Wang  |
| Frank | Plum  |
| Tom  | Louis  |
| Kim | Carol  |
| Frank | Plum  |
| Gary  | Washington  |
| David | Lee |
