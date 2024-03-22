Here's a summary of the changes: 

1. `router_id`: Ensure that the `router_id `remains unique for this Keepalived instance. 

2. `vrrp_instance VI_1`: 

      • `state`: Set it to `BACKUP` on the slave server. 

      • `interface`: Replace `enp0s3` with the actual network interface name. 

      • `priority`: Set a lower priority (e.g., `50`) than the master server. 

      • `virtual_ipaddress`: Use the same virtual IP address (`192.168.1.101`) as on the master server. 

      • `auth_pass`: Replace `keepalived_password` with your actual authentication password. 

Remember to apply these changes consistently across all servers participating in the Keepalived setup. If you encounter any issues, feel free to ask for further assistance! 🛠️ 