---
title: MongoDB
category: Development
---

## Querying

```
{ name: 'john' }
{ name: { $eq: 'john' } }

## dump restore

mongodump --uri=mongodb://user:passord@host:port/dbname

mongorestore -h <hostname><:port> -d dbname <path>
