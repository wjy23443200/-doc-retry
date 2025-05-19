# 审计规则说明表

> 以下规则用于常见网络审计、代理或过滤系统（如 Clash/V2Ray/防火墙等），识别特定行为或拦截不良请求。

## 1. 地图与搜索服务识别

- **百度地图相关请求**  
  匹配：`api|ps|sv|offnavi|newvector|ulog.imap|newloc(.map|).(baidu|n.shifen).com`

- **360 / 搜狗搜索识别**  
  匹配：`(.+.|^)(360|so).(cn|com)`

## 2. 邮件协议与一次性邮箱识别

- **SMTP邮件协议识别**  
  匹配：`Subject|HELO|SMTP`

- **一次性邮箱平台识别**  
  匹配：`(@)(guerrillamail|sharklasers|spam4|pokemail|bccto|chacuo|...).(info|com|org|...)`

## 3. 下载与P2P行为识别

- **BitTorrent下载行为识别**  
  匹配：`torrent|peer_id=|info_hash|get_peers|find_node|BitTorrent|announce_peer|announce.php?passkey=`

- **迅雷相关识别**  
  匹配：`xunlei|sandai|Thunder|XLLiveUD`

- **eD2K / 磁力链接识别**  
  匹配：`ed2k|magnet:|bt_key`

## 4. 安全软件识别

- **腾讯电脑管家**  
  匹配：`guanjia.qq.com|qqpcmgr|QQPCMGR`

- **国产杀毒软件**  
  匹配：`rising|kingsoft|duba|xindubawukong|jinshanduba`

## 5. 政治与翻墙网站识别

- **法轮功及相关站点**  
  匹配：`dafahao|minghui|epochtimes|falundafa|zhengjian|ntdtv`

- **政治敏感、举报、民运类网站**  
  匹配：`aboluowang|boxun|chinadigitaltimes|dwnews|12377|secretchina|renminbao|soundofhope|mhradio|inmediahk|epochweekly`

- **翻墙工具与匿名通信项目**  
  匹配：`torproject|netvigator`

## 6. 广告与追踪平台识别

- **国产流量追踪统计平台**  
  匹配：`miaozhen|cnzz|umeng|talkingdata`

## 7. 支付/银行类关键词识别

- **金融支付相关识别**  
  匹配：`visa|mycard|gash|beanfun|bank`

- **与银行相关关键词**  
  匹配：`.bank.`

## 8. 特殊站点识别

- **品葱论坛**  
  匹配：`pincong.rocks`

- **淘宝访问**  
  匹配：`taobao.com`

- **不良内容网站（关键词、短域名等）**  
  匹配：`laomoe|jiyou|ssss|vv1234|868123|ksweb|mm126` 等

- **GitHub Pages 托管机场页面识别**  
  匹配：`flows.pages.dev|miaoko.pages.dev`

