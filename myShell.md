- 1. 获取内核进程堆栈

```bash
#!/bin/bash
ps -eo comm,pid | grep nfsd | awk '{print $NF}' | while read pid; do
echo ===pid:$pid:`cat /proc/$pid/comm`
cat /proc/$pid/stack
done
```
