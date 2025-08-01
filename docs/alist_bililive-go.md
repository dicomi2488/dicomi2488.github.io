### 开局讲故事
本人高一，最近不放假了吗，我们高中化学老师就在抖音上给同学们开直播讲题，想给同学们制作一个录播，并且主机的空间不是很大，所以希望能把录播挂到云盘上去
### 需要用到以下项目
[bililive-go](https://github.com/hr3lxphr6j/bililive-go)
https://github.com/AlistGo/alist(如果你只是想把录播上传到云盘上去可以直接用云盘厂提供的webdav账号）
https://github.com/volga629/davfs2
### 安装
```
apt update
apt install ffmpeg davfs2 -y #bililive依赖和挂载webdav工具

mkdir bililive && cd bililive
curl -o bililive.tar.gz https://github.com/hr3lxphr6j/bililive-go/releases/download/v0.7.35/bililive-linux-amd64.tar.gz
tar -zxvf bililive.tar.gz

#安装alist
curl -fsSL "https://alist.nn.ci/v3.sh" -o v3.sh && bash v3.sh        
mkdir webdav #创建一个用于挂载webdav的文件夹，路径随意

```
### 挂载webdav

 打开alist，创建一个有webdav权限的账号
![alist_webdav](https://1drv.ms/i/c/f11b1c10cc3896aa/IQSue0p1Vy1kQYXTAx9oHBLAAQi1RQrzip-q4Z0uq3SyfoE)
```
mount -t davfs http://127.0.0.1:5244/dav /home/user/webdav #前面填写 你的alist地址/dav 后面填写刚才创建的文件夹
vim /etc/davfs2/secrets
```
添加以下内容：
```
http(s)://你的alist地址/dav webdav账号 webdav密码
```
设置权限
```
chmod 600 /etc/davfs2/secrets
```
此时打开文件夹应该能看到alist的内容即为成功
### 配置bililive
编辑bililive文件夹内的config.yml
```
rpc:
  enable: true
  bind: :8080
debug: false
interval: 20
out_put_path: /home/user/webdav #此处修改为你映射的webdav地址中的文件夹，例如：/home/user/webdav/189cloud/直播
ffmpeg_path: 
log:
  out_put_folder: ./
  save_last_log: true
  save_every_log: false
feature:
  use_native_flv_parser: false
```
### 启动！！！
`./bililive`


示例：~~[alist.dicomi.dpdns.org](https://alist.dicomi.dpdns.org)~~(已关)
