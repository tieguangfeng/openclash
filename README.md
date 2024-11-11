自定OpenClash
```
curl -# -o /etc/config/openclash https://raw.githubusercontent.com/tieguangfeng/openclash/refs/heads/main/openclash.ini
curl -# -o /etc/openclash/custom/openclash_custom_rules.list https://raw.githubusercontent.com/tieguangfeng/openclash/refs/heads/main/custom_rules.list
curl -# -o /etc/openclash/custom/openclash_custom_firewall_rules.sh https://raw.githubusercontent.com/tieguangfeng/openclash/refs/heads/main/firewall_rules.sh
curl -# -o /etc/crontabs/root https://raw.githubusercontent.com/tieguangfeng/openclash/refs/heads/main/crontabs
curl -# -o /www/iptv.txt https://raw.githubusercontent.com/tieguangfeng/openclash/refs/heads/main/iptv.txt
curl -# -o /www/macinstall.html https://raw.githubusercontent.com/tieguangfeng/document/refs/heads/main/macinstall.html
```
更新Meta内核
```
rm -rf /etc/openclash/core/
mkdir /etc/openclash/core/
curl -# -o /etc/openclash/core/clash_meta https://raw.githubusercontent.com/tieguangfeng/openclash/refs/heads/main/clash_meta && chmod 755 /etc/openclash/core/clash_meta
```
定时重启（每周五5点）  
0 5 * * 5 sleep 70 && touch /etc/banner && reboot  
系统重置  
rm -rvf /overlay/*  
