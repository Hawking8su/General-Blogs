# Data Types 数据类型对比总结

更新日期：2021-06-14

详细见：20210614-DataTypes数据类型总结.xlsx

## Programming Languages 编程语言

Data types & Data structures & Programming unit

![image-20210614181620887](https://raw.githubusercontent.com/Hawking8su/Images/main/20210614181948.png)



## Databases 数据库

| Data Type Group | Sqlserver      | Oracle        | Mysql                    | Hive          | Hive 补充说明                                           |
| --------------- | -------------- | ------------- | ------------------------ | ------------- | ------------------------------------------------------- |
| Number          | int            | number(m,d)   | int                      | int           |                                                         |
|                 | decimal(m,d)   | float(m,d)    | tinyint                  | tinyint       |                                                         |
|                 | numeric(m,d)   | binary_float  | smallint                 | smallint      |                                                         |
|                 | bigint         | binary_double | mediumint                | bigint        |                                                         |
|                 | smallint       |               | bigint                   | float         |                                                         |
|                 | tinyint        |               | float(m,d)               | double        | Hive 2.2.0                                              |
|                 | money          |               | double(m,d)              | decimal       | Hive 0.13.0                                             |
|                 | smallmoney     |               | decimal(m,d)             | numeric       | Hive 3.0.0                                              |
|                 | bit            |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
|                 | float(m,d)     |               |                          |               |                                                         |
|                 | real           |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
| Strings         | char           | char          | char(m)                  | string        |                                                         |
|                 | varchar        | varchar2      | varchar(m)               | varchar       | Hive 0.12.0                                             |
|                 | text           | nchar         |                          | char          | Hive 0.13.0                                             |
|                 | nchar          | nvarchar2     |                          |               |                                                         |
|                 | nvarchar       |               |                          |               |                                                         |
|                 | ntext          |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
| Binary Strings  | binary         | blob          | blob or text             | binary        | Hive 0.8.0                                              |
|                 | varbinary      | clob          | tinyblob or tinytext     | boolean       |                                                         |
|                 | image          | nclob         | mediumblob or mediumtext |               |                                                         |
|                 |                | bfile         | longblob or longtext     |               |                                                         |
|                 |                | long          | enum                     |               |                                                         |
|                 |                | raw           |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
| Datetime        | date           | date          | date                     | date          | Hive 0.12.0                                             |
|                 | datetime2      | timestamp     | datetime                 | timestamp     | Hive 0.8.0                                              |
|                 | datetime       | interval      | timestamp                | interval      | Hive 1.2.0                                              |
|                 | time           |               | time                     |               |                                                         |
|                 | datetimeoffset |               |                          |               |                                                         |
|                 | smalldatetime  |               |                          |               |                                                         |
|                 |                |               |                          |               |                                                         |
| Other           |                |               |                          | Complex Types |                                                         |
|                 |                |               |                          | array         | ARRAY<data_type>                                        |
|                 |                |               |                          | map           | MAP<primitive_type, data_type>                          |
|                 |                |               |                          | struct        | STRUCT<col_name : data_type [COMMENT col_comment], ...> |
|                 |                |               |                          | union         | incomplete support                                      |

![image-20210614115722629](https://raw.githubusercontent.com/Hawking8su/Images/main/20210614181955.png)

Reference:

- Sqlserver: https://docs.microsoft.com/en-us/sql/t-sql/data-types/data-types-transact-sql?view=sql-server-ver15
- Oracle: https://docs.oracle.com/database/121/SQLRF/sql_elements001.htm#SQLRF0021
- Mysql:https://dev.mysql.com/doc/refman/8.0/en/data-types.html
- Hive: https://cwiki.apache.org/confluence/display/Hive/LanguageManual+Types