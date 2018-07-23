# Save Replies
---
# 请求类型: POST
# URL: https://jovanapi.top/replies
# 请求头（headers）: Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
postId | 帖子ID   | Long
commentId | 评论ID   | Long
replyId | 父回复ID   | Long
replyType | 回复类型（Comment, Reply）   | String
replyLevel | 回复层级   | Integer
content  | 内容        | String
fromUid  | 回复人ID        | Long
fromUserName  | 回复人用户名   | String
toUid  | 被回复人ID        | Long
toUserName  | 被回复人用户名   | String

# Tip: 回复类型指的是回复的是评论（comment）还是回复（reply），若是回复的是评论，则不需要填写replyId

# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "reply created successfully",
    "data": {
        "id": 4,
        "postId": 1,
        "commentId": 1,
        "replyId": 3,
        "replyType": "Reply",
        "replyLevel": 4,
        "content": "test reply DD",
        "points": null,
        "fromUid": 4,
        "fromUserName": "test@user4",
        "toUid": 3,
        "toUserName": "test@user3",
        "createdOn": "2018-07-23T08:46:24.298+0000"
    }
}
</code></pre>
