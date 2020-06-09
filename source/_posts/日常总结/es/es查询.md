title:  es查询与聚合细节
date: 2020-06-08
tags:[elasticsearch,query,search]
---
通过收集的资料学习elasticsearch query and aggs篇

 <!--more-->

 # es查询与聚合细节

 ## es查询

 `可知的是es的版本迭代犹为的快,一些版本间的修修改改也特别多,所以这里有查询主要以我收集到的资料为主,目前的主要目的是去掌握一套,后续再去调研是否存在较大的版本间的差异`

进入正题

### 全部查询

方式1

```
POST /indexName/_search
{
    "match_all":{}
}

```

方式2

```
GET /indexName/_search
{
"match_all":{}
}
```

方式3 :match_all可以省略

```
GET /indexName/_search
{

}
```

