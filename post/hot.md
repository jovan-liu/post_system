# Posts top 3
---
# 请求类型: GET
# URL: https://jovanapi.top/posts/hot
# Tip: 根据points查询前3个帖子
# 返回值:
<pre><code>
{
	"code": 200,
	"msg": "post query top 3 successfully",
	"data": [{
		"id": 1,
		"categoryId": 1,
		"categoryName": "lundao",
		"title": "test title",
		"content": "test content",
		"postType": "text",
		"totalCount": 10,
		"points": 2,
		"voteType": null,
		"createUserId": 1,
		"createUserName": "admin",
		"createdOn": "2018-07-22T09:46:21.000+0000"
	}, {
		"id": 2,
		"categoryId": 1,
		"categoryName": "lundao",
		"title": "test post title 2",
		"content": "test post content 222",
		"postType": "text",
		"totalCount": 0,
		"points": 2,
		"voteType": null,
		"createUserId": 1,
		"createUserName": "admin",
		"createdOn": "2018-07-22T15:45:22.000+0000"
	}, {
		"id": 6,
		"categoryId": 1,
		"categoryName": "lundao",
		"title": "test title 44",
		"content": "test content 44",
		"postType": "text",
		"totalCount": 0,
		"points": 0,
		"voteType": null,
		"createUserId": 1,
		"createUserName": "admin",
		"createdOn": "2018-07-31T04:56:34.000+0000"
	}]
}
</code></pre>
