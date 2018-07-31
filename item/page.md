# Item page
---
# 请求类型: GET
# URL: https://jovanapi.top/items
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
pageNum | 第几页   | Integer
pageSize  | 一页多少        | Integer
# 返回值:
<pre><code>
{
	"code": 200,
	"msg": "query item by id successfully",
	"data": {
		"total": 3,
		"list": [{
			"id": 1,
			"itemName": "item test 1", // 商品名称
			"itemCode": "test", // 商品code
			"itemDesc": "item desc 1", // 商品描述
			"price": 60.9, // 商品价格
			"icon": "https://img10.360buyimg.com/n7/jfs/t22951/40/802097321/412821/42b44509/5b433243N888b865f.jpg", // 商品图片
			"url": "https://item.jd.com/25627446665.html", // 商品网址
			"createdOn": "2018-07-31T05:43:43.000+0000"
		}, {
			"id": 2,
			"itemName": "item test 2",
			"itemCode": "test",
			"itemDesc": "item desc 2",
			"price": 70.0,
			"icon": "https://img13.360buyimg.com/n7/jfs/t21175/266/2173579744/505765/af1ddf8b/5b4aa953N7fcff026.jpg",
			"url": "https://item.jd.com/4889153.html",
			"createdOn": "2018-07-31T05:43:43.000+0000"
		}],
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
		"navigatepageNums": [1, 2],
		"navigateFirstPage": 1,
		"navigateLastPage": 2,
		"firstPage": 1,
		"lastPage": 2
	}
}
</code></pre>
