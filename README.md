<h1 align="center">qqChan🐧</h1>




<div align="center">


「qqChan」qq的消息推送bot,server酱的qq版。


</div>

# 功能

通过简单的请求向QQ用户推送消息


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
user       |string        |发送目标的qq号|
text       |string        |发送的文本|


#### 示例
http://myim.online/api/qmsg?user=123456789&text=你好

{
    "user": "123456789",
    "text": "你好"
}


Finished!!!


