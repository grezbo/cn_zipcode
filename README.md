# cn_zipcode

cn_zipcode 是一个中国邮编数据库，包含了从网上爬取的邮编数据

---

## 使用方法

#### 1. 创建数据库

我测试使用的是MariaDB
```sql
CREATE DATABASE `zip` DEFAULT CHARACTER SET utf8 COLLATE utf8_general_ci
```

#### 2. 创建表

使用 zip_code.sql 中的建表语句创建表

#### 3. 插入数据

使用 zip_code_insert_value.sql 中的insert语句插入数据

---

## 表结构展示

|  code  | province | city   | district   | area                             |
| ------ |----------| -------| ---------- | -------------------------------- |
| 200333 | 上海市   | 辖区   | 普陀区     |大渡河路(单1175-9999#双1122-9999#)|
| 230061 | 安徽省   | 合肥市 | 包河区     |屯溪路                            |
| 

---

##注意事项

1. 数据量有80多万条，建议建表时根据实际使用情况创建索引
2. 建议使用UTF-8编码
