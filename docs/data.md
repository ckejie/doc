## 数据字典

### user
> 用户表,储存用户信息

|字段|类型|空|默认|注释|
|:-|:---|:---:|:---|:---|
|id|int(10)|否||用户编号|	
|username|varchar(20)|否||用户名|
|email|varchar(50)|是|null|邮箱|
|password|varchar(50)|否|null|密码|
|avatar|varchar(200)|是|null|头像|
|nick_name|varchar(20)|是|null|昵称|
|created_at|int(11)|是|null|注册时间|

--------------------------------
### product
> 产品表,储存产品信息

|字段|类型|空|默认|注释|
|:-|:---|:---:|:---|:---|
|id|int(10)|否||项目编号|	
|title|varchar(50)|否||项目名称|
|description|varchar(250)|是|null|项目内容|
|price|int(10)|是|null|价格(单位:分)|
|uid|int(10)|否|null|发布者编号|
|created_at|int(11)|是|null|发布时间|
