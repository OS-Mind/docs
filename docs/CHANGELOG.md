# Change Log

<!--
- New data types: BOOL, TIMESTAMP
- Client-Server Mode
- SQL: GROUP BY 
- Add CrossDB `TCP-B` benchmark test
- WAL

## 0.7.0 <small>(2024-08-26)</small>

**Features**
**Improvements**
**Test**
**Bug Fixes**

## 0.8.0 <small>(2024-08-26)</small>

**Features**

- Support operators: `>`, `>=`, `<`, `<=`, `!=`, `<>` https://github.com/crossdb-org/CrossDB/issues/13

**Improvements**
**Test**
**Bug Fixes**

-->

## 0.7.0 <small>(2024-08-26)</small>

**Features**

- `UPDATE` SET clause supports simple expression, ex: `SET val=val+5` `SET val=a-b`
- `UPDATE` SET supports prepared statement
- `INSERT` supports prepared statement
- New APIs: `xdb_bexec`, `xdb_vbexec`, `xdb_stmt_bexec`, `xdb_stmt_vexec`, `xdb_clear_bindings`

**Improvements**

- `INSERT` parser avoids malloc
- `UPDATE` only updates affected indexes
- Optimize `INSERT` `UPDATE` `DELETE` auto-commit performance for `IMDB` 

**Test**

- Improve benchmark test
- Add `SQLite` benchmark test

**Bug Fixes**

- Fix hash index infinite loop issue
- Fix bench test time unit `ns` to `us`


## 0.6.0 <small>(2024-08-18)</small>

**Initial refactor release**

- This project was redesigned and rewritten from scratch for over one year
- Standard RDBMS model
- New SQL APIs which can support more language
- MySQL style SQL and shell, which will be easy to study.


## 0.5.0 <small>(2023-06-26)</small>

**Features**

- CrossDB command line tool `crossdb-cli` is released
- Optimize insert/update/query/delete performance
- Add new API `cross_matchCreate` and `cross_matchFree`
- DML APIs supports `cross_fields_h` and `cross_match_h`

**Bug Fixes**


## 0.4.0 <small>(2023-06-20)</small>

**Features**

- Support FreeBSD(X64)
- Optimize insert/update/query/delete performance
- Add new API `cross_fieldsCreate` and `cross_fieldsFree`

**Bug Fixes**


## 0.3.0 <small>(2023-06-13)</small>

**Features**

- Support MacOS (X64 and ARM64)
- Change `CROSS_DB_XXX` to `CROSS_XXX`

**Bug Fixes**

- `cross_dbTblCreate` flags `CROSS_DB_RBTREE` doesn't create Primary Key Index type correctly


## 0.2.0 <small>(2023-06-07)</small>

**Features**

- Support Windows
- Support Linux ARM64

**Bug Fixes**


## 0.1.0 <small>(2023-06-03)</small>

- **Initial release**