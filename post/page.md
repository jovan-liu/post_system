# Posts page
---
# 请求类型: GET
# URL: https://jovanapi.top/posts （e.g. https://jovanapi.top/posts?pageNum=1&pageSize=2）
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
    "msg": "post query page successfully",
    "data": {
        "total": 1,
        "list": [
            {
                "id": 1,
                "categoryId": 1, // 分类ID
                "categoryName": "论道", // 分类名称
                "title": "test title", // 标题
                "content": "test content", // 内容
                "postType": "text", // 帖子类型
                "totalCount": 5, // 总回复数 = commentsCount + repliesCount
                "points": 1, // 点赞数
                "isUpvoted": false, // 当前用户是否点赞（匿名用户默认false）
                "createUserId": 1, // 创建人ID
                "createUserName": "test@user1", // 创建人用户名
                "createdOn": "2018-07-23T07:19:02.000+0000" // 创建时间
            }
        ],
        "pageNum": 1,
        "pageSize": 2,
        "size": 1,
        "startRow": 1,
        "endRow": 1,
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
