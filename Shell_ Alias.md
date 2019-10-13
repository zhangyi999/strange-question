# 使用 Alias 配置 mac 全局命令

这个比较常用。

mac 一般使用bash作为默认shell

Mac系统的环境变量，加载顺序为：
/etc/profile /etc/paths ~/.bash_profile ~/.bash_login ~/.profile ~/.bashrc

当然/etc/profile和/etc/paths是系统级别的，系统启动就会加载，后面几个是当前用户级的环境变量。后面3个按照从前往后的顺序读取，如果~/.bash_profile文件存在，则后面的几个文件就会被忽略不读了，如果~/.bash_profile文件不存在，才会以此类推读取后面的文件。

```bash
$ cd ~
```

```bash
$ vim .bash_profile
```

```bash
$ alias cdtaoke='cd ~/code/taoke/taoke'
```

```bash
$ source .bash_profile
```