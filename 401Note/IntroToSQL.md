# PREP: Intro to SQL


## SQLBolt

Query data from SQL database

What's a table: in a DB, rows represent instances of the entity and columns are the properties

What is Schema: a description of the strucure of each table and the datatypes in each column
  - this structure promotes efficiency in the DB

  Keywords 
    {
      SELECT [column, another_column] 
      FROM [DB name]
      WHERE <conditional> [column name] and/or <conditional> [column name]
      ORDER BY [column] ASC/DESC
      LIMIT [limit_numner] OFFSET [offset_number]
    }

  Queries from Multiple tables - Database Normalization
    { minimize duplicate data in any table and promote database growth independently - in order to use this, write a query that combines all data then extract necessary information }
      - JOIN clause allows combination of row data across two separate tables
    {
      SELECT [Column]
      FROM [DB table name]
      INNER JOIN [another DB table name]
        ON [this_table.ID = another_table.id]
      Where etc etc etc
    }
  
  Inseting Data

  { INSERT statement declares which table to write into, the columns, and how many rows - insert mutliple rows at a time }

   {
      SELECT [Column]
      FROM [DB table name]
      INSERT INTO [table name] <column, another_column>
      VALUES [value/expression, value/expres, etc,etc]
      Where etc etc etc
    }

    <column> is used for when there is incomplete data, you can specify which columns you can write - the values need to match the columns specified

    {
      INSERT INTO boxoffice
      (movie_id, rating, sales_in_millions)
      VALUES (1, 9.9, 283742034 / 1000000);
    }
  
  Update Rows
  {
    UPDATE [table]
    SET [column] = [value_or_expr]
    WHERE <Condition>
  }
  DO NOT leave out the WHERE clause = causes update to apply to ALL rows (TIP: Test in a select query)

  DELETE
{
  DELETE FROM mytable
  WHERE condition;
}

Create Table - define table schema 

CREATE TABLE IF NOT EXISTS mytable (
    column DataType TableConstraint DEFAULT default_value,
    another_column DataType TableConstraint DEFAULT default_value,
    …
)
    Movies table schema
    CREATE TABLE movies (
        id INTEGER PRIMARY KEY,
        title TEXT,
        director TEXT,
        year INTEGER, 
        length_minutes INTEGER
    );

  ALTERING TABLES - 
Adding a new column
{
  ALTER TABLE [table_name]
  ADD [column] [DATA_TYPE]
    DEFAULT [default_value]
}
Dropping columns
{
  ALTER TABLE [table_name]
  DROP [column] 
}
Renaming Table
{
  ALTER TABLE [table_name]
  RENAME TO [new_table_name]
}
  
  Remove entire table

  {
    DROP TABLE IF EXISTS [table_name]
  }

  PHOTOS 
  1. [Exercise 01](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.1&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  2. [Exercise 02](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.2&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  3. [Exercise 03](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.3&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  4. [Exercise 04](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.4&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  5. [Exercise 05](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.5&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  6. [Exercise 06](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.6&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  13. [Exercise 13](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.7&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  14. [Exercise 14](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.8&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  15. [Exercise 15](https://mail.google.com/mail/u/0?ui=2&ik=fa552fbded&attid=0.1&permmsgid=msg-f:1744477555824044815&th=1835a1182988ab0f&view=att&disp=safe)
  16. [Exercise 16](./imgs/SQL%20-2.png)
  17. [Exercise 17](./imgs/SQLBolt3.png)
  18. [Exercise 18](./imgs/SQLBolt4.png)
