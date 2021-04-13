### 添加

``` sql
INSERT INTO `表名` (`字段一`,`字段二`, `字段N`) VALUES (`value1`, `value2`,`...valueN`);
```

### 删除

``` sql
DELETE FROM `表名` WHERE `id=3<条件>` AND NAME="张三";
```

### 修改

``` sql
UPDATE `表名` SET field1=new-value1, field2=new-value2;
```

### 查询

``` sql
SELECT * FROM `表名`;

SELECT `字段一`,`字段二` FROM `表名` WHERE `id=3<条件>`;
```

### 分页查询

``` sql
-- 使用 LIMIT 属性来设定返回的记录数。
-- 通过OFFSET指定SELECT语句开始查询的数据偏移量。默认情况下偏移量为0。
SELECT `字段一`,`字段二` FROM `表名` WHERE `id>3<条件>` LIMIT N OFFSET M
```


### COUNT(column_name) 

``` sql
-- 函数返回指定列的值的数目（NULL 不计入）
SELECT COUNT(column_name) FROM table_name
```

### 外键

``` sql

```

### 连表查询

``` sql

```







### 参考

[菜鸟教程](https://www.runoob.com/mysql/mysql-tutorial.html)

[廖雪峰](https://www.liaoxuefeng.com/wiki/1177760294764384/1179613436834240)