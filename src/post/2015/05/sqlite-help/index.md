---
title: "SQLite Help"
date: "2015-05-10"
categories: 
  - "ios"
tags: 
  - "date"
  - "sqlite"
---

Order By Date

Dates are stored as TEXT or if you want a number from 1970.

If they are TEXT and you want to sort them you need to convert them to a Date first.

```
SELECT * FROM Table ORDER BY date(dateColumn) DESC
```
