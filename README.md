# ansible-project



### shadowsocks部署


```bash
sudo vi /etc/ssh/sshd_config
PasswordAuthentication yes
sudo systemctl restart sshd

sudo passwd levonfly
vi /etc/sudoers

ansible-playbook -i hosts sites/shadowsocks.yml -b -u levonfly -K -k
```
