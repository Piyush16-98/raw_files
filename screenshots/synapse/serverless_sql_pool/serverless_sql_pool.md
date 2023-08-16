# 1. Read data from datalake


```python
SELECT top 10 * from 
OPENROWSET(
    bulk 'https://storage_name.dfs.core.windows.net/input/a.csv',
    format = 'csv',
    HEADER_ROW = TRUE,
    PARSER_VERSION = '2.0') 
as r1
```

![https://raw.githubusercontent.com/Piyush16-98/raw_files/main/screenshots/synapse/serverless_sql_pool/read_Datalake_csv_Screenshot%202023-08-16%20191926.png](attachment:image-2.png)


```python

```
