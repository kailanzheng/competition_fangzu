- python
  - 全局变量和局部变量，生效范围
  - python函数访问和修改全局变量
  - python函数执行中，数组、字典等与整型、字符串等在函数修改数据产生的影响(值传递和地址传递)
  - 类、对象的定义实现，面向对象的三大特征，python的MRO(简单了解)
  - python的GIL，多线程、多进程、线程锁、进程池等的定义实现
  - python类中classmethod、staticmethod装饰器定义函数,类变量和实例变量
  -  python实现单例模式
  - python装饰器
  - (数据处理方面)dataframe，定义实现、增删查改、拼接合并
  - 代码注释，对复杂些的函数，写上函数功能、输入参数的功能和格式、返回值的功能和格式

- mysql
  - 表的增删查改
  - 在sql语句中`的作用
  - 索引的建立,以及为什么要建立索引
  - 事务
  - 建表 eg.
    - CREATE TABLE IF NOT EXISTS stock_cal
      (
          `id`          bigint NOT NULL AUTO_INCREMENT COMMENT '自增id',
          `exchange`     varchar(16) DEFAULT 'unknown' COMMENT '交易所',
          `cal_date`      varchar(16) DEFAULT 'unknown' COMMENT '日期',
          `is_open`        smallint DEFAULT 0 COMMENT '是否开盘',
          `pretrade_date`        varchar(16) DEFAULT 'unknown' COMMENT '前一交易日',
          `nexttrade_date`    varchar(16) default 'unknown' COMMENT '后一交易日',
          UNIQUE KEY `idx_exc_date` (`exchange`, `cal_date`),
          PRIMARY KEY (`id`)
      ) ENGINE = InnoDB
        DEFAULT CHARSET = utf8 COMMENT ='股票日历数据';
  - python使用pymysql库进行数据库的操作

- git
  - git init, clone, pull, push, add, commit
  - git checkout -b new_branch 创建并切换到新分支, 各分支的管理
  - (协作开发)针对别人的项目提出issue,fork别人的代码到自己仓库, 修改后提出合并请求
  - .gitignore文件
  - README.md文件