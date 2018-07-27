# Posts page
---
# 请求类型: GET
# URL: https://jovanapi.top/category/{cid}/posts
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
pageNum | 第几页   | Integer
pageSize  | 一页多少        | Integer
isLogin   | 是否登录（true/false） | Boolean
loginId   | 登录ID，若登录，需填此项 | Long
# Tip: 当isLogin=true且loginId不为空时为登录状态
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "post query page by categoryId successfully",
    "data": {
        "total": 2,
        "list": [
            {
                "id": 1,
                "categoryId": 1,
                "categoryName": "lundao",
                "title": "test title",
                "content": "test content",
                "postType": "text",
                "totalCount": 7,
                "points": 2,
                "voteType": upvoted, // 当前用户点赞状态（匿名用户统一为null）
                "createUserId": 1,
                "createUserName": "test@user1",
                "createdOn": "2018-07-23T07:19:02.000+0000"
            },
            {
                "id": 2,
                "categoryId": 1,
                "categoryName": "论道",
                "title": "test title 2",
                "content": "test content 22",
                "postType": "text",
                "totalCount": 0,
                "points": -3,
                "voteType": downvoted, // 当前用户点赞状态（匿名用户统一为null）
                "createUserId": 2,
                "createUserName": "test@user2",
                "createdOn": "2018-07-23T08:10:53.000+0000"
            }
        ],
        "pageNum": 1,
        "pageSize": 4,
        "size": 2,
        "startRow": 1,
        "endRow": 2,
        "pages": 1,
        "prePage": 0,
        "nextPage": 0,
        "isFirstPage": true,
        "isLastPage": true,
        "hasPreviousPage": false,
        "hasNextPage": false,
        "navigatePages": 8,
        "navigatepageNums": [
            1
        ],
        "navigateFirstPage": 1,
        "navigateLastPage": 1,
        "firstPage": 1,
        "lastPage": 1
    }
}
</code></pre>
