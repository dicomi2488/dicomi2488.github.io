# 使用免费的虚拟主机搭建私有云盘
### 配置虚拟主机

最近在nl上又看到了个支持ssh的虚拟主机了，看了下免费的版本还不错,大概长这样：  
![virtual_hosting_cloud_1.PNG](https://i0.hdslb.com/bfs/openplatform/6bb71536374243029a23ddac2446bae050c01472.png ':size=25%')  
[这是官网链接](https://my.dataonline.vn/?affid=206)，有中文，注册的时候手机号可以随便填，不会验证，注册完选那个免费的廉价主机，然后要绑定域名，注意这里二级域名也是可以用的，例如我之前白嫖了个xxx.dpdns.org的域名，那就这样填：  
![virtual_hosting_cloud_2.PNG](https://i0.hdslb.com/bfs/openplatform/5095f8113d3da1a56c61c44f9724e22a5dac48c8.png ':size=50%')  
检查完后前面的那个www.就没有了。  
然后就是把他给你的dns记录给抄到自己域名那里，ns记录可不抄  
![virtual_hosting_cloud_3.PNG](https://i0.hdslb.com/bfs/openplatform/80e9371bdd4064feab21f73b4f5862cf2f351a88.png ':size=50%')  
然后我使用的是开源的[可道云](https://kodcloud.com/explorer/download/)，直接进官网下服务器端(约36.7MB)  
然后需要把下下来的zip文件传到主机上去，推荐用ftp传，比[控制面板](https://sv66.dataonline.vn:2222/evo/)传快不少，ftp和ssh的ip就是你之前设置dns指向的那个ip，账密在这：  
![virtual_hosting_cloud_4.PNG](https://i0.hdslb.com/bfs/openplatform/14fa07f97924dcfafd7a6dd961e8683f43ed52eb.png ':size=50%')  
把zip文件传到/your_domains/public_html/下，把原来自带的两个文件删掉，解压zip文件。
此时你的文件夹应该长这样：  
![virtual_hosting_cloud_5.PNG](https://i0.hdslb.com/bfs/openplatform/11f7b84f49bb971542feedaf1df6be8ca1a8da75.png ':size=50%')

### 配置云盘

打开你的域名，开始系统安装，环境检测直接跳过，数据库类型mysql，然后回到控制面板，创建一个数据库，把账密copy过来，最终大概长这样：  
![virtual_hosting_cloud_6.PNG](https://i0.hdslb.com/bfs/openplatform/accd5c8cf3fd08cfaa6bda9ae5dc9afc1b784b98.png ':size=50%')  
然后设置账密就行了。
给大家展示一下最终成品：  
![virtual_hosting_cloud_7.PNG](https://i0.hdslb.com/bfs/openplatform/bf1caf49a583722d2e176df0e6fc28c5f7f04675.png ':size=50%')  
![virtual_hosting_cloud_8.PNG](https://i0.hdslb.com/bfs/openplatform/8597028eb930b058beea2cb7321d55c3a95fad61.png ':size=50%')  
最后把我的网盘放这给大家看看速度把，不要乱搞，掉了不补http://mrc.dpdns.org  
账号root密码qkSbh97L0X6tDx

------

发布日期：2025/7/31

最后编辑日期：2025/10/1
