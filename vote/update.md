# Update PostVote （更改点赞）
---
# 请求类型: PUT
# URL: https://jovanapi.top/postVote
# 请求头（headers）：Content-Type=application/x-www-form-urlencoded
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
userId | 用户ID   | Long
postId  | 帖子ID        | String
voteType   | 点赞类型(upvoted/downvoted)          | String
# Tip: 评论及回复更改点赞，只需将post换成对应的名称就行，如https://jovanapi.top/commentVote?userId=1&commentId=1&voteType=upvoted, 故不再另写API
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "post vote update successfully",
    "data": {
        "userId": 2,
        "postId": 3,
        "voteType": "downvoted"
    }
}
</code></pre>
