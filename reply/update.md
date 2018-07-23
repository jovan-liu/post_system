# Update Replies
---
# 请求类型: PUT
# URL: https://jovanapi.top/replies
# 请求头（headers）: Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
id | 回复ID   | Long
content  | 内容        | String
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "reply updated successfully",
    "data": {
        "id": 4,
        "postId": 1,
        "commentId": 1,
        "replyId": 3,
        "replyType": "Reply",
        "replyLevel": 4,
        "content": "test reply DDD",
        "points": null,
        "fromUid": 4,
        "fromUserName": "test@user4",
        "toUid": 3,
        "toUserName": "test@user3",
        "createdOn": "2018-07-23T08:47:38.000+0000"
    }
}
</code></pre>
