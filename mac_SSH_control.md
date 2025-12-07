# SSH远程开发(mac)

本次实训过程中，有些同学使用mac进行学习。在硬件上相较于Windows和Linux有一定差距。在面对陌生的操作系统时，会感到不习惯。SSH(secure server)能够很好地应对接下来的工作，提升学习效率。
__利用SSH可以在mac操作系统的终端和VS code界面进行开发，提升使用手感__

## 步骤

1. 在ubuntu系统安装ssh-server

__更新安装包列表__
```

sudo apt update 
```

__安装ssh-server__
```

sudo apt install openssh-server
```

2. 设置SSH开机自启

__检查SSH服务状态，看到__
active (running)
就可以了
```

sudo apt install openssh-server

如果不是
sudo systemctl start ssh
```

__启动__
```

sudo systemctl enable ssh
```

3. 切换网络设置

- [ ] 关闭虚拟机

- [ ] 打开设置

- [ ] 选择网络

- [ ] 将共享网络换成桥接（高级）

- [ ] 选择选项带有en0的

4. 确定ubuntu用户名以及IP地址

__在ubuntu确认用户名__
```

whoami
```

__确认IP地址__
```

hostname -I
```

5. 在mac终端上连接SSH


```

ssh <ubuntu用户名>@IP地址
```
