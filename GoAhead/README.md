[GoAhead v3.1.3源码](https://gitee.com/mirrors/GoAhead/tree/v3.1.3)

[配置参考](https://www.cnblogs.com/zgq0/p/7511898.html)

[Exploits](https://www.exploit-db.com/exploits/31915)

```sh
cd GoAhead
make # 不用bit
cp test/auth.txt test/route.txt linux-x64-default/bin
cd linux-x64-default/bin
./goahead -v ../../doc 'http://*:8887' #可远程访问

python exploit.py 127.0.0.1 8887 # 触发segmentation fault
```
