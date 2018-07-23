# Save Comment
---
# 请求类型: POST
# URL: https://jovanapi.top/comments
# 请求头（headers）: Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
postId | 帖子ID   | Long
content  | 内容        | String
fromUid | 评论人ID | Long
fromUserName | 评论人用户名 | String
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "comment created successfully",
    "data": {
        "id": 3,
        "postId": 1,
        "content": "test comment C",
        "repliesCount": null,
        "points": null,
        "fromUid": 4,
        "fromUserName": "test@user4",
        "createdOn": "2018-07-23T08:25:27.125+0000"
    }
}
</code></pre>
