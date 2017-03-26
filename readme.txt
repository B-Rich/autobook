模块介绍:
loginMan 负责登陆,检查登陆信息,获取cookie值(用户信息都保存在cookie里面)
watchMan 检查订场信息的变化(8天都需要检查），log住任何变化，发现有免费场地，立即通知上级
bookMan 负责执行订场程序（由上级安排，什么号码订哪个场地），把订场结果通知给上级
recordMan记录了订场信息，可用号码,数据必须持续化
master 协调各方面的工作
consoleMan 提供web界面,录入号码,查询订场信息.取消订单(需提早24小时),布置订场计划.查询log，设置接受邮箱，发送邮箱帐号
logMan记录所有信息(登陆成功失败,订场成功失败,邮件发送,程序状态,对方服务器状况等)
mailMan发送订场信息
configMan 记录login地址，个人中心地址，查询地址，下单地址。（此文件不放github）
utilMan 需要的工具函数

需要的工具库
lxml lxml解析html
pyquery pyquery是依赖于lxml包的，lxml没有安装成功，那么pyquery也无法正常执行。
logging  日志输出


var baseURL='/sport';