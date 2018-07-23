# Comment page by postId
---
# 请求类型: GET
# URL: https://jovanapi.top/posts/{pid}/comments
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
pageNum | 第几页   | Integer
pageSize  | 一页多少        | Integer
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "comment query page successfully",
    "data": {
        "total": 2,
        "list": [
            {
                "id": 1,
                "postId": 1, // 帖子ID
                "content": "test comment A", // 内容
                "repliesCount": 3, // 回复总数 = repliesCount
                "points": 1, // 点赞数
                "isUpvoted": false, // 当前用户是否点赞（匿名用户默认false，登录用户尚未实现）
                "fromUid": 2, // 评论人ID
                "fromUserName": "test@user2", // 评论人用户名
                "createdOn": "2018-07-23T07:19:41.000+0000" // 评论时间
            },
            {
                "id": 2,
                "postId": 1,
                "content": "test comment B",
                "repliesCount": 0,
                "points": 0,
                "isUpvoted": false,
                "fromUid": 3,
                "fromUserName": "test@user3",
                "createdOn": "2018-07-23T07:19:41.000+0000"
            }
        ],
        "pageNum": 1,
        "pageSize": 2,
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
