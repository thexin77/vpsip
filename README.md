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
