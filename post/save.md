# Register User
---
# 请求类型: POST
# URL: https://jovanapi.top/posts
# 请求头（headers）：Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
categoryId | 分类ID   | Long
categoryName  | 分类名称（论道，读经，心路）        | String
title   | 标题          | String
content | 内容（post_type为text时可选）  | String
postType | 帖子类型 （text, image, video, link） | String
createUserId | 创建人ID | Long
createUserName | 创建人用户名 | String
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "post created successfully",
    "data": {
        "id": 2,
        "categoryId": 1,
        "categoryName": "论道",
        "title": "test title 2",
        "content": "test content 2",
        "postType": "text",
        "totalCount": null,
        "points": null,
        "createUserId": 2,
        "createUserName": "test@user2",
        "createdOn": "2018-07-23T08:06:34.518+0000"
    }
}
</code></pre>
