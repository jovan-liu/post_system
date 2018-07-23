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
        "total": 3,
        "list": [
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
        "pageNum": 1,
        "pageSize": 2,
        "size": 2,
        "startRow": 1,
        "endRow": 2,
        "pages": 2,
        "prePage": 0,
        "nextPage": 2,
        "isFirstPage": true,
        "isLastPage": false,
        "hasPreviousPage": false,
        "hasNextPage": true,
        "navigatePages": 8,
        "navigatepageNums": [
            1,
            2
        ],
        "navigateFirstPage": 1,
        "navigateLastPage": 2,
        "firstPage": 1,
        "lastPage": 2
    }
}
</code></pre>
