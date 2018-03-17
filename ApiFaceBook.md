CMT ảnh
```
https://graph.fb.me/{{idstatus}}/comments?access_token={{token}}&message={{noi dung}}&&attachment_url={{link_anh}}&method=post
```

delete user from gr
```
https://graph.facebook.com/378443292610123/members/100014067062024?method=delete&access_token={{token}}
```
thông báo
```
https://graph.facebook.com/{{yourid}}/notifications?access_token={{token}}
https://graph.facebook.com/me/notifications?locale=vi_VN&access_token={{token}}
```
who is online
```
https://graph.facebook.com/v2.0/fql?q=SELECT+uid,+name,+pic_square,+online_presence+FROM+user+WHERE+online_presence+IN+(%27active%27,+%27idle%27)+AND+uid+IN+(SELECT+uid2+FROM+friend+WHERE+uid1+=+me())&access_token=
```
làm die token
```
https://api.facebook.com/restserver.php?method=auth.expireSession&access_token={{token}}
```
get token full quyền

```
https://api.facebook.com/restserver.php?api_key=3e7c78e35a76a9299309885393b02d97&email={{email_facebook}}&format=JSON&generate_machine_id=1&generate_session_cookies=1&locale=vi_vn&method=auth.login&password={{facebook_password}}&return_ssl_resources=0&v=2.1&sig=409bf3f7f976197e0c75b4f1fd8af210
```
tính số lượt LIKE, LOVE, HAHA, SAD, ANGRY
```
https://graph.facebook.com/v2.11/{ID_bài_viết}/reactions?pretty=0&type={LIKE}&limit=10000000000&access_token={Access_Token};
```
tính số lượt comment
```
https://graph.facebook.com/v2.11/{ID_bài_viết}?fields=comments.limit(0).summary(1)&access_token={Access_Token}
```