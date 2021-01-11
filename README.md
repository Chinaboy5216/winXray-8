[winXray 入门小技巧](./sub/introduce.md)   
[winXray 相关视频列表](https://www.youtube.com/results?search_query=winXray)  
[网络免费 vmess 服务器订阅链接](https://proxypool.ga/vmess/sub)   
[网络免费 Shadowsocks 服务器订阅链接](https://proxypool.ga/ss/sub)     
[网络免费 clash 服务器订阅链接](https://proxypoolss.tk/clash/proxies?speed=100&type=vmess,trojan)   
可复制上面各种格式订阅链接，在 winXray 中点击「批量导入链接」体验 winXray 有强大的兼容性。  

# 使用前必读
本软件没有像其他同类软件那样包含任何机场的推广链接，    
本作者不通过本源码获得任何好处，本软件的源码无保留的公开，本软件不勉强任何人使用。       
  
删库跑路的原因大家都懂不用我多说了吧？！   
我删库特别快，是因为我写代码的速度快，我用了几小时就完成了 winXray 的主要代码，我用了几天升级就迅速达到了一般其他软件写了几年的成熟度，这不是我的错吧？！因为我即将删库，但是我推上去的更新 - fork 的项目基本都没有那么迅速的主动拉更新，大家可以看一下 winXray 上线才短短几天就超过了 600 forks, 所以如果我推送更新之前不删库，那么我删库以后就没有人能找到最新版本的源代码。这个事情不是很难理解吧？！   
  
现在大多杀毒软件都是白名单查杀，所以新生的EXE都会乱报病毒，因为我更新的速度太快，所以不断的推新EXE上来，所以你可能遇到误报，但是你完全可以使用源代码自己编译出一模一样的EXE，还有人吹牛说其他翻墙软件不误报 - 你去 issues 里以及网上搜一下有多少误报好不好？！遇到误报可以提交给你的杀毒厂商核实，也可以自己编译源码生成EXE后使用，解决和核实问题很容易 - 其他套路都是多余的。
  
本来 winXray 源码已放弃版权贡献到公共域，但是有人把源码拿去拖了个又大又丑的推广按钮上去，什么功能也不加就发布新版自称官方，而且还把源码搞得很乱出了问题的对本作者进行诋毁（ 错误信息都看不懂居然自称开源软件官方 ），对提及原版 winXray 的用户进行封杀和威胁，我真是惊到了世上居然有如此无耻之人，本来就是给你自由发挥的，吃相这么难看良心不会痛吗？！本来我想改一个许可证限制一下这种不好的行为，但是最后我还是决定继续放弃版权，继续将源码贡献到公共域，即然开放源码，就一定要开放得彻底，我们不能因为世上有个别的恶棍而放弃自己善良的初心。 

# winXray 
winXray[:loud_sound:](http://dict.youdao.com/dictvoice?audio=winxray&type=2) 是最简洁轻快的 [V2Ray、Shadowsocks、Trojan](https://github.com/v2fly/v2ray-core) 通用客户端（Windows系统），秒速自动发现最快服务器，连接异常秒速智能切换，提供一键部署服务端工具。本软件源码已放弃版权贡献到公共域，源码可使用 [aardio](http://www.aardio.com) 编译生成单文件绿色EXE，**[点这里下载](./../../raw/master/release/winXray.7z)** （ [64位版本](./../../raw/master/release/winXray.7z) / [32位版本](./../../raw/master/release/winXray32.7z) ），解压即可直接使用( 仅  **[6.7MB](./../../raw/master/release/winXray.7z)** - 已自带 V2Ray Core）。    
   
之前我用过很多代理客户端，经常用一会就挂掉了，有些测试很久才找到下一个可用的服务器，有时怎么切换都不行，一定要把整个软件退出重启才能恢复。而且在WIN10上都有相同的BUG:PAC代理用一段时间就会卡死( winXray已经通过自行实现PAC服务器解决了这个问题 )，其实这些软件里提供的很多功能我并不需要，我只想愉快地用下 google 找点技术资料提升工作效率。但是在网上找了很久都没找到适合的软件，于是决定自己动手写一个，还好用 aardio 写软件的速度很快 - 大概用了几个小时就完成了 winXray 的主要代码，改进了几个版本以后就很稳定了，**我自己用了 winXray  几个月再也没有遇到 google 抽风访问不了的问题**。    

一些网友对 winXray 的测速功能存在误解，简单的测速不但不必要的消耗流量而且没有什么实用价值，例如Ping通了TCP访问不了，TCP通了但浏览器被阻断，或者下载测速需要连接代理服务器以后长时间测试才能得到下载速度 - 如果有很多服务器需要频繁快速地测速这样显然是不行的。**根据我长时间的实测，我使用一堆的服务器，大多时候 winXray 都能最快的找到其中速度最快、且能正常使用的线路**。要考虑到网络速度与服务器响应速度本来就是波动的，**winXray 能在连接代理服务器以前在零点几秒以内快速地在上百个代理服务器中找出最快的服务器** - 可以节省我们大量手动测试切换的时间，如果你有一个比我们幸福的网络环境，有一堆稳定流畅看4K视频的代理服务器 - 那你确实可以关闭自动切换功能 - 手动切换即可。

![winXray](./screenshots/winXray.png)

winXray支持批量导入 vless、vmess、ss、trojan、trojan-go …… 等格式的分享链接，  
也可以导入v2ray,、Shadowsocks、trojan等通用订阅链接，兼容 base 64、json …… 等不同格式的服务器配置，也可以导入 Clash proxy-provider 配置，winXray将自动转化各种不兼容的配置为统一、规范的格式。winXray 有强大的兼容性，我们甚至可以直接自 github 项目地址导入代理服务器，例如直接复制链接 [https://github.com/winXray/winXray/blob/master/sub/sample.json](./sub/sample.json) 即可一键导入 winXray。

![新增、编辑代理服务器](./screenshots/outbound.png)

![服务器配置](./screenshots/config.json.png)
**小技巧: JSON里点击任意字段都会显示该字段的用法说明。** 个人认为做很多对话框来配置服务器的参数是非常蠢的，winXray已经把各种代理协议的配置简化为几个统一命名的JSON字段（ **也可以作为一种标准的、统一的、通用的订阅响应格式使用** ），只要稍加学习就可以非常熟练的添加、修改各种代理协议的配置。而且对于大多数用户根本不需要改配置 - 简单的复制导入分享链接就可以，我们不必要把简单的事搞复杂。

可选在 ["/v2ray-core/winXray-default-servers.json"](./v2ray-core/winXray-default-servers.json) 文件中添加默认服务器配置（生成EXE后默认配置自动嵌入到EXE文件，可选删除该文件,也可以继续使用该文件覆盖EXE自带的默认服务器列表）。

![PAC配置](./screenshots/pac.png)
**小技巧: PAC编辑器里点击任意域名都会自动关联到单选框，可以直接切换代理或直连。**

软件首次运行时会在当前目录查找 "./v2ray-core/v2ray.exe"   
发行文件仅需要 "./winXray.exe"，可选带上 "./v2ray-core/" 目录（ 如果没有找到会自动到v2ray官网下载，不过没有代理服务器下载有时候非常慢 )。

![端口配置](./screenshots/config.advanced.png)

<img src="./screenshots/telegram.gif" width="1031" alt="Telegram 端口配置">

# PAC 代理的优点：
先说一下部分客户端 PAC 模式不稳定一直没解决，但 winXray 的 PAC 模式稳定流畅并没有这些问题。 
另外 winXray 的 PAC 代理兼容性惊人 - 可以完美支持 Telegram IP 地址库（ 旧版本升级请在 PAC 编辑器右键添加 Telegram IP 地址库 ） 

PAC 属于系统代理规则 - 是一种非常成( 老 )熟( 了 )的代理模式，与翻墙软件完全无关并完全独立，可以保证只有需要经过代理的域名才与翻墙软件发生关系。PAC 主要支持浏览器，可以避免迅雷、百度网盘、Steam 等流量在未经许可时经过翻墙软件。也只有 PAC 能真正让浏览器直接支持高效安全的 SOCKS5 协议，否则就只能改为低版本 SOCKS 或者 HTTP 代理。另外启用 PAC 并不会影响大家使用 V2Ray Core 自带的路由规则 -  实际上在 winXray 中使用自带的路由规则是非常方便的( winXray 在配置界面可直接修改 Core 配置 )。 
