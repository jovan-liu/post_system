# Page reply by commentId
---
# 请求类型: GET
# URL: https://jovanapi.top/comments/{cid}/replies
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
pageNum | 第几页   | Integer
pageSize  | 一页多少        | Integer
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "reply query page successfully",
    "data": {
        "total": 3, // 总记录数
        "list": [ // 当前分页数据
            {
                "id": 1,
                "postId": 1,
                "commentId": 1,
                "replyId": null,
                "replyType": "Comment",
                "replyLevel": 1,
                "content": "test reply AA",
                "points": null,
                "fromUid": 3,
                "fromUserName": "test@user3",
                "toUid": 2,
                "toUserName": "test@user2",
                "createdOn": "2018-07-23T07:21:23.000+0000"
            },
            {
                "id": 2,
                "postId": 1,
                "commentId": 1,
                "replyId": 1,
                "replyType": "Reply",
                "replyLevel": 2,
                "content": "test reply BB",
                "points": null,
                "fromUid": 2,
                "fromUserName": "test@user2",
                "toUid": 3,
                "toUserName": "test@user3",
                "createdOn": "2018-07-23T07:21:23.000+0000"
            }
        ],
        "pageNum": 1, // 当前页数
        "pageSize": 2, // 每页的数量
        "size": 2, // 当前页的数量
        "startRow": 1, // 当前页面第一个元素在数据库中的行号
        "endRow": 2, // 当前页面最后一个元素在数据库中的行号
        "pages": 2, // 总页数
        "prePage": 0, // 上一页
        "nextPage": 2, // 下一页
        "isFirstPage": true, // 是否是第一页
        "isLastPage": false, // 是否是最后一页
        "hasPreviousPage": false, // 是否有上一页
        "hasNextPage": true, // 是否有下一页
        "navigatePages": 8, // 导航页码数
        "navigatepageNums": [ // 所有导航页号
            1,
            2
        ],
        "navigateFirstPage": 1, // 导航条上的第一页
        "navigateLastPage": 2, // 导航条上的最后一页
        "firstPage": 1, // 第一页
        "lastPage": 2 // 最后一页
    }
}
</code></pre>
