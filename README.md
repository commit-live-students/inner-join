![GitHub Logo](https://s3.ap-south-1.amazonaws.com/greyatom-social/GreyAtom-logo.png)

# INNER JOINS

The most important and frequently used of the joins is the INNER JOIN. They are also referred to as an EQUIJOIN.

The INNER JOIN creates a new result table by combining column values of two tables (table1 and table2) based upon the join-predicate. The query compares each row of table1 with each row of table2 to find all pairs of rows which satisfy the join-predicate. When the join-predicate is satisfied, column values for each matched pair of rows of A and B are combined into a result row.

### Syntax

The basic syntax of the INNER JOIN is as follows.

        SELECT table1.column1, table2.column2...
        FROM table1
        INNER JOIN table2
        ON table1.common_field = table2.common_field;

Now, let us join these two tables using the INNER JOIN as follows −

        SELECT  Customers.CustomerID, Customers.CustomerName, ORDERS.OrderDate
            FROM Customers
            INNER JOIN ORDERS
            ON Customers.CustomerID = ORDERS.CustomerID;

This would produce the following result.

| CustomerID | CustomerName | OrderDate |
| ---------- | --------- | --------- |
| 51 | Bottom-Dollar Marketse	| 2017-03-20 |
| 71 | Split Rail Beer & Ale | 2016-11-21 |
| 72 | Princesa Isabel Vinhoss	| 2016-12-29 |
| 73 | Folk och fä HB	| 2017-01-04 |
| 74 | Consolidated Holdings	| 2017-03-28 |
