### What is SQL?
*SQL, or Structured Query Language, is a language designed to allow both technical and non-technical users query, manipulate, and transform data from a relational database. And due to its simplicity, SQL databases provide safe and scalable storage for millions of websites and mobile applications.*

* A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

#### To create table:
`CREATE TABLE "table_name"`
`("column_1" "data_type_for_column_1",`
`"column_2" "data_type_for_column_2",`
`... )`

#### Select query for a specific columns:
`SELECT column, another_column, …`
`FROM mytable;`

#### Select query with constraints:
`SELECT column, another_column, …`
`FROM mytable`
`WHERE condition`
    `AND/OR another_condition`
    `AND/OR …;`

 #### Add columns in an existing table:
 `ALTER TABLE table_name ADD column_name datatype`   

 