# Update Post
---
# 请求类型: PUT
# URL: https://jovanapi.top/posts
# 请求头（headers）: Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
id | 帖子ID   | Long
content  | 内容        | String
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "post updated successfully",
    "data": {
        "id": 2,
        "categoryId": 1,
        "categoryName": "论道",
        "title": "test title 2",
        "content": "test content 22",
        "postType": "text",
        "totalCount": null,
        "points": null,
        "createUserId": 2,
        "createUserName": "test@user2",
        "createdOn": "2018-07-23T08:10:53.000+0000"
    }
}
</code></pre>
