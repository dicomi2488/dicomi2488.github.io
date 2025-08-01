###配置虚拟主机

最近在nl上又看到了个支持ssh的虚拟主机了，看了下免费的版本还不错,大概长这样：

![捕获-2.PNG](https://img.remit.ee/api/file/BQACAgUAAyEGAASHRsPbAAJUdmiKRtKIYCb1x4p-xMm5toAyOYHnAAIZFwAC_JFRVJEXtlEHnuLyNgQ.png)

[这是官网链接](https://my.dataonline.vn/?affid=206)，有中文，注册的时候手机号可以随便填，不会验证，注册完选那个免费的廉价主机，然后要绑定域名，注意这里二级域名也是可以用的，例如我之前白嫖了个xxx.dpdns.org的域名，那就这样填：

![捕获-3.PNG](https://img.remit.ee/api/file/BQACAgUAAyEGAASHRsPbAAJUd2iKRvv0SkriOA-3t_ZEeeihbINVAAIaFwAC_JFRVHbuXaCWw37CNgQ.png)

检查完后前面的那个www.就没有了。
然后就是把他给你的dns记录给抄到自己域名那里，ns记录可不抄

![捕获-5.PNG](https://img.remit.ee/api/file/BQACAgUAAyEGAASHRsPbAAJUeGiKRx4kbCzdnUzBlc0sdByBfBHYAAIbFwAC_JFRVF3xpJ_W5IxUNgQ.png)

然后我使用的是开源的[可道云](https://kodcloud.com/explorer/download/)，直接进官网下服务器端(约36.7MB)
然后需要把下下来的zip文件传到主机上去，推荐用ftp传，比[控制面板](https://sv66.dataonline.vn:2222/evo/)传快不少，ftp和ssh的ip就是你之前设置dns指向的那个ip，账密在这：

![捕获-6.PNG](https://img.remit.ee/api/file/BQACAgUAAyEGAASHRsPbAAJUeWiKRz7dFO27k7pMYIZVcwkIvodEAAIeFwAC_JFRVA90mAWcUtNvNgQ.png)

把zip文件传到/your_domains/public_html/下，把原来自带的两个文件删掉，解压zip文件。
此时你的文件夹应该长这样：

![捕获-7.PNG](https://img.remit.ee/api/file/BQACAgUAAyEGAASHRsPbAAJUemiKR1blvaHb-VOMH8d9ufEMhWYpAAIfFwAC_JFRVPLGCV0N6CkoNgQ.png)

###配置云盘

打开你的域名，开始系统安装，环境检测直接跳过，数据库类型mysql，然后回到控制面板，创建一个数据库，把账密copy过来，最终大概长这样：

![捕获8.PNG](https://img.remit.ee/api/file/BQACAgUAAyEGAASHRsPbAAJUe2iKR3FO1EWmx0IS5J5_iU22d7WTAAIgFwAC_JFRVFzGLfRjDLuENgQ.png)

然后设置账密就行了。
最后把我的网盘放这给大家看看速度把，不要乱搞，掉了不补http://mrc.dpdns.org
账号root密码qkSbh97L0X6tDx
