### 部署
```
curl -ksSL https://gitlab.com/rwkgyg/cdnopw/raw/main/cdnopw.sh -o cdnopw.sh && bash cdnopw.sh
```
### 部署完输入
```
crontab -e
```
### 十分钟更新一次代码
```
*/10 * * * * cd /root/cfipopw/ && bash cdnip.
```
### 一个小时更新一次代码
```
* */1 * * * cd /root/cfipopw/ && bash cdnip.sh
```
### 面板
```
bash cdnopw.sh
```
实例1：每1分钟执行一次command

命令：

* * * * * command

 

实例2：每小时的第3和第15分钟执行

命令：

3,15 * * * * command

 

实例3：在上午8点到11点的第3和第15分钟执行

命令：

3,15 8-11 * * * command

 

实例4：每隔两天的上午8点到11点的第3和第15分钟执行

命令：

3,15 8-11 */2 * * command

 

实例5：每个星期一的上午8点到11点的第3和第15分钟执行

命令：

3,15 8-11 * * 1 command

 

实例6：每晚的21:30重启smb 

命令：

30 21 * * * /etc/init.d/smb restart

 

实例7：每月1、10、22日的4 : 45重启smb 

命令：

45 4 1,10,22 * * /etc/init.d/smb restart

 

实例8：每周六、周日的1 : 10重启smb

命令：

10 1 * * 6,0 /etc/init.d/smb restart

 

实例9：每天18 : 00至23 : 00之间每隔30分钟重启smb 

命令：

0,30 18-23 * * * /etc/init.d/smb restart

 

实例10：每星期六的晚上11 : 00 pm重启smb 

命令：

0 23 * * 6 /etc/init.d/smb restart

 

实例11：每一小时重启smb 

命令：

* */1 * * * /etc/init.d/smb restart

 

实例12：晚上11点到早上7点之间，每隔一小时重启smb 

命令：

* 23-7/1 * * * /etc/init.d/smb restart

 

实例13：每月的4号与每周一到周三的11点重启smb 

命令：

0 11 4 * mon-wed /etc/init.d/smb restart

 

实例14：一月一号的4点重启smb 

命令：

0 4 1 jan * /etc/init.d/smb restart

 

实例15：每小时执行/etc/cron.hourly目录内的脚本

命令：

01   *   *   *   *     root run-parts /etc/cron.hourly
