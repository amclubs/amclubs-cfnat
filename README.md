# amclubs-cfnat
解决Cloudflare的泛播IP的问题，WIn、Mac、Linux、IOS、Android各端现实中遇到cf官方ip /cdn-cgi/trace 后会出现不同的路由和数据中心反馈。 cfnat是一个自动查找自动进行CF转发的工具，目的是为了解决泛播ip路由乱跳的问题。 有了它，绝大多数用户网络环境下用cf中转ip意义就不大了。 其中高阶用法是修改同目录下的ips-v4.txt和ips-v6.txt 用上面的colo工具找适合自己的cidr地址段。
