# Database Seller Used Cars

## Data types:
- strings: [varchar(number), char(number), text, longtext]
- numbers: [tinyint, smallint, mediumint, int, bigint]
- decimals: [float(i,d), double(i,d), decimal(i,d)]
- dates: [datetime, date, time, year, timestamp]

## Attributes:
- NULL / NOT NULL
- DEFAULT(value)
- PRIMARY_KEY
- AUTO_INCREMENT
- UNIQUE

## Entity name: Car

## Table name: Cars

## Table columns:
- id                | BIGINT, PRIMARY_KEY, AUTO_INCREMENT, NOTNULL, UNIQUE, INDEX
- car_plate         | CHAR(7), NOTNULL, UNIQUE
- manufacturer      | VARCHAR(30), NOTNULL, INDEX
- model             | VARCHAR(50), NOTNULL, INDEX
- setup             | VARCHAR(50), NULLABLE
- description       | TEXT, NULLABLE
- car_image         | VARCHAR(255), NOTNULL, UNIQUE
- price             | DECIMAL(9,2), NOTNULL, INDEX
- year              | YEAR, NOTNULL
- kms               | MEDIUMINT, NOTNULL
- fuel_type         | VARCHAR(30), NOTNULL, INDEX
- transmission      | VARCHAR(20), NOTNULL, INDEX
- kw                | SMALLINT, NOTNULL
- engine_capacity   | SMALLINT, NOTNULL
- euro_class        | TINYINT, NULLABLE
- length            | SMALLINT, NULLABLE
- height            | SMALLINT, NULLABLE
- width             | SMALLING, NULLABLE
- car_type          | VARCHAR(30), NOTNULL
- car_doors         | TINYINT, DEFAULT(5)
- seats             | TINYINT, DEFAULT(5)
- color             | VARCHAR(30), NOTNULL, INDEX
- car_state         | VARCHAR(50), NULLABLE
- optionals         | TEXT, NULLABLE
- precedent_owners  | TINYINT, DEFAULT(1)
- sold              | TINYINT, DEFAULT(0), INDEX
