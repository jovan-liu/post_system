# Page reply by commentId
---
# 请求类型: GET
# URL: https://jovanapi.top/comments/{cid}/replies
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
pageNum | 第几页   | Integer
pageSize  | 一页多少        | Integer
isLogin   | 是否登录（true/false） | Boolean
loginId   | 登录ID，若登录，需填此项 | Long
# Tip: 当isLogin=true且loginId不为空时为登录状态; 默认排序方式为replyLevel升序，若为值null则在最前
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
                "postId": 1, // 帖子ID
                "commentId": 1, // 评论ID
                "replyId": null, // 回复父ID
                "replyType": "Comment", // 回复类型 Comment Reply
                "replyLevel": 1, // 回复等级
                "content": "test reply AA", // 内容
                "points": 1, // 点赞数
                "voteType": upvoted, // 当前用户点赞状态（匿名用户统一为null）
                "fromUid": 3, // 回复人ID
                "fromUserName": "test@user3", // 回复人用户名
                "toUid": 2, // 被回复人ID
                "toUserName": "test@user2", // 被回复人用户名
                "createdOn": "2018-07-23T07:21:23.000+0000" // 回复时间
            },
            {
                "id": 2,
                "postId": 1,
                "commentId": 1,
                "replyId": 1,
                "replyType": "Reply",
                "replyLevel": 2,
                "content": "test reply BB",
                "points": 0,
                "voteType": upvoted,
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
