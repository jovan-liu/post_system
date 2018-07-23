# Get Post
---
# 请求类型: GET
# URL: https://jovanapi.top/posts/{id}
# e.g.: https://jovanapi.top/posts/1 (例子)
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
    "msg": "post query successfully",
    "data": {
        "id": 1,
        "categoryId": 1,
        "categoryName": "lundao",
        "title": "test title",
        "content": "test content",
        "postType": "text",
        "totalCount": 5,
        "points": 1,
        "isUpvoted":true,
        "createUserId": 1,
        "createUserName": "test@user1",
        "createdOn": "2018-07-23T07:19:02.000+0000"
    }
}
</code></pre>
