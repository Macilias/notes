SQL

>select:
SELECT column1, column2, ...
FROM table_name;

>update:
UPDATE table_name
SET column1 = value1, column2 = value2, ...       
WHERE condition;

>insert

[ WITH [ RECURSIVE ] with_query [, ...] ]
INSERT INTO table_name [ ( column_name [, ...] ) ]
    { DEFAULT VALUES | VALUES ( { expression | DEFAULT } [, ...] ) [, ...] | query }
    [ RETURNING * | output_expression [ [ AS ] output_name ] [, ...] ]

INSERT INTO films VALUES
    ('UA502', 'Bananas', 105, '1971-07-13', 'Comedy', '82 minutes');
OR
INSERT INTO films (code, title, did, date_prod, kind)
    VALUES ('T_601', 'Yojimbo', 106, '1961-06-16', 'Drama');

IMPORTANT: if set varchar then column1 = ‚value1‘ use singe quotes!