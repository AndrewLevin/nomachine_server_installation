# nomachine_server_installation

```
[amlevin@lxplus043 ~]$ ssh root@amlevin3
[root@amlevin3 ~]# yum install cern-krb5-conf
[root@amlevin3 ~]# yum install useraddcern
[root@amlevin3 ~]# cern-get-keytab
[root@amlevin3 ~]# useraddcern amlevin
[root@amlevin3 ~]# mkdir /home/amlevin/
[root@amlevin3 ~]# usermod -d /home/amlevin -s /bin/bash amlevin
[root@amlevin3 ~]# chown amlevin: /home/amlevin/
[root@amlevin3 ~]# chmod go-rx /home/amlevin/
[root@amlevin3 ~]# sudo -u amlevin cp /etc/skel/.bashrc /home/amlevin/
[root@amlevin3 ~]# sudo -u amlevin cp /etc/skel/.bash_profile /home/amlevin/
[root@amlevin3 ~]# sudo -u amlevin cp /etc/skel/.bash_logout /home/amlevin/
[root@amlevin3 ~]# exit
[amlevin@lxplus043 ~]$ ssh amlevin3       
[amlevin@amlevin3 ~]$ sudo yum install emacs
[amlevin@amlevin3 ~]$ sudo yum group install "GNOME Desktop"
[amlevin@amlevin3 ~]$ sudo rpm -i nomachine_6.4.6_1_x86_64.rpm
```
