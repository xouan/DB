
# sql语言及其种类
## DDL(data definition language,数据定义语言)
用来创建或者删除存储数据用的数据库以及数据库中的表等对象

1. CREATE:创建数据库和表等对象
create database <数据库名>
create database shop
create table <表名> (
    <列1> <数据类型> <该列约束>,
    <列2> <数据类型> <该列约束>,
    ...
    <该表的约束>...
);
 CREATE TABLE Product
 (product_id char(4) not null,
 product_name varchar(100) not null,
 product_type varchar(32) not null,
 sale_price integer  ,
 purchase_price integer  ,
 regist_date date  ,
 primary key (product_id)
 );

2. DROP：删除数据库和表等对象
drop database <数据库名>
drop table <表名>

3. ALTER:修改数据库和表等对象

## DML(data mamipulation language, 数据操纵语言) （*****）
用来查询或者变更表中的记录

1. SELECT：查询表中的数据
2. INSETT:向表中插入新数据
3. UPDATE：更新表中的数据
4. DELETE:删除表中的数据

## DCL(data control language, 数据控制语言)
用来确认或者取消对数据库中的数据进行的变更。除此之外，还可以对 RDBMS 的用户是否有权限操作数据库中的对象（数据库表等）进行设定。

1. COMMIT：确认对数据库中的数据进行的变更
2. ROLLBACK:取消数据库中的数据进行的变更
3. GRANT：赋予用户操作权限、
4. REVOKE：取消用户的操作权限

## 显示数据库与表的数量
show databases
show tables