# Delete PostVote （取消点赞）
---
# 请求类型: DELETE
# URL: https://jovanapi.top/postVotes/{userId}/{postId}
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
userId | 用户ID   | Long
postId  | 帖子ID        | Long
# Tip: 评论及回复点赞，只需将post换成对应的名称就行，如https://jovanapi.top/commentVotes/1/1, 故不再另写API
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "postVote delete successfully",
    "data": {}
}
</code></pre>
