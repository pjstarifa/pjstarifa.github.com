---
layout: post
title: "Information Schema Views"
date: 2013-05-29 12:02
comments: true
categories: sql
published: false
---

Information Schema Views are a set of views in a database which contain metadata about the schema. 
Typically your ORM of choice will not provide strongly typed access to information schema views. 
However you can create views of your own to provide strongly typed access. 

<!-- more -->
``` sql Create Information Schema View 

    create view isvTables as 
      select * from information_schema.tables
    
    create view isvColumns as 
      select * from information_schema.columns
```

{% gist 996818 %}

{% jsfiddle tCjsq result.js.html.css %}


