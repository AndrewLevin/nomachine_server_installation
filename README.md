# nomachine_server_installation

```
[amlevin@lxplus043 ~]$ ssh root@amlevin3
[root@amlevin3 ~]# yum install cern-krb5-conf
[root@amlevin3 ~]# yum install pam_krb5
[root@amlevin3 ~]# yum install useraddcern
[root@amlevin3 ~]# cern-get-keytab
[root@amlevin3 ~]# useraddcern amlevin
[root@amlevin3 ~]$ yum install emacs
[root@amlevin3 ~]$ yum group install gnome-desktop
[root@amlevin3 ~]$ rpm -i nomachine_8.11.3_4_x86_64.rpm
[root@amlevin3 ~]$ scp amlevin@lxplus.cern.ch:~/password-auth /etc/pam.d/
[root@amlevin3 ~]$ scp amlevin@lxplus.cern.ch:~/system-auth /etc/pam.d/
[root@amlevin3 ~]$ scp amlevin@lxplus.cern.ch:~/50-cloud-init.conf /etc/ssh/sshd_config.d/
[root@amlevin3 ~]$ service sshd restart
```
