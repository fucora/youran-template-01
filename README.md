# youran-template-01

#### 介绍

本项目是[youran代码自动化平台](https://gitee.com/caixiaoge/youran)的预置代码模板：
**java标准后端模板**

包含如下技术栈：
- [spring-boot](https://spring.io/projects/spring-boot/)+[mybatis](http://www.mybatis.org/mybatis-3/)架构
- [hibernate-validator](http://hibernate.org/validator/releases/)
- [swagger](https://swagger.io/)(API文档自动生成)
- [mapstruct](http://mapstruct.org/)(属性映射)
- 基于[H2](http://www.h2database.com)内存数据库的单元测试


#### 软件架构
标准的maven模块化结构，包含以下三个模块：

1. common模块
2. core模块
3. web模块

##### common模块

和业务无关的通用代码，包括：
- LoginContext接口
- dao接口
- BusinessException异常类
- 乐观锁相关抽象代码
- pojo的超类及接口
- 通用util工具包
- 防xss相关通用代码


##### core模块

和具体业务相关的核心代码，包括：
- 业务相关dao接口及mybatis的dao.xml
- 业务相关pojo类
- 业务相关service类

##### web模块

和具体业务相关的web层代码，包括：
- 项目启动入口类
- 包含swagger注解的api文档接口
- controller类
- 单元测试代码
- 单元测试目录下还有数据库建表脚本


#### 安装教程

1.  首先保证本地maven仓库中已经安装了youran代码生成器的核心jar包
2.  用package命令直接编译打包本项目
3.  打包完之后生成的youran-template-01-x.x.x-SNAPSHOT-src.zip
就能在youran平台中导入了
