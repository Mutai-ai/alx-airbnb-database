##1NF - First Normal Form

- All tables have atomic columns (no multiple values in one column).
- Each record is uniquely identifiable via a primary key (UUID).
  
## 2NF - Second Normal Form

- No tables use composite primary keys.
- Every non-key attribute fully depends on the entire primary key.
- Thus it is in 2NF
  
## 3NF - Third Normal Form

- There are no transitive dependencies.
- All non-key attributes depend only on the primary key and not on other non-key attributes.
