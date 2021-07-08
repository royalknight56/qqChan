<h1 align="center">qqChan🐧</h1>




<div align="center">


「qqChan」qq的消息推送bot,server酱的qq版。


</div>

# 功能

通过简单的请求向QQ用户推送消息

### 1.目前收到警告,接口暂时无法调用,具体需求联系2930470134
### 2.目前已经上线敏感词过滤系统


# 使用方法

### 1.添加qq酱的qq号[2930470152]

添加后才可发送哦!!

### 2.发送请求到http://myim.online/api/qmsg

#### 接口信息:

GET:/api/qmsg

#### 请求参数


字段       |字段类型       |字段说明 |是否必填|
------------|-----------|-----------|-----------|
user       |string        |发送目标的qq号| 是|
text       |string        |发送的文本| 是|


#### 返回值


字段       |字段类型       |字段说明 |
------------|-----------|-----------|
state       |string        |success: 代表成功,'fail:代表失败,具体原因看reason|
code       |string        |状态码|
reason      |string        |失败的原因|


#### 示例
http://myim.online/api/qmsg?user=123456789&text=你好

{"state":"success","code":"100"}

# 发送到群聊的使用方法


### 1.邀请qq酱加群[2930470152]

qq酱被邀请后才可发送哦!!

### 2.发送请求到http://myim.online/api/groupmsg

#### 接口信息:

GET:/api/groupmsg

#### 请求参数


字段       |字段类型       |字段说明 |是否必填|
------------|-----------|-----------|-----------|
group       |string        |发送目标的群号| 是|
text       |string        |发送的文本| 是|




#### 返回值


字段       |字段类型       |字段说明 |
------------|-----------|-----------|
state       |string        |success: 代表成功,'fail:代表失败,具体原因看reason|
code       |string        |状态码|
reason      |string        |失败的原因|


#### 示例
http://myim.online/api/groupmsg?group=123456789&text=你好

{"state":"success","code":"100"}



# 调用量

每天每人默认200次调用量
超出会返回错误
{"state":"fail","code":"102","reason":"超过每日调用上限200"}


Finished!!!
