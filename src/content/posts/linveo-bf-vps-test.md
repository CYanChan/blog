---
title: Linveo黑五vps融合怪测试
published: 2025-12-07
description: 今年没新鸡，干脆把去年的德克萨斯续了，再跑一次测试
tags:
  - VPS
  - Test
category: VPS
draft: false
---
探针：[L1nuors - Komari Monitor](https://status.linuors.com/instance/981e7614-020c-406f-8ce7-3435be054d67)    
数据还不错，年付也才25刀，9950X这个价格可以接受    
[购买地址](https://billing.linveo.com/order/main/packages/vps/?group_id=10)
```
测评频道: https://t.me/+UHVoo2U4VyA5NTQ1                    
VPS融合怪版本：2025.11.29
Shell项目地址：https://github.com/spiritLHLS/ecs
Go项目地址 [推荐]：https://github.com/oneclickvirt/ecs
---------------------基础信息查询--感谢所有开源项目----------------------
NAT Type being detected ......
 CPU 型号          : AMD Ryzen 9 9950X 16-Core Processor
 CPU 核心数        : 2
 CPU 频率          : 4291.932 MHz
 CPU 缓存          : L1: 96.00 KB / L2: 2.00 MB / L3: 128.00 MB
 AES-NI指令集      : ✔ Enabled
 VM-x/AMD-V支持    : ✔ Enabled
 内存              : 683.93 MiB / 1.90 GiB
 Swap              : 0 KiB / 1.00 GiB
 硬盘空间          : 5.13 GiB / 48.91 GiB
 启动盘路径        : /dev/vda1
 系统在线时间      : 5 days, 2 hour 13 min
 负载              : 0.05, 0.01, 0.00
 系统              : Debian GNU/Linux 12 (bookworm) (x86_64)
 架构              : x86_64 (64 Bit)
 内核              : 6.1.0-39-cloud-amd64
 TCP加速方式       : cubic
 虚拟化架构        : KVM
 IPV4 ASN          : AS62564 LINVEO, LLC
 IPV4 位置         : Dallas / Texas / US
 IPV6 ASN          : AS62564 LINVEO-LLC
 IPV6 位置         : United States
 IPV6 子网掩码     : 64
------------------------CPU测试--通过sysbench测试-------------------------
 -> CPU 测试中 (Fast Mode, 1-Pass @ 5sec)
 1 线程测试(单核)得分: 		6706 Scores
 2 线程测试(多核)得分: 		13408 Scores
--------------------内存测试--感谢lemonbench开源----------------------------
 -> 内存测试 Test (Fast Mode, 1-Pass @ 5sec)
 单线程读测试:		103078.02 MB/s
 单线程写测试:		39743.11 MB/s
--------------------磁盘dd读写测试--感谢lemonbench开源--------------------
 -> 磁盘IO测试中 (4K Block/1M Block, Direct Mode)
 测试操作		写速度					读速度
 100MB-4K Block		51.7 MB/s (12.62 IOPS, 2.03s)		41.6 MB/s (10159 IOPS, 2.52s)
 1GB-1M Block		3.4 GB/s (3287 IOPS, 0.30s)		3.1 GB/s (2998 IOPS, 0.33s)
----------------------磁盘fio读写测试--感谢yabs开源-----------------------
Block Size | 4k            (IOPS) | 64k           (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 245.12 MB/s  (61.2k) | 1.36 GB/s    (21.3k)
Write      | 245.77 MB/s  (61.4k) | 1.37 GB/s    (21.4k)
Total      | 490.90 MB/s (122.7k) | 2.73 GB/s    (42.7k)
           |                      |                     
Block Size | 512k          (IOPS) | 1m            (IOPS)
  ------   | ---            ----  | ----           ---- 
Read       | 2.80 GB/s     (5.4k) | 3.32 GB/s     (3.2k)
Write      | 2.95 GB/s     (5.7k) | 3.54 GB/s     (3.4k)
Total      | 5.75 GB/s    (11.2k) | 6.87 GB/s     (6.7k)
正在并发测试中，大概2~3分钟无输出，请耐心等待。。。
---------------流媒体解锁--感谢oneclickvirt/UnlockTests测试----------------
测试时间:  2025-12-07 10:20:39
IPV4:
============[ 跨国平台 ]============
Apple                     YES (Region: USA)
BingSearch                YES (Region: US)
Claude                    YES
Dazn                      YES (Region: US)
Disney+                   NO (forbidden-location)
Gemini                    YES (Region: US)
GoogleSearch              YES
Google Play Store         YES (Region: US)
IQiYi                     YES (Region: US)
Instagram Licensed Audio  YES
KOCOWA                    YES
MetaAI                    YES (Region: US)
Netflix                   NO
Netflix CDN               NO (Main Service Unavailable) (Region: US)
OneTrust                  YES (Region: US TEXAS)
ChatGPT                   YES (Region: US)
Paramount+                YES
Amazon Prime Video        YES (Region: US)
Reddit                    YES
SonyLiv                   YES (Region: US)
Sora                      YES (Region: US)
Spotify Registration      NO
Steam Store               YES (Community Available) (Region: US)
TVBAnywhere+              YES (Region: US)
TikTok                    YES (Region: US)
Viu.com                   YES
Wikipedia Editability     YES
YouTube Region            YES
YouTube CDN               DFW
IPV6:
============[ 跨国平台 ]============
Apple                     YES (Region: USA)
BingSearch                YES (Region: US)
Claude                    YES
Dazn                      N/A (No IPv6 Support)
Disney+                   NO (forbidden-location)
Gemini                    YES (Region: US)
GoogleSearch              YES
Google Play Store         YES (Region: US)
IQiYi                     N/A (No IPv6 Support)
Instagram Licensed Audio  YES
KOCOWA                    N/A (No IPv6 Support)
MetaAI                    YES (Region: US)
Netflix                   NO
Netflix CDN               NO (Main Service Unavailable) (Region: US)
OneTrust                  YES (Region: US TEXAS)
ChatGPT                   Unknown
Paramount+                YES
Amazon Prime Video        N/A (No IPv6 Support)
Reddit                    Failed (Network Connection Failed)
SonyLiv                   YES (Region: US)
Sora                      YES (Region: US)
Spotify Registration      NO
Steam Store               Failed (Network Connection Failed)
TVBAnywhere+              N/A (No IPv6 Support)
TikTok                    N/A (No IPv6 Support)
Viu.com                   N/A (No IPv6 Support)
Wikipedia Editability     YES
YouTube Region            YES
YouTube CDN               DFW
---------------------TikTok解锁--感谢lmc999的源脚本---------------------
 Tiktok Region:		【US】
-------------IP质量检测--基于oneclickvirt/securityCheck使用--------------
数据仅作参考，不代表100%准确，如果和实际情况不一致请手动查询多个数据库比对
以下为各数据库编号，输出结果后将自带数据库来源对应的编号
ipinfo数据库  [0] | scamalytics数据库 [1] | virustotal数据库   [2] | abuseipdb数据库   [3] | ip2location数据库    [4]
ip-api数据库  [5] | ipwhois数据库     [6] | ipregistry数据库   [7] | ipdata数据库      [8] | db-ip数据库          [9]
ipapiis数据库 [A] | ipapicom数据库    [B] | bigdatacloud数据库 [C] | dkly数据库        [D] | ipqualityscore数据库 [E]
ipintel数据库 [F] | ipfighter数据库   [G] | fraudlogix数据库   [H] | cloudflare数据库  [I] |
IPV4:
安全得分:
信任得分(越高越好): 1 [8]
VPN得分(越低越好): 100 [8] 
代理得分(越低越好): 99 [8] 
社区投票-无害: 0 [2] 
社区投票-恶意: 0 [2] 
威胁得分(越低越好): 97 [8] 
欺诈得分(越低越好): 0 [E] 
滥用得分(越低越好): 0 [3] 
ASN滥用得分(越低越好): 0.0082 (Low) [A] 
公司滥用得分(越低越好): 0 (Very Low) [A] 
威胁级别: low [9] 
流量占比: 真人(越高越好)42% [I] 机器人(越低越好)57% [I]
黑名单记录统计:(有多少黑名单网站有记录):
无害记录数: 0 [2]  恶意记录数: 0 [2]  可疑记录数: 0 [2]  无记录数: 95 [2] 
安全信息:
使用类型: hosting [0 3 7 9 C] business [8 A]
公司类型: hosting [0 7 A] 
浏览器类型: 主流90% 其他9% [I] 
设备类型: 桌面91% 移动8% 其他0% [I] 
操作系统类型: 主流91% 其他8% [I] 
是否云提供商: Yes [7] 
是否数据中心: Yes [0 A C] No [5 6 8 G]
是否移动设备: Yes [E] No [5 A C G]
是否代理: No [0 4 5 6 7 8 9 A C E] Yes [G]
是否VPN: No [0 6 7 A C E G] 
是否TorExit: No [7] 
是否Tor出口: No [7] 
是否网络爬虫: No [9 A E] 
是否匿名: No [6 7 8] 
是否攻击者: No [7 8] 
是否滥用者: No [7 8 A C E] 
是否威胁: No [7 8 C] 
是否中继: No [0 7 8 C] 
是否Bogon: No [7 8 A C] 
是否机器人: No [E] 
DNS-黑名单: 314(Total_Check) 0(Clean) 0(Blacklisted) 0(Other) 
IPV6:
安全得分:
滥用得分(越低越好): 0 [3] 
ASN滥用得分(越低越好): 0.0082 (Low) [A] 
公司滥用得分(越低越好): 0 (Very Low) [A] 
流量占比: 真人(越高越好)42% [I] 机器人(越低越好)57% [I]
安全信息:
使用类型: hosting [3] business [A]
公司类型: hosting [A] 
浏览器类型: 主流90% 其他9% [I] 
设备类型: 桌面91% 移动8% 其他0% [I] 
操作系统类型: 主流91% 其他8% [I] 
是否数据中心: Yes [A] No [G]
是否移动设备: No [A G] 
是否代理: No [A] Yes [G]
是否VPN: No [A G] 
是否Tor: No [3 A] 
是否网络爬虫: No [A] 
是否滥用者: No [A] 
是否Bogon: No [A] 
DNS-黑名单: 314(Total_Check) 0(Clean) 0(Blacklisted) 314(Other) 
Google搜索可行性：NO
------------邮件端口检测--基于oneclickvirt/portchecker开源------------
Platform  SMTP  SMTPS POP3  POP3S IMAP  IMAPS
LocalPort ✔     ✔     ✔     ✔     ✔     ✔    
QQ        ✘     ✘     ✔     ✘     ✔     ✘    
163       ✘     ✘     ✔     ✘     ✔     ✘    
Sohu      ✘     ✘     ✔     ✘     ✔     ✘    
Yandex    ✘     ✘     ✔     ✘     ✔     ✘    
Gmail     ✘     ✘     ✘     ✘     ✘     ✘    
Outlook   ✘     ✘     ✔     ✘     ✔     ✘    
Office365 ✘     ✘     ✔     ✘     ✔     ✘    
Yahoo     ✘     ✘     ✘     ✘     ✘     ✘    
MailCOM   ✘     ✘     ✔     ✘     ✔     ✘    
MailRU    ✘     ✘     ✘     ✘     ✔     ✘    
AOL       ✘     ✘     ✘     ✘     ✘     ✘    
GMX       ✘     ✘     ✔     ✘     ✔     ✘    
Sina      ✘     ✘     ✔     ✘     ✔     ✘    
Apple     ✘     ✘     ✘     ✘     ✘     ✘    
FastMail  ✘     ✘     ✘     ✘     ✘     ✘    
ProtonMail✘     ✘     ✘     ✘     ✘     ✘    
MXRoute   ✘     ✘     ✔     ✘     ✔     ✘    
Namecrane ✘     ✘     ✔     ✘     ✔     ✘    
XYAMail   ✘     ✘     ✘     ✘     ✘     ✘    
ZohoMail  ✘     ✘     ✘     ✘     ✘     ✘    
Inbox_eu  ✘     ✘     ✔     ✘     ✘     ✘    
Free_fr   ✘     ✘     ✔     ✘     ✔     ✘    
-------------上游及三网回程--基于oneclickvirt/backtrace开源--------------
国家: US 城市: Dallas 服务商: AS62564 LINVEO, LLC
     AS400402          AS397423          AS40676      
 Hosting Bot, LLC Tier.Net Technolog Psychz Networks  
      Direct           Indirect          Indirect     
北京电信v4 219.141.140.10           电信163    [普通线路] 
北京联通v4 202.106.195.68           联通4837   [普通线路] 
北京移动v4 221.179.155.161          移动CMI    [普通线路] 
上海电信v4 202.96.209.133           电信163    [普通线路] 
上海联通v4 210.22.97.1              联通4837   [普通线路] 
上海移动v4 211.136.112.200          移动CMI    [普通线路] 
广州电信v4 58.60.188.222            电信163    [普通线路] 
广州联通v4 210.21.196.6             联通4837   [普通线路] 
广州移动v4 120.196.165.24           移动CMI    [普通线路] 
成都电信v4 61.139.2.69              电信163    [普通线路] 
成都联通v4 119.6.6.6                联通4837   [普通线路] 
成都移动v4 211.137.96.205           移动CMI    [普通线路] 
北京电信v6 2400:89c0:1053:3::69     电信163    [普通线路] 
北京联通v6 2400:89c0:1013:3::54     检测不到回程路由节点的IPV6地址
北京移动v6 2409:8c00:8421:1303::55  移动CMI    [普通线路] 移动CMIN2  [精品线路] 
上海电信v6 240e:e1:aa00:4000::24    电信163    [普通线路] 
上海联通v6 2408:80f1:21:5003::a     联通4837   [普通线路] 
上海移动v6 2409:8c1e:75b0:3003::26  移动CMI    [普通线路] 
广州电信v6 240e:97c:2f:3000::44     电信163    [普通线路] 
广州联通v6 2408:8756:f50:1001::c    联通4837   [普通线路] 
广州移动v6 2409:8c54:871:1001::12   移动CMI    [普通线路] 
准确线路自行查看详细路由，本测试结果仅作参考
同一目标地址多个线路时，检测可能已越过汇聚层，除第一个线路外，后续信息可能无效
----------------------回程路由--基于nexttrace开源-----------------------
依次测试电信/联通/移动经过的地区及线路，核心程序来自nexttrace，请知悉!
广州电信 58.60.188.222
0.29 ms 	AS62564 美国 亚利桑那州 凤凰城 Bunny Communications
0.18 ms 	AS400402 美国 德克萨斯 达拉斯 hostingbot.net
0.92 ms 	AS397423 美国 德克萨斯州 达拉斯 tier.net
0.48 ms 	* RFC1918
0.75 ms 	AS3257 美国 德克萨斯 达拉斯 gtt.net
28.70 ms 	AS3257 美国 弗吉尼亚州 狼阱 gtt.net
41.45 ms 	AS3257 [TINET-TINET] 美国 弗吉尼亚州 郡戴维森 gtt.net
74.06 ms 	AS4134 [CHINANET-BB] 美国 加利福尼亚 圣何塞 chinatelecom.com.cn 电信
217.33 ms 	AS4134 [CHINANET-BB] 中国 广东 广州 X-I chinatelecom.com.cn 电信
220.98 ms 	AS4134 [CHINANET-BB] 中国 广东 广州 chinatelecom.com.cn
广州联通 210.21.196.6
0.60 ms 	AS62564 美国 亚利桑那州 凤凰城 Bunny Communications
0.21 ms 	AS400402 美国 德克萨斯 达拉斯 hostingbot.net
0.81 ms 	AS397423 美国 德克萨斯州 达拉斯 tier.net
16.72 ms 	AS3356 美国 德克萨斯 达拉斯 lumen.com
32.91 ms 	AS3356 美国 加利福尼亚 洛杉矶 lumen.com
56.59 ms 	AS3356 美国 加利福尼亚 圣何塞 Level3-CU-Peer lumen.com
261.17 ms 	AS4837 [CU169-BACKBONE] 中国 广东 广州 chinaunicom.cn 联通
237.11 ms 	AS4837 [CU169-BACKBONE] 中国 广东 广州 X-I chinaunicom.cn 联通
253.42 ms 	AS17816 [APNIC-AP] 中国 广东 深圳 中国联通 联通
242.11 ms 	AS17623 [APNIC-AP] 中国 广东 深圳 chinaunicom.cn 联通
238.38 ms 	AS17623 中国 广东 深圳 宝安区 chinaunicom.cn 联通
广州移动 120.196.165.24
0.20 ms 	AS62564 美国 亚利桑那州 凤凰城 Bunny Communications
0.20 ms 	AS400402 美国 德克萨斯 达拉斯 hostingbot.net
0.78 ms 	AS397423 美国 德克萨斯州 达拉斯 tier.net
17.42 ms 	AS3356 美国 德克萨斯 达拉斯 lumen.com
115.57 ms 	AS3356 德国 黑森 美因河畔法兰克福 lumen.com
117.32 ms 	AS58453 [CMI-INT] 德国 黑森 美茵河畔法兰克福 cmi.chinamobile.com 移动
283.14 ms 	AS9808 [CMNET] 中国 广东 广州 X-I chinamobileltd.com 移动
287.03 ms 	AS9808 [CMNET] 中国 广东 广州 I-C chinamobileltd.com 移动
291.15 ms 	AS9808 [CMNET] 中国 广东 广州 chinamobileltd.com 移动
290.03 ms 	AS9808 [CMNET] 中国 广东 广州 chinamobileltd.com 移动
289.86 ms 	AS56040 [APNIC-AP] 中国 广东 深圳 gd.10086.cn 移动
---------------------自动更新测速节点列表--本脚本原创----------------------
位置		 上传速度	 下载速度	 延迟
Speedtest.net	 2734.93Mbps	 7681.71Mbps	 898.93ms	
法兰克福	 103.97Mbps	 266.55Mbps	 114.67ms	
中国香港	 91.75Mbps	 126.12Mbps	 170.12ms	
联通上海5G	 0.43Mbps	 34.25Mbps	 355.43ms	
电信Suzhou5G	 4.10Mbps	 56.87Mbps	 205.05ms	
电信浙江	 11.24Mbps	 68.06Mbps	 232.62ms	
------------------------------------------------------------------------
 总共花费      : 4 分 29 秒
 时间          : Sun Dec  7 10:23:52 CST 2025
------------------------------------------------------------------------
```