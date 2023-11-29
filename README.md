## 本项目实现的最终作用是基于JSP个人日记本
## 分为1个角色
### 第1个角色为作者账号，实现了如下功能：
 - 个人中心管理
 - 写日记
 - 日记分类管理
 - 登录页面
 - 登陆主页
## 数据库设计如下：
# 数据库设计文档

**数据库名：** diary

**文档版本：** 


| 表名                  | 说明       |
| :---: | :---: |
| [t_diary](#t_diary) |  |
| [t_diarytype](#t_diarytype) |  |
| [t_user](#t_user) | 用户表 |

**表名：** <a id="t_diary">t_diary</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | diaryId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | title |   varchar   | 60 |   0    |    Y     |  N   |   NULL    |   |
|  3   | content |   text   | 65535 |   0    |    Y     |  N   |   NULL    | 内容  |
|  4   | typeId |   int   | 10 |   0    |    Y     |  N   |   NULL    |   |
|  5   | releaseDate |   datetime   | 19 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="t_diarytype">t_diarytype</a>

**说明：** 

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | diaryTypeId |   int   | 10 |   0    |    N     |  Y   |       |   |
|  2   | typeName |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |

**表名：** <a id="t_user">t_user</a>

**说明：** 用户表

**数据列：**

| 序号 | 名称 | 数据类型 |  长度  | 小数位 | 允许空值 | 主键 | 默认值 | 说明 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
|  1   | UserId |   int   | 10 |   0    |    N     |  Y   |       | 用户ID  |
|  2   | userName |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 用户名  |
|  3   | password |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 密码  |
|  4   | nickname |   varchar   | 255 |   0    |    Y     |  N   |   NULL    | 昵称  |
|  5   | imageName |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |
|  6   | mood |   varchar   | 255 |   0    |    Y     |  N   |   NULL    |   |

**运行不出来可以微信 javape 我的公众号：源码码头**
