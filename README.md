![Anurag’s github stats](https://github-readme-stats.vercel.app/api?username=lan-tianxiang&show_icons=true&theme=merko)

## 请仔细阅读 [WIKI](https://github.com/lan-tianxiang/jd_shell/wiki) 和各文件注释，95%的问题都能找到答案

## 适用于以下系统

- ArmBian/Debian/Ubuntu/OpenMediaVault/CentOS/Fedora/RHEL等Linux系统

- OpenWRT(教程划归于Linux)

- Android

- MacOS

- Docker


### 如何部署？

### 1.Linux 一键部署：
内有多个环节选择，可退出！
```shell
curl -O linux_install_jd.sh https://cdn.jsdelivr.net/gh/lan-tianxiang/jd_shell/install_scripts/linux_install_jd.sh && chmod +x linux_install_jd.sh && bash linux_install_jd.sh
```

### 2. Docker 一键部署单个容器：

```shell
curl https://cdn.jsdelivr.net/gh/lan-tianxiang/jd_shell/install_scripts/docker_install_jd.sh && chmod +x docker_install_jd.sh && bash docker_install_jd.sh
```


Linux部署时会有

+----------------- 开 始 执 行 更 新 脚 本 -----------------+

   活动脚本目录：/home/jd/scripts

   当前系统时间：2021-03-22 11:40

+-----------------------------------------------------------+

的提示，记得记住你脚本的目录，Wiki中的命令都需要进入目录中运行才可生效！！！！！！！！！！

以上例来说，则进入目录命令为

```shell
cd /home/jd/
```


## 说明

1. 即将推出远程面板功能，需安装数据库php等，非服务器的用户可以忽略

## 更新日志

> 只记录大的更新，小修小改不记录。

2021-02-19，面板功能集成至jd.sh内，运行jd.sh会出现操作提示

2021-01-23，控制面板增加日志查看功能，Docker重启容器后可以使用`docker restart jd`，非Docker如果是pm2方式的请重启pm2进程`pm2 resatrt server.js`。

2020-01-21，增加shylocks/Loon脚本。

2021-01-15，如果本机上安装了pm2，则挂机程序以pm2启动，否则以nohup启动。
