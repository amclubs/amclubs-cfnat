# [amclubs-cfnat](https://github.com/amclubs/amclubs-cfnat)
1、解决Cloudflare的泛播IP的问题，WIn、Mac、Linux、IOS、Android各端现实中遇到cf官方ip /cdn-cgi/trace 后会出现不同的路由和数据中心反馈。 cfnat是一个自动查找自动进行CF转发的工具，目的是为了解决泛播ip路由乱跳的问题。 有了它，绝大多数用户网络环境下用cf中转ip意义就不大了。 其中高阶用法是修改同目录下的ips-v4.txt和ips-v6.txt 用上面的colo工具找适合自己的cidr地址段。

2、通过结合Cloudflare部署VLESS、Trojan免费节点项目 [am-cf-tunnel](https://github.com/amclubs/am-cf-tunnel) 和 [am-cf-trojan](https://github.com/amclubs/am-cf-trojan) 实现自动优先IP实现科学上网。

#
▶️ **新人[YouTube](https://youtube.com/@am_clubs?sub_confirmation=1)** 需要您的支持，请务必帮我**点赞**、**关注**、**打开小铃铛**，***十分感谢！！！*** ✅
</br>🎁请 **follow** 我的[GitHub](https://github.com/amclubs)、给我所有项目一个 **Star** 星星（拜托了）！你的支持是我不断前进的动力！ 💖
</br>✅**解锁更多技能** [加入TG群【am_clubs】](https://t.me/am_clubs)、[YouTube频道【@am_clubs】](https://youtube.com/@am_clubs?sub_confirmation=1)、[【博客(国内)】](https://amclubss.com)、[【博客(国际)】](https://amclubs.blogspot.com) 
</br>✅点击观看教程[CLoudflare免费节点](https://www.youtube.com/playlist?list=PLGVQi7TjHKXbrY0Pk8gm3T7m8MZ-InquF) | [VPS搭建节点](https://www.youtube.com/playlist?list=PLGVQi7TjHKXaVlrHP9Du61CaEThYCQaiY) | [获取免费域名](https://www.youtube.com/playlist?list=PLGVQi7TjHKXZGODTvB8DEervrmHANQ1AR) | [免费VPN](https://www.youtube.com/playlist?list=PLGVQi7TjHKXY7V2JF-ShRSVwGANlZULdk) | [IPTV源](https://www.youtube.com/playlist?list=PLGVQi7TjHKXbkozDYVsDRJhbnNaEOC76w) | [Mac和Win工具](https://www.youtube.com/playlist?list=PLGVQi7TjHKXYBWu65yP8E08HxAu9LbCWm) | [AI分享](https://www.youtube.com/playlist?list=PLGVQi7TjHKXaodkM-mS-2Nwggwc5wRjqY)

#
![check-in](https://raw.githubusercontent.com/amclubs/amclubs-cfnat/main/amclubs-cfnat.jpg)

## 参数说明:
~~~
  -数据中心 string
        筛选数据中心例如 HKG,SJC,LAX (多个数据中心用逗号隔开,留空则忽略匹配)
  -本地IP string
        本地监听的 IP (default "0.0.0.0")
  -检查域名 string
        响应状态码检查的域名地址 (default "cloudflaremirrors.com/debian")
  -有效延迟 int
        有效延迟（毫秒），超过此延迟将断开连接 (default 300)
  -并发数 int
        并发请求最大协程数 (default 100)
  -本地端口 string
        本地监听的端口 (default "1234")
  -有效IP int
        提取的有效IP数量 (default 20)
  -目标IP int
        目标负载 IP 数量 (default 10)
  -目标端口 int
        转发的目标端口 (default 443)
  -随机IP
        是否随机生成IP，如果为false，则从CIDR中拆分出所有IP (default true)
  -tls
        是否为 TLS 端口 (default true)
  -ipv4/6 string
        指定生成IPv4还是IPv6地址 (4或6) (default "4")
~~~
香港：HKG 美国：USA 美国洛杉矶：LAX 美国圣何塞：SJC 日本：JPN 新加坡：SGP

CF端口类型:
HTTP：80，8080，8880，2052，2082，2086，2095

HTTPS：443，2053，2083，2087，2096，8443

 # 
<center>
<details><summary><strong> [点击展开] 赞赏支持 ~🧧</strong></summary>
*我非常感谢您的赞赏和支持，它们将极大地激励我继续创新，持续产生有价值的工作。*

- **USDT-TRC20:** `TWTxUyay6QJN3K4fs4kvJTT8Zfa2mWTwDD`
- **TRX-TRC20:** `TWTxUyay6QJN3K4fs4kvJTT8Zfa2mWTwDD`

<div align="center"> 
  <img src="https://github.com/user-attachments/assets/e6cdc42a-6374-4722-b833-601738f72196" width="200"></br> 
  TRC10/TRC20扫码支付 
</div> 
</details>
</center>

 #
 免责声明:
 - 1、该项目设计和开发仅供学习、研究和安全测试目的。请于下载后 24 小时内删除, 不得用作任何商业用途, 文字、数据及图片均有所属版权, 如转载须注明来源。
 - 2、使用本程序必循遵守部署服务器所在地区的法律、所在国家和用户所在国家的法律法规。对任何人或团体使用该项目时产生的任何后果由使用者承担。
 - 3、作者不对使用该项目可能引起的任何直接或间接损害负责。作者保留随时更新免责声明的权利，且不另行通知。
