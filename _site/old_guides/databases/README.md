# Common db standards

## Dabatase naming

Database names will be in English.

Database names will contain the name of the project

Preffer `utf8` as database charset.

Consider that the databases will end up storing Romanian names, choose **case sensitive** collations that support correct sorting in Romanian.

## Database scripting

Always use migrations to deploy and upgrade your poject. Do not modify the database manually. If your technology stack supports migrations, leverage the support. If not, talk with us about how to properly deploy the database. Every change must be scripted, upgrade of existing data is required. Test your migrations on large datasets.

## Column data types

Column data types chosen for each column will try to be the LEAST precise type that will accomodate ALL POSSIBLE VALUES in all cases. 

Types that support optimization will be chosen (varchar, bit vs text, blob etc) <br/>

Reffer to your chosen backed database platform documentation for types, lengths and limits.

### CHAR vs. VARCHAR

Unless a small fixed size code (eg. `CHAR(5)`), preffer VARCHAR. The possible size overhead of variable length is more than compensated by the flexibility for future changes.

## Time

Preffer UTC time in the database. Altough Romania doe snot span multiple time zones, storing UTC avoids DST change anomalies (in November the same hour appears *twice* in the DST change day). If needed, convert to local time in presentation layer (ie. web front end).

### General considerations

The length attribute for numeric types does not affect the range of values that can be stored in the column. Columns defined as `TINYINT(1)` or `TINYINT(20)` can store the exact same values. Instead, for integers, the length dictates the display width; for decimals, the length is the total number of digits that can be stored.

If you need absolute precision when using non-integers, `DECIMAL` is preferred over `FLOAT` or `DOUBLE`.

MySQL has a `BOOLEAN` type, which is just a `TINYINT(1)`, with `0` meaning `FALSE` and `1` meaning `TRUE`.

MySQL also has several variants on the text types that allow for storing binary data. These types are `BINARY`, `VARBINARY`, `TINYBLOB`, `MEDIUMBLOB`, and `LONGBLOB`. Such types can be used for storing files or encrypted data.
