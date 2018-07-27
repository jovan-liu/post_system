# Get Replies
---
# 请求类型: GET
# URL: https://jovanapi.top/replies/{id}
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
    "msg": "reply query successfully",
    "data": {
        "id": 1,
        "postId": 1,
        "commentId": 1,
        "replyId": null,
        "replyType": "Comment",
        "replyLevel": 1,
        "content": "test reply AA",
        "points": 1,
        "voteType": upvoted, // 当前用户点赞状态（匿名用户统一为null）
        "fromUid": 3,
        "fromUserName": "test@user3",
        "toUid": 2,
        "toUserName": "test@user2",
        "createdOn": "2018-07-23T07:21:23.000+0000"
    }
}
</code></pre>
