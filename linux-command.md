- 1. 解压RPM包
> rpm2cpio kernel-4.14.0-49.el7.centos.x86_64.rpm | cpio -div

- 2. 故意让系统崩溃（其他用法查/proc/sysrq-trigger）
> echo "c" > /proc/sysrq-trigger
