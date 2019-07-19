# blog

前端开发博客
============
> 关注 Javascript, ES6, React, Redux 等
* [还在纠结 Flux 或 Relay，或许 Redux 更适合你](https://github.com/camsong/blog/issues/1)
* [传统 Ajax 已死，Fetch 永生](https://github.com/camsong/blog/issues/2)
* [Immutable 详解及 React 中实践](https://github.com/camsong/blog/issues/3)
* [抛弃 jQuery，拥抱原生 JavaScript](https://github.com/camsong/blog/issues/4)
* [CSS Modules 详解及 React 中实践](https://github.com/camsong/blog/issues/5)
* [React 最佳实践](https://github.com/camsong/blog/issues/6)
* [精读前后端渲染之争](https://github.com/camsong/blog/issues/8)
* [JavaScript 浮点数陷阱及解法](https://github.com/camsong/blog/issues/9)
* [给2019前端的5个建议](https://github.com/camsong/blog/issues/11)

[iron-redex](https://github.com/nefe/iron-redux)

### ES6
```
1.let const 与var
```
* [ES6!!!](https://www.kancloud.cn/pwstrick/fe-questions/1094973)

### 服务器配置
1.centos安装nginx
* 添加资源库 vi /etc/yum.repos.d/nginx.repo
[nginx]
name=nginx repo
baseurl=http://nginx.org/packages/centos/$releasever/$basearch/
gpgcheck=0
enabled=1
* 安装
yum install nginx
* 测试安装成功  nginx -t
* 找文件 find -name nginx
* 查看NG状态 systemctl status nginx.service
* 配置目录地址： /etc/nginx
* 修改配置目录下nginx.conf
``` 
    #user nginx;
    user  root;
```
* 修改web目录的读写权限 ： chmod  -R 777 /文件目录
* 重定向解决刷新404找不到页面问题：defult.conf文件中server配置属性location /{}对象下加try_files $uri $uri/ /index.html;
