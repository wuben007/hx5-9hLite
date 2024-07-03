# hx5-9hLite
### 移动光猫hx5-9hLite 获取超级密码 
1.   开启telnet 
curl --location --request POST 'http://192.168.1.1/boaform/set_telenet_enabled_mod.cgi' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'mode_name=/boaform/set_telenet_enabled_mod' \
--data-urlencode 'nonedata=0.8681615761763514' \
--data-urlencode 'telenet_enabled=1' \
--data-urlencode 'user_name=root' \
--data-urlencode 'user_password=nE7jA%5m'
替换密码
2. telnet 测试 telnet 192.168.1.1   出现登录 登录  用户名root ,密码为上面设置的密码
3. 查找超级账号的密码 ，进入 路径： /config/work   vi lastgood.xml  输入：/CMCCAdmin 则下一行则为 超级密码
4. 超级密码有有效期，具体多久没有测试，以及telnet 也会关机，需要的时候，可以重复操作
