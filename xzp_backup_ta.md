# flash [G8142-47.1.A.3.254_RU.rar](https://www.androidfilehost.com/?fid=11410932744536993431)

# root xzp by [renosploit](https://forum.xda-developers.com/xperia-xz1-compact/development/devonly-exploits-temp-root-to-backup-t3795510)
```
PS L:\bksony> .\adb.exe push .\renosploit /data/local/tmp
2393 KB/s (609064 bytes in 0.248s)
PS L:\bksony> .\adb.exe push .\renoshell /data/local/tmp
1506 KB/s (14536 bytes in 0.009s)
PS L:\bksony> ./adb install -r renotrap.apk
3416 KB/s (268736 bytes in 0.076s)
Success
PS L:\bksony> .\adb.exe shell
G8142:/ $ cd /data/local/tmp
cd /data/local/tmp
G8142:/data/local/tmp $ ls
ls
renoroot  renoshell  renosploit
G8142:/data/local/tmp $ chmod 755 re*
chmod 755 re*
G8142:/data/local/tmp $ ./renoroot
./renoroot

renosploit by j4nn
https://j4nn.github.io

starting rename/notify attack,
please wait...


```
# reboot and root again then backup
```
PS L:\bksony> .\adb.exe shell
G8142:/ $ cd /data/local/tmp
cd /data/local/tmp
G8142:/data/local/tmp $ ./renoroot
./renoroot

renosploit by j4nn
https://j4nn.github.io

starting rename/notify attack,
please wait...

    0m08.50s real     0m00.00s user     0m00.00s system

renoshell - rename/notify temp root shell
https://github.com/j4nn/renoshell/README.md

kaslr slide 0x415200000
task_struct 0xffffffe2252b5e80

got root, start shell...

G8142:/data/local/tmp # dd if=/dev/block/bootdevice/by-name/TA of=TA-locked.img
d if=/dev/block/bootdevice/by-name/TA of=TA-locked.img                        <
4096+0 records in
4096+0 records out
2097152 bytes transferred in 0.049 secs (42799020 bytes/sec)
G8142:/data/local/tmp # chown shell:shell TA-locked.img
chown shell:shell TA-locked.img
G8142:/data/local/tmp # sync
sync
G8142:/data/local/tmp # sync
sync

PS L:\bksony> ./adb pull /data/local/tmp/TA-locked.img
1783 KB/s (2097152 bytes in 1.148s)
```

说明：一定要使用指定固件

保证TA能用，拨号输入`*#*#7378423#*#*`，找到`security`，内部key为`PROVISIONED`

链接：[百度云](https://pan.baidu.com/s/1HaAVInF57f1T3wRzSVazsg) 提取码：id5h 
