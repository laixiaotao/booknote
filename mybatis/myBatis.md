# 1. 简介

**视频链接：** https://www.bilibili.com/video/BV1NE411Q7Nx 

**官网链接：** https://mybatis.org/mybatis-3/zh/index.html 

## 1.1 什么是 MyBaits

+ **作用：**MyBatis 是一款优秀的**持久层框架**，它支持自定义 SQL、存储过程以及高级映射。MyBatis 免除了几乎所有的 JDBC 代码以及设置参数和获取结果集的工作。MyBatis 可以通过简单的 XML 或注解来配置和映射原始类型、接口和 Java POJO（Plain Old Java Objects，普通老式 Java 对象）为数据库中的记录 。

+ **环境：**

  + JDK 1.8
  + Mysql 5.7
  + maven 3.6.1
  + IDEA

+ **依赖：**

  ~~~xml
  <!-- https://mvnrepository.com/artifact/org.mybatis/mybatis -->
  <dependency>
      <groupId>org.mybatis</groupId>
      <artifactId>mybatis</artifactId>
      <version>3.5.5</version>
  </dependency>
  ~~~

  

## 1.2 持久化

+ **数据持久化：**
  + 持久化就是将程序的数据在持久状态和瞬时状态转化的过程
  + 内存：**断电即失**
  + 数据库 (JDBC)，io文件持久化
+ **原因：**
  + 有一些对象，不能让他丢掉
  + 内存太贵了



## 1.3 持久层

Dao 层，Service 层，Controller 层

+ 完成持久化工作的代码块
+ 层界限区分十分明显



## 1.4 为什么需要 MyBaits

传统的 JDBC 操作繁琐复杂，myBaits 简化了数据库操作

+ **优点：**
  + 简单易学
  + 灵活
  + 解除 sql 与程序代码的耦合：通过提供 DAO 层，将业务逻辑和数据访问逻辑分离，使系统的设计更清晰，更易维护，更易单元测试。sql 和代码的分离，提高了可维护性。
  + 提供映射标签，支持对象与数据库的 orm 字段关系映射
  + 提供对象关系映射标签，支持对象关系组建维护
  + 提供 xml 标签，支持编写动态 sql。