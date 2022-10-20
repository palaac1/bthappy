# bthappy
#宝塔面板7.7原版第三方存档
纯原版1：curl -sSO https://raw.githubusercontent.com/zhucaidan/btpanel-v7.7.0/main/install/install_panel.sh && bash install_panel.sh
纯原版2：wget -O install.sh http://f.cccyun.cc/bt/install_6.0.sh && bash install.sh
升级(降级)到7.7命令： curl http://f.cccyun.cc/bt/update6.sh|bash

<!--宝塔7.7原版一键开心脚本-->
curl -sSO https://raw.githubusercontent.com/ztkink/bthappy/main/one_key_happy.sh && bash one_key_happy.sh

<!--手动解锁宝塔所有付费插件为永不过期-->
文件路径：www/server/panel/data/plugin.json
搜索字符串："endtime": -1 全部替换为 "endtime": 999999999999
<!--手动阻止解锁插件后自动修复为免费版-->
chattr +i /www/server/panel/data/plugin.json

# 宝塔linux工具箱优化脚本
一键修改宝塔面板模板、去除强制登陆、一键修复面板、一键更换yum源、清除系统垃圾缓存、系统优化等
https://gitee.com/gacjie/btpanel_tools
wget -O btpanel_tools.sh https://download.btpanel.cm/tools/btpanel_tools.sh && bash btpanel_tools.sh

#宝塔面板一键优化补丁 -彩虹
1.去除宝塔面板强制绑定账号
2.去除各种删除操作时的计算题与延时等待
3.去除创建网站自动创建的垃圾文件（index.html、404.html、.htaccess）
4.关闭未绑定域名提示页面，防止有人访问未绑定域名直接看出来是用的宝塔面板
5.关闭活动推荐与在线客服
6.去除自动校验文件与上报信息定时任务
7.去除面板日志与网站绑定域名上报
适用7.7版本：wget -O optimize.sh http://f.cccyun.cc/bt/optimize.sh && bash optimize.sh
适用7.9版本：wget -O optimize.sh http://f.cccyun.cc/bt/optimize_new.sh && bash optimize.sh
