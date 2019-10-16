
用户注册(regiest)
---
```
baseUrl = https://api.github.com
```

传输方法：`POST`

访问路径：`baseUrl + /repos/:uid/:name/contents/:id`

* 请求参数:

|参数名|类型|必选|说明|
|:-    |:------:|:------:|:---|
|uid|Int|是|用户编号|
|name|String|是|项目名称|
|id|Int|是|栏目编号|

* 请求头:
```json
{
  "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/77.0.3865.90 Safari/537.36"
  ""
}
```
* 请求表单:
```json
{
  "name": "guest",
  "pwd": "5D4sD6ff498f6J46feP498eW",
  "phone": 13012340001 ,
  "code": "102030",
  "realName": "张三",
}
```
|参数名|类型|必选|说明|
|:-    |:------:|:------:|:---|
|name|String|是|用户名|
|pwd|String|是|密码MD5|
|phone|String|是|手机号|
|code|String|是|验证码|
|realName|String|否|真实名称|
* 返回结果:
```json
{
    "status": 0,
    "message": "成功",
    "data": {
      "uid": "1",
      "username": "12154545",
      "name": "吴系挂",
      "groupid": 2 ,
      "reg_time": "1436864169",
      "last_login_time": "0",
    }
  }
```
|参数名|类型|必选|说明|
|:-    |:------:|:------:|:---|
|uid|Int|是|用户编号|
|username|String|是|用户名|
|name|String|是|用户真实姓名|
|groupid|Int|是|用户组id，1：超级管理员；2：普通用户|
|reg_time|Time|是|注册时间|
|last_login_time|Time|是|最后登录时间|

