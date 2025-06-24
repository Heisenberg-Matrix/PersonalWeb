sys
#
aaa
 local-user jump-it password cipher BKcs^2^5!1#3
 local-user jump-it privilege level 1
 local-user jump-it service-type ssh
#
ssh user jump-it authentication-type password
ssh user jump-it service-type stelnet
stelnet server enable
user-interface vty 0 4  
authentication-mode aaa 
protocol inbound ssh 
ssh client first-time enable