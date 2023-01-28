---
title: "FMDB"
date: "2015-05-15"
categories: 
  - "ios"
tags: 
  - "fmdb"
---

Useful ways to get data out of FMDB.

Count

```
NSUInteger count = [db intForQuery:@"SELECT COUNT(field) FROM table_name"];
```

Make sure to include the [`FMDatabaseAdditions.h` header file](https://github.com/ccgus/fmdb/blob/master/src/FMDatabaseAdditions.h) to use `intForQuery:`

Max

```
NSUInteger max = [db intForQuery:@"SELECT MAX(field) FROM table_name"];
```

Min

```
NSUInteger min = [db intForQuery:@"SELECT MIN(field) FROM table_name"];
```

Average

```
NSUInteger average = [db intForQuery:@"SELECT AVG(field) FROM table_name"];
```

Sum (Σ)

```
NSUInteger sum = [db intForQuery:@"SELECT SUM(field) FROM table_name"];
```

Total

```
NSUInteger total = [db intForQuery:@"SELECT TOTAL(field) FROM table_name"];
```

[https://www.sqlite.org/lang\_aggfunc.html](https://www.sqlite.org/lang_aggfunc.html)
