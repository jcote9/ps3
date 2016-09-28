# ps3

## Problem Set 3 

1. Define the terms: relation, tuple, attribute, record, and field.

  A relation is a table that may consist of numerous attributes, which are columns or fields. A relation may also have (multiple) tuple(s) which is a row or a record. 
  
2. What are keys in a relation?

  There are multiple key types in a relation, and keys function in multiple ways. Foreign keys identify records in a relation by      matching a primary key in a different table. A primary key is a determinate that holds a unique value which identifies each record in the relation. There are also candidate keys, natural, surrogate, and composite keys.  
  
3. What is a surrogate key and how is it used?

  A surrogate key is independent of the item/data. Meaning that they are not derived from application data, they are just values that are generated and then stored with the rest of the columns in a record. 

4. In the following equation, Area = Length x Width, identify the determinant(s).

  The determinant(s) are length and width, because both of these determine the area. The area is dependent on the length and width values. 

5. If a relation has no duplicate data, how can you be sure there is always at least one primary key?

  You can create a foreign key that links two tables (key columns and related columns of another table). In other words, the foreign key identifies records in a table by matching a primary key in a different table. 

6. Give an example of a relation.  Determine a natural key for this relation.

  An example of a relation would be R=(adv ID, AD first, AD last, office, phone, ad department) The natural key for this relation would be the advisors ID, because it has a logical relationship with to the other attributes in the record. 

  For question 7 - 8, Consider product *orders*.  In particular, associated with an order is: customer name (first and last), address (street, city, state, zip), phone, email, the products orders (including item, quantity, and price).  

7. Create a relational data model for *orders*.  Consider applying normalization rules (discuss Monday)

  R= (order_id, customer_id, invoice_number, status)
  I would apply the first normalization rule and divide the date into indivisible units. The primary key in this relation is the order_number. I would create a customer entity. Customers= (order_id, c_first, c_last, zip, state) 

8. For customer, could email be used as a primary key?  If so, state why.  Also, if possible to use as a primary key, discuss any disadvantages of using email as a primary key.

  I do not think email is a good canditate for a primary key. This is because, a primary key needs to be hold a unique value. It may be possible that two people have similar email addresses. 

9. Given two relations S and R below find the Cartsian Product S x R.

  Every element of S has to be matched of each element of R. (1,2,3,1,1 1,2,2,2,3,1,2,1,2,5,2,3,3,1,1,2,3,2,2,3,2,3,2,1,5)
  
10. Find the natural join between the Faculty and Department relations below.

  The natural join is department, because this column has a relationship with the rest of the data. 

 
S
--------------
| A | B |
|---|---|
| 1 | 2 |
| 2 | 3 |
---------

R
------------
| C | D | E |
|---|---|---|
| 3 | 1 | 1 |
| 2 | 2 | 3 |
| 2 | 1 | 5 |



Faculty
--------------
| Name | ID | Dept |
|-------|----|----------------|
| Joe | 1 | Chemistry |
| Susan | 2 | Math |
| Tom | 3 | Marine Science |
| Mike | 4 | Math |


Department
------------
| Dept | Chair  |
|---|---|
| Chemistry | John |
| Math | Mike |
| Marine Science | Barry |
