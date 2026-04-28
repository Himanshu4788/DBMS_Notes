# DBMS_Notes
Normalization (DBMS)
  Normalization is the process of organizing data in a database to:
    Remove redundancy (duplicate data)
    Improve data consistency & integrity

Why do we need Normalization?
  Duplicate data
  Update errors
  Inconsistent data


1NF (First Normal Form)
  No repeating groups
  Atomic values (single value per cell)


2NF (Second Normal Form)
  Must be in 1NF
  No partial dependency(Depends on full primary key)


3NF (Third Normal Form)
  Must be in 2NF
  No transitive dependency(Non-key should depend only on key)



BCNF
   Stronger version of 3NF
   Every determinant must be a candidate key


4NF (Fourth Normal Form)
  It is in BCNF
  It has no multi-valued dependencies (When one attribute determines multiple independent values)
 
  4NF removes redundancy caused by independent multi-valued attributes



5NF (Fifth Normal Form)
  It is in 4NF
  It has no join dependency( When a table can be split into smaller tables and reconstructed (joined) without losing data)


Why rarely used?
  Complex to implement
  More joins → slower queries
  Rare real-world need
