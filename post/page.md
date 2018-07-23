# Posts page
---
# 请求类型: GET
# URL: https://jovanapi.top/posts （e.g. https://jovanapi.top/posts?pageNum=1&pageSize=2）
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
pageNum | 第几页   | String
pageSize  | 一页多少        | String
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
                "categoryId": 1,
                "categoryName": "lundao",
                "title": "test title",
                "content": "test content",
                "postType": "text",
                "totalCount": 5,
                "points": null,
                "createUserId": 1,
                "createUserName": "test@user1",
                "createdOn": "2018-07-23T07:19:02.000+0000"
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
