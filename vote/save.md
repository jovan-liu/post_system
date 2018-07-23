# Save PostVote （给帖子点赞）
---
# 请求类型: POST
# URL: https://jovanapi.top/postVotes
# 请求头（headers）：Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
userId | 用户ID   | Long
postId  | 帖子ID        | String
voteType   | 点赞 (upvoted/downvoted)          | String
# Tip: 评论及回复点赞，只需将post换成对应的名称就行，如https://jovanapi.top/commentVotes?userId=1&commentId=1&voteType=upvoted, 故不再另写API
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "post vote save successfully",
    "data": {
        "userId": 2,
        "postId": 3,
        "voteType": "upvoted"
    }
}
</code></pre>
