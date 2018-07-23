# Update Comment
---
# 请求类型: PUT
# URL: https://jovanapi.top/comments
# 请求头（headers）: Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
id | 评论ID   | Long
content  | 内容        | String
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "comment updated successfully",
    "data": {
        "id": 3,
        "postId": 1,
        "content": "test comment CC",
        "repliesCount": null,
        "points": null,
        "fromUid": 4,
        "fromUserName": "test@user4",
        "createdOn": "2018-07-23T08:26:57.000+0000"
    }
}
</code></pre>
