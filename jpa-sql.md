![jpa-sql](https://img.shields.io/jetbrains/plugin/v/15242-jpa-sql?label=version&style=flat-square)
[![jpa-sql](https://img.shields.io/jetbrains/plugin/d/15242-jpa-sql?style=flat-square)](https://plugins.jetbrains.com/plugin/15242-jpa-sql/versions)
![](https://visitor-badge.glitch.me/badge?page_id=jpa-sql)

# JPA-SQL
## Features
- Restore mybatis sql log to original whole sql.
- It will generate executable sql statements with replace ? to the really param value.
- Select the console sql log and right-click "Restore Sql" menu to restore sql.

![](https://plugins.jetbrains.com/files/15242/348-page/image272.png)

## Config
Taking the springboot project as an example, the output level of the sql log needs to be configured in the application.yml file as: `trace`  
```yaml
logging:
  level:
    org.hibernate.type.descriptor.sql.BasicBinder: trace
```
Complete configuration example:
```yaml
server:
  port: 8080
spring:
  datasource:
    driverClassName: com.mysql.jdbc.Driver
    url: jdbc:mysql://localhost:3306/test?useSSL=false&useUnicode=true&characterEncoding=utf8&serverTimezone=UTC
    username: root
    password: root
  jpa:
    database-platform: org.hibernate.dialect.MySQL5InnoDBDialect
    show-sql: true
    hibernate:
      ddl-auto: update
    properties:
      hibernate.format_sql: false
logging:
  level:
    org.hibernate.type.descriptor.sql.BasicBinder: trace
```
Settings button configuration on the left side of the plugin window：  
**Preparing:** `Hibernate:`  
**Parameters:** `binding parameter`  
![](https://plugins.jetbrains.com/files/15242/348-page/image273.png)  

## Button Features
- **Text**: Restore sql from text
- **Settings**: Setup filter rules and navigation switch
- **Format**: Output beautiful formatted sql statements
- **Rerun**: Rerun plugin
- **Stop**: Stop plugin

## Example
```sql
Hibernate: select userdo0_.id as id1_0_0_, userdo0_.last_login_time as last_log2_0_0_, userdo0_.password as password3_0_0_, userdo0_.sex as sex4_0_0_, userdo0_.user_name as user_nam5_0_0_ from t_user userdo0_ where userdo0_.id=?
2020-10-24 09:45:07.895 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
Hibernate: update t_user set last_login_time=?, password=?, sex=?, user_name=? where id=?
2020-10-24 09:45:07.949 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [TIMESTAMP] - [Sat Oct 24 09:45:07 CST 2020]
2020-10-24 09:45:07.952 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [2] as [VARCHAR] - [passWord]
2020-10-24 09:45:07.953 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [3] as [INTEGER] - [1]
2020-10-24 09:45:07.954 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [4] as [VARCHAR] - [fishpro]
2020-10-24 09:45:07.954 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [5] as [INTEGER] - [1]
Hibernate: select userdo0_.id as id1_0_0_, userdo0_.last_login_time as last_log2_0_0_, userdo0_.password as password3_0_0_, userdo0_.sex as sex4_0_0_, userdo0_.user_name as user_nam5_0_0_ from t_user userdo0_ where userdo0_.id=?
2020-10-24 09:45:07.973 TRACE 9980 --- [           main] o.h.type.descriptor.sql.BasicBinder      : binding parameter [1] as [INTEGER] - [1]
```
JPA SQL output executable sql statements:
```sql
--  1
 select userdo0_.id as id1_0_0_, userdo0_.last_login_time as last_log2_0_0_, userdo0_.password as password3_0_0_, userdo0_.sex as sex4_0_0_, userdo0_.user_name as user_nam5_0_0_
 FROM t_user userdo0_
 WHERE userdo0_.id=1;
--  ------------------------------------------------------------------------------------------------
--  2
 update t_user set last_login_time='Sat Oct 24 09:45:07 CST 2020', password='passWord', sex=1, user_name='fishpro'
 WHERE id=1;
--  ------------------------------------------------------------------------------------------------
--  3
 select userdo0_.id as id1_0_0_, userdo0_.last_login_time as last_log2_0_0_, userdo0_.password as password3_0_0_, userdo0_.sex as sex4_0_0_, userdo0_.user_name as user_nam5_0_0_
 FROM t_user userdo0_
 WHERE userdo0_.id=1;
--  ------------------------------------------------------------------------------------------------
```

## Pictures
![](https://plugins.jetbrains.com/files/15242/348-page/image274.png)  

## Download
[jpa-sql](https://plugins.jetbrains.com/plugin/15242-jpa-sql/versions)  

## Price
`$5/year`

## Plugins
* [MyBatis Log Plugin](https://plugins.jetbrains.com/plugin/13905-mybatis-log-plugin) 
* [JPA SQL](https://plugins.jetbrains.com/plugin/15242-jpa-sql) 
* [Smart Jump](https://plugins.jetbrains.com/plugin/14053-smart-jump) 
* [Smart Search](https://plugins.jetbrains.com/plugin/14615-smart-search)
* [Toolset](https://plugins.jetbrains.com/plugin/14384-toolset) 
