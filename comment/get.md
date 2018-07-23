# Get Comment
---
# 请求类型: Get
# URL: https://jovanapi.top/comments/{id}
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
isLogin   | 是否登录（true/false） | Boolean
loginId   | 登录ID，若登录，需填此项 | Long
# Tip: 当isLogin=true且loginId不为空时为登录状态
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "comment query successfully",
    "data": {
        "id": 1,
        "postId": 1,
        "content": "test comment A",
        "repliesCount": 3,
        "points": null,
        "fromUid": 2,
        "fromUserName": "test@user2",
        "createdOn": "2018-07-23T07:19:41.000+0000"
    }
}
</code></pre>
