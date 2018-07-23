# Comment page by postId
---
# 请求类型: GET
# URL: https://jovanapi.top/posts/{pid}/comments?pageNum=1&pageSize=2
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
                "postId": 1,
                "content": "test comment A",
                "repliesCount": 3,
                "points": null,
                "fromUid": 2,
                "fromUserName": "test@user2",
                "createdOn": "2018-07-23T07:19:41.000+0000"
            },
            {
                "id": 2,
                "postId": 1,
                "content": "test comment B",
                "repliesCount": 0,
                "points": null,
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
