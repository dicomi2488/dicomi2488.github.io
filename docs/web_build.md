# 本站搭建方案

## 静态网站托管  
本站的所有源码都托管在[![github](https://img.shields.io/badge/github-12100E.svg?&logo=github&logoColor=white)](https://github.com/dicomi2488/dicomi2488.github.io)上，然后由[![Netlify Status](https://api.netlify.com/api/v1/badges/7f67682a-e069-462e-8dcd-00016c1cd399/deploy-status)](https://app.netlify.com/projects/dicomi/deploys)从github仓库拉取源码

## 域名
### dicomi.dpdns.org
于[DigitalPlat](https://domain.digitalplat.org/)免费获取，托管在cloudflare上，因为2025年7月份，cloudflare cdn的ip在大陆被封，所以关闭了cloudflare代理
### dicomi.cloudns.ch
于[cloudns](https://www.cloudns.net)免费获取，通过双向解析托管在cloudflare上，同样关闭了cloudflare代理
### dicomi.netlify.app
使用netlify静态网站托管服务时免费赠送
### dicomi2488.github.io
由github page提供
## 网页  
### 网页の根  
本站使用[docsify](https://docsify.js.org)
将markdown文件转换为网站  
### 网页插件
- [全文搜索-Search](https://docsify.js.org/#/zh-cn/plugins?id=%e5%85%a8%e6%96%87%e6%90%9c%e7%b4%a2-search)  
- [图片缩放-Zoom image](https://docsify.js.org/#/zh-cn/plugins?id=%e5%9b%be%e7%89%87%e7%bc%a9%e6%94%be-zoom-image)-Medium's 风格的图片缩放插件. 基于 [![github](https://img.shields.io/badge/github-medium_zoom-green)](https://github.com/francoischalifour/medium-zoom)。  
- [复制到剪贴板](https://docsify.js.org/#/zh-cn/plugins?id=%e5%a4%8d%e5%88%b6%e5%88%b0%e5%89%aa%e8%b4%b4%e6%9d%bf)  
- [评论系统](https://github.com/docsify-note/docsify-giscus)

### 图床
~~我对图床的要求不是要有多快，只要稳就够了，所以该网站的图片都是存在onedrive上的并且使用官方接口。~~
后来我发现onedrive在国内访问不了，所以就换成了基于bilibili的图床，全球速度都比较快

------

发布日期：2025/8/2

最后编辑日期：2026/1/1
