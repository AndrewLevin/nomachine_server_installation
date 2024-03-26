# nomachine_server_installation

```
[amlevin@lxplus9106 ~]$ ssh root@amlevin1
[root@amlevin1 ~]# yum install cern-krb5-conf
[root@amlevin1 ~]# yum install pam_krb5
[root@amlevin1 ~]# yum install useraddcern
[root@amlevin1 ~]# cern-get-keytab
[root@amlevin1 ~]# useraddcern amlevin
[root@amlevin1 ~]$ yum install emacs
[root@amlevin1 ~]$ yum group install gnome-desktop
[root@amlevin1 ~]$ rpm -i nomachine_8.11.3_4_x86_64.rpm
[root@amlevin1 ~]$ scp amlevin@lxplus.cern.ch:~/password-auth /etc/pam.d/
[root@amlevin1 ~]$ scp amlevin@lxplus.cern.ch:~/system-auth /etc/pam.d/
[root@amlevin1 ~]$ scp amlevin@lxplus.cern.ch:~/50-cloud-init.conf /etc/ssh/sshd_config.d/
[root@amlevin1 ~]$ service sshd restart
```
