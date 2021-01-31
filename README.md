#备份

# Quantumult X小白配置 制作 by Orz-3 TG频道：t.me/Orzmini 2020/12/24更新

[general]
server_check_url=http://bing.com/
dns_exclusion_list=*.cmpassport.com, *.jegotrip.com.cn, *.icitymobile.mobi, id6.me, *.icitymobile.mobi, *.pingan.com.cn, *.cmbchina.com, *.localnetwork.uop, mfs.ykimg.com*.ttf
geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://raw.githubusercontent.com/Orz-3/QuantumultX/master/IP.js
resource_parser_url=https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/resource-parser.js
profile_img_url=https://raw.githubusercontent.com/Orz-3/mini/none/qikuo.png

[dns]
no-ipv6
server=119.29.29.29
address=/mtalk.google.com/108.177.125.188

[policy]
static=新加坡, server-tag-regex=(?=.*(新加坡|狮城|SG|(?i)Singapore))^((?!(专线|手游|游戏|(?i)IPLC|IEPL|game)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/SG.png
static=美国, server-tag-regex=(?=.*(美国|美國|US|(?i)States|American))^((?!(专线|手游|游戏|(?i)IPLC|IEPL|game)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/US.png
static=日本, server-tag-regex=(?=.*(日本|JP|(?i)Japan))^((?!(专线|手游|游戏|(?i)IPLC|IEPL|game)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/JP.png
static=韩国, server-tag-regex=(?=.*(韩国|韓國|南朝鲜|KR|(?i)Korean))^((?!(专线|手游|游戏|(?i)IPLC|IEPL|game)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/KR.png
static=香港, server-tag-regex=(?=.*(香港|HK|(?i)Hong))^((?!(专线|手游|游戏|(?i)IPLC|IEPL|game)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/HK.png
static=台湾, server-tag-regex=(?=.*(台湾|台灣|TW|(?i)Taiwan))^((?!(专线|手游|游戏|(?i)IPLC|IEPL|game)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/TW.png
static=特殊, server-tag-regex=^((?!(专线|手游|游戏|香港|台湾|日本|新加坡|美国|韩国|狮城|南朝鲜|US|SG|JP|KR|HK|TW|台灣|美國|韓國|獅城|账号|试用|流量|电报|网址|最新|域名|剩余|(?i)IPLC|IEPL|game|States|American|Singapore|Japan|Korea|Hong|Taiwan|data|date|website)).)*$, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/UN.png
static=IPLC, server-tag-regex=(手游|游戏|专线|(?i)IPLC|IEPL|game), img-url=https://raw.githubusercontent.com/Orz-3/mini/master/IPLC.png
static=苹果服务, direct, 美国, 香港, proxy, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Apple.png
static=全球加速, proxy, 美国, 新加坡, 日本, 韩国, 香港, 台湾, 特殊, IPLC, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Global.png
static=港台番剧, direct, 香港, 台湾, proxy, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/StreamingSE.png
static=国际媒体, proxy, 美国, 新加坡, 日本, 韩国, 香港, 台湾, 特殊, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Streaming.png
static=声田音乐, proxy, 美国, 香港, 日本, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Spotify.png
static=网飞影视, proxy, 新加坡, 香港, 台湾, direct, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Netflix.png
static=电报代理, proxy, direct, 新加坡, IPLC, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Telegram.png
static=黑白名单, proxy, direct, 美国, 新加坡, 日本, 韩国, 香港, 台湾, 特殊, IPLC, img-url=https://raw.githubusercontent.com/Orz-3/mini/master/Final.png

[server_remote]
https://subv2.nanoport.xyz/api/v1/client/subscribe?token=019a5364273141735dd4067283203bc6, tag=Nanoport, update-interval=86400, opt-parser=false, enabled=false

[filter_remote]
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Unbreak.list, tag=规则修正, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Guard/Advertising.list, tag=广告拦截, force-policy=reject, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/AdRule.list, tag=广告拦截, force-policy=reject, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Guard/Privacy.list, tag=隐私保护, force-policy=reject, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Guard/Hijacking.list, tag=运营劫持, force-policy=reject, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Extra/Telegram/Telegram.list, tag=电报代理, force-policy=电报代理, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/StreamingMedia/Music/Spotify.list, tag=声田音乐, force-policy=声田音乐, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/StreamingMedia/Video/Netflix.list, tag=网飞影视, force-policy=网飞影视, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/StreamingMedia/Video/TikTok.list, tag=海外抖音, force-policy=国际媒体, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/StreamingMedia/Video/Bahamut.list, tag=动画疯, force-policy=台湾, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/StreamingMedia/Streaming.list, tag=国际媒体, force-policy=国际媒体, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/StreamingMedia/StreamingSE.list, tag=港台番剧, force-policy=港台番剧, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Global.list, tag=全球加速, force-policy=全球加速, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Extra/Apple/AppStoreConnect.list, tag=苹果服务, force-policy=苹果服务, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Extra/Apple/AppStore.list, tag=苹果服务, force-policy=苹果服务, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Extra/Apple/TestFlight.list, tag=苹果服务, force-policy=苹果服务, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/China.list, tag=国内网站, force-policy=direct, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Extra/ChinaIP.list, tag=ChinaIP, update-interval=86400, enabled=true

[rewrite_remote]
https://raw.githubusercontent.com/yichahucha/surge/master/qx_sub.txt, tag=京东比价, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/Semporia/TikTok-Unlock/master/Surge/TiKok-TW.sgmodule, tag=解锁Tiktok, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/script/zhihu/zhihu_plus.qxrewrite, tag=知乎助手_去广告及体验增强, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/script/bilibili/bilibili_plus.qxrewrite, tag=哔哩哔哩_去广告, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/YouTube.conf, tag=YouTube去广告, update-interval=86400, opt-parser=false, enabled=true
https://gitee.com/chavyleung/scripts/raw/master/box/rewrite/boxjs.rewrite.quanx.tf.conf, tag=BoxJS, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/General.conf, tag=神机重定向, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/NobyDa/Script/master/QuantumultX/Rewrite_lhie1.conf, tag=lhie1去广告, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/Block/Advertising.conf, tag=神机去广告, update-interval=86400, opt-parser=false, enabled=false
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Rewrite/Unlock/TikTokTW.conf, tag=解锁Tiktok, update-interval=86400, opt-parser=false, enabled=false
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/JS_GetCookie.conf, tag=Cookie, update-interval=86400, opt-parser=false, enabled=false
https://raw.githubusercontent.com/Orz-3/QuantumultX/master/JS.conf, tag=Script, update-interval=86400, opt-parser=false, enabled=false

[server_local]
shadowsocks=2.58.241.43:38033, method=aes-256-gcm, password=xpQwyV4W5FdA6NMANJJx73US, fast-open=false, udp-relay=false, tag=1611557685.046616


[filter_local]
# 知乎去广告
DOMAIN,118.89.204.198,REJECT
DOMAIN-KEYWORD,118.89.204.198,REJECT
IP-CIDR,118.89.204.198/32,REJECT
DOMAIN,appcloud2.in.zhihu.com,REJECT
USER-AGENT,AVOS*,REJECT
host-suffix, local, direct
ip-cidr, 192.168.0.0/16, direct
ip-cidr, 10.0.0.0/8, direct
ip-cidr, 172.16.0.0/12, direct
ip-cidr, 127.0.0.0/8, direct
ip-cidr, 100.64.0.0/10, direct
ip-cidr, 224.0.0.0/4, direct
ip6-cidr, fe80::/10, direct
-geoip, cn, direct
final, 黑白名单

[rewrite_local]

[task_local]
5 0 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jx_sign.js, tag=京喜, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jx_sign.png, enabled=true
#5G狂欢城
0 0,6,12,18 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_5g.js, tag=5G狂欢城, img-url=https://raw.githubusercontent.com/Orz-3/task/master/jd.png, enabled=true
#小鸽有礼2
30 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_xgyl.js, tag=小鸽有礼2, img-url=https://raw.githubusercontent.com/58xinian/icon/master/jd_xgyl.png, enabled=true
20 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_super_box.js, tag=京东超级盒子, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_super_box.png, enabled=true
0 0,9,11,13,15,17,19,20,21,22,23 * * * https://raw.githubusercontent.com/Tartarus2014/Script/master/jd_live_redrain_offical.js, tag=官方号直播红包雨, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_live_redrain_offical.png, enabled=true
0 0,9,11,13,15,17,19,20,21,23 3,5,20-30/1 1,2 * https://raw.githubusercontent.com/Tartarus2014/Script/master/jd_live_redrain_nian.js, tag=年货直播红包雨, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_live_redrain_nian.png, enabled=true
30,31 12-23/1 * * * https://raw.githubusercontent.com/Tartarus2014/Script/master/jd_live_redrain_half.js, tag=半点红包雨, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_live_redrain_half.png, enabled=true
0,1 19-21/1 * * * https://raw.githubusercontent.com/Tartarus2014/Script/master/jd_live_redrain2.js, tag=直播间红包雨, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_live_redrain2.png, enabled=true
30,31 20-23/1 * * * https://raw.githubusercontent.com/Tartarus2014/Script/master/jd_live_redrain.js, tag=超级直播间红包雨, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_live_redrain.png, enabled=true
0 * * * * https://raw.githubusercontent.com/moposmall/Script/main/Me/jx_cfd.js, tag=京喜财富岛, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jx_cfd.png, enabled=true
30 6,12,22 * * * https://raw.githubusercontent.com/moposmall/Script/main/Me/jx_cfd_exchange.js, tag=京喜财富岛兑换提醒, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jx_cfd_exchange.png, enabled=true
20 7 * * * https://gitee.com/lxk0301/jd_scripts/blob/master/jd_super_box.js, tag=京东超级盒子, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_super_box.png, enabled=true
15 0 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_festival.js, tag=京东手机年终奖, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_festival.png, enabled=true
11 1 * * * https://raw.githubusercontent.com/yangtingxiao/QuantumultX/master/scripts/jd/jd_lotteryMachine.js, tag=抽奖机, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_lotteryMachine.png, enabled=true
11 9 * * * https://raw.githubusercontent.com/yangtingxiao/QuantumultX/master/scripts/jd/jd_rankingList.js, tag=排行榜, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_rankingList.png, enabled=true
1 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_mh.js, tag=盲盒抽京豆, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_mh.png, enabled=true
10 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_ms.js, tag=京东秒秒币, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_ms.png, enabled=true
5 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_xg.js, tag=小鸽有礼, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_xg.png, enabled=true
20 8 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_sgmh.js, tag=闪购盲盒, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_sgmh.png, enabled=true
20 8 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_immortal_answer.js, tag=神仙书院答题, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_immortal_answer.png, enabled=true
0 8 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_immortal.js, tag=京东神仙书院, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_immortal.png, enabled=true
50 8 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_nian_wechat.js, tag=炸年兽小程序, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_nian_wechat.png, enabled=true
30 8 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_nian_sign.js, tag=炸年兽签到任务, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_nian_sign.png, enabled=true
0 9 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_nian_ar.js, tag=炸年兽AR, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_nian_ar.png, enabled=true
20 * * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_nianCollect.js, tag=炸年兽收爆竹, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_nianCollect.png, enabled=true
0 8,9,10 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_nian.js, tag=京东炸年兽, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_nian.png, enabled=true
1 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_nh.js, tag=京东年货节, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_nh.png, enabled=true
0 2 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_cash.js, tag=签到领现金, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_cash.png, enabled=true
1 8,12,18 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_bookshop.js, tag=口袋书店, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_bookshop.png, enabled=true
10 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_crazy_joy.js, tag=CrazyJoy任务, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_crazy_joy.png, enabled=true
10 0 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_kd.js, tag=京东快递签到, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_kd.png, enabled=true
10 7 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_bean_home.js, tag=领京豆额外奖励, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_bean_home.png, enabled=true
10 0,20 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_necklace.js, tag=点点券, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_necklace.png, enabled=true
10 * * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_jdfactory.js, tag=东东工厂, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_jdfactory.png, enabled=true
2 9 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_bean_change.js, tag=京豆变动通知, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_bean_change.png, enabled=true
1 1 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_redPacket.js, tag=京东全民开红包, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_redPacket.png, enabled=true
5 0 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_club_lottery.js, tag=摇京豆, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_club_lottery.png, enabled=true
55 23 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_unsubscribe.js, tag=取关店铺商品, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_unsubscribe.png, enabled=true
10 0 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_shop.js, tag=进店领豆, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_shop.png, enabled=true
0 0 0 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_blueCoin.js, tag=京小超兑换奖品, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_blueCoin.png, enabled=true
11 1-23/5 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_superMarket.js, tag=东东超市, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_superMarket.png, enabled=true
3 */2 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_moneyTree.js, tag=摇钱树, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_moneyTree.png, enabled=true
8 */3 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_speed.js, tag=天天加速, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_speed.png, enabled=true
1 7-21/2 * * * https://gitee.com/lxk0301/jd_scripts/raw/master/jd_plantBean.js, tag=种豆得豆, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/jd_plantBean.png, enabled=true
5 0 * * * https://raw.githubusercontent.com/NobyDa/Script/master/JD-DailyBonus/JD_DailyBonus.js, tag=京东, img-url=https://raw.githubusercontent.com/ChuheGit/1/main/QuantumultX/Gallery/API-Icon/JD_DailyBonus.png, enabled=true


[http_backend]

[mitm]
passphrase = 2A17D9C3
p12 = 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
skip_validating_cert = true

