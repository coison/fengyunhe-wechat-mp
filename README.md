# 简介
此项目是一个非官方的微信公众号SDK，适用于java环境下的微信公众号后台开发使用。


# 功能

已经实现的功能有：
* 获取接口调用凭据
  * 获取access_token
  * 获取微信服务器IP地址
* 接收消息
  * 接收普通消息
  * 接收事件推送
* 发送消息
  * 被动回复消息
  * 客服接口
  * 群发接口
  * 模板消息接口
  * 模板消息运营规范
  * 获取自动回复规则
* 消息加解密
* 素材管理 （没有完全测试）
  * 新增临时素材
  * 获取临时素材
  * 新增永久素材
  * 获取永久素材
  * 删除永久素材
  * 修改永久图文素材
  * 获取素材总数
  * 获取素材列表
* 用户管理
  * 用户分组管理
  * 设置用户备注名
  * 获取用户基本信息(UnionID机制)
  * 获取用户列表
  * 获取用户地理位置
  * 网页授权获取用户基本信息
* 自定义菜单管理
  * 自定义菜单创建接口
  * 自定义菜单查询接口
  * 自定义菜单删除接口
  * 自定义菜单事件推送
* 账号管理
  * 生成带参数的二维码
  * 长链接转短链接接口
* JS-SDK 的JS-TICK生成
* 发送红包、分裂红包
* 微信门店（没有测试过）

没有实现的功能有：
* 微信支付
* 微信卡券
* 微信小店
* 微信WIFI
* 微信摇一摇周边


因为有些功能需要有特定的条件才可以开发和测试，所以也希望可以找到有条件一起开发和维护的朋友。
如果有想要一起维护这个项目的可以加群：233753794


## JDK 加密位数限制异常的处理：
<ol>
	<li>在官方网站下载JCE无限制权限策略文件，需要根据使用的jdk版本下载对应的文件。（JDK7的下载地址：
     http://www.oracle.com/technetwork/java/javase/downloads/jce-7-download-432124.html</li>
	<li>下载后解压，可以看到local_policy.jar和US_export_policy.jar以及readme.txt</li>
	<li>如果安装了JRE，将两个jar文件放到%JRE_HOME%\lib\security目录下覆盖原来的文件</li>
	<li>如果安装了JDK，将两个jar文件放到%JDK_HOME%\jre\lib\security目录下覆盖原来文件</li>
</ol>
