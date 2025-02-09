<img src="./doc/assets/icon.png" width="300">

[![](https://img.shields.io/chrome-web-store/v/nhpjggchkhnlbgdfcbgpdpkifemomkpg.svg?logo=Google%20Chrome&logoColor=white&color=blue&style=flat-square)](https://chrome.google.com/webstore/detail/ajax-interceptor/nhpjggchkhnlbgdfcbgpdpkifemomkpg)
[![](https://img.shields.io/chrome-web-store/stars/nhpjggchkhnlbgdfcbgpdpkifemomkpg.svg?logo=Google%20Chrome&logoColor=white&color=blue&style=flat-square)](https://chrome.google.com/webstore/detail/nhpjggchkhnlbgdfcbgpdpkifemomkpg)
[![](https://img.shields.io/chrome-web-store/users/nhpjggchkhnlbgdfcbgpdpkifemomkpg.svg?logo=Google%20Chrome&logoColor=white&color=blue&style=flat-square)](https://chrome.google.com/webstore/detail/ajax-interceptor/nhpjggchkhnlbgdfcbgpdpkifemomkpg)

[![](https://img.shields.io/github/followers/YGYOOO.svg?label=Follow&style=social)](https://github.com/YGYOOO)


这是一个可以修改Ajax请求返回结果的Chrome插件，可用于调试/排查页面上的问题。（当然你也可以用其它一些工具如Charles修改网络请求的返回值，但操作繁琐，该插件方便很多，且不会对Chrome之外造成影响）

## 开发者手册

>python2 + node 10

chrome extensions documentation: <https://developer.chrome.com/docs/extensions/>

- [Manifest file format](https://developer.chrome.com/docs/extensions/mv3/manifest/)
- [使用 service_worker 来管理事件](https://developer.chrome.com/docs/extensions/mv3/service_workers/)
- [Content scripts](https://developer.chrome.com/docs/extensions/mv3/content_scripts/)
- [web_accessible_resources](https://developer.chrome.com/docs/extensions/mv3/manifest/web_accessible_resources/)

## 安装

chrome商店地址：<https://chrome.google.com/webstore/detail/ajax-interceptor/nhpjggchkhnlbgdfcbgpdpkifemomkpg>
不能翻墙的话可以在这里下载：<https://github.com/YGYOOO/ajax-interceptor/blob/master/Ajax-Interceptor.crx>

## 使用示例

<img src="./doc/assets/screenshot2.png" width="700">

示例视频：<https://weibo.com/tv/v/HlVZD8cR9?fid=1034:4352275389595232>

## 注意

1. 建议第一次安装完重启浏览器，或者刷新你需要使用的页面。
2. 当你不需要使用该插件时，建议把开关关上（插件icon变为灰色），以免对页面正常浏览造成影响。
3. 该插件只会在JS层面上对返回结果进行修改，即只会修改全局的XMLHTTPRequest对象和fetch方法里的返回值，进而影响页面展现。而你在chrome的devtools的network里看到的请求返回结果不会有任何变化。

## 更新说明

version 1.4.0:

- 1.调整目录结构和打包方式
- 2.修改样式
- 3.添加右键功能项

version 0.7:

- 新增单个URL开关功能：<https://github.com/YGYOOO/ajax-interceptor/issues/7>

version 0.5：

- 修复bug：<https://github.com/YGYOOO/ajax-interceptor/issues/1>

version 0.4:

- fetch发起的请求也可以被修改了

version 0.3:

- 增加了JSON编辑功能
