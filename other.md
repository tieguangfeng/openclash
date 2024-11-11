##恢复默认后，不确定参数
option update '0'
 
 option enable_rule_proxy '0'	##启用规则代理
option rule_source '0' 		##规则来源
option other_rule_auto_update '0'##其他规则自动更新

option servers_if_update '0'	##像插件设置-DNS设置
option servers_update '0' 	##像插件设置-DNS设置
	
option redirect_dns '0'		##默认是0，启动后是1
option cachesize_dns '0'	##默认是0，启动后是1

option stream_auto_select '0'	##翻译，流自动选择
===fake-ip模式===
option operation_mode 'fake-ip'
option en_mode 'fake-ip-mix'
===redir-host模式===
option operation_mode 'redir-host'
option en_mode 'redir-host-mix'
##覆写设置-DNS设置（fake-ip）
option fakeip_range '198.18.0.1/16'	##Fake-IP地址范围
option store_fakeip '1'			##Fake-IP持久化
option custom_fakeip_filter '1'		##Fake-IP-Filter
option custom_fakeip_filter_mode 'blacklist'	##Fake-IP-Filter-Mode
option filter_aaaa_dns '0'		##不知道
