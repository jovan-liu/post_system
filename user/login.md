# User Login
---
# 请求类型: POST
# URL: https://jovanapi.top/user/login
# 参数:
参数名 | 说明                   | 类型
----- |----------------------- | ----
userName | 用户名（唯一,必填）   | String
password  | 密码（必填）        | String
# 返回值:
<pre><code>
{
    "code": 200,
    "msg": "user login successfully",
    "data": {
        "id": 4,
        "userName": "test@user4",
        "displayName": null,
        "password": "1ebaee4578e8c3d86c524fce8d57f39c3debae73",
        "passwordSalt": "688ccb88-4198-4192-a507-e58ea41b21ae",
        "email": "test_user4@newbeleive.com",
        "emailVerify": null,
        "phone": null,
        "avatar": null,
        "createdOn": "2018-07-23T07:37:30.000+0000"
    }
}
</code></pre>
