## 介绍

webs 是一个运行前端代码(html/css/js)的 app ，运行的容器是 wkwebview。

除了拥有 浏览器的能力外，也可以使用 由 webs 提供的 增强能力，比如 粘贴板、无跨域的 http 等等 。
> ps : 该文档需要配合 webs (ios app) 使用，暂无支持安卓的计划


## 如何编写一个webs 的程序呢 ？

 如果你熟悉 （ html / css / js ）， 那编写一个 webs 的应用程序几乎不需要什么学习成本，你只需要添加一个 webApp.json 文件项目的根目录即可。
例如这样

```shell
- index.html
- icon.png
- webApp.json
```

>ps: icon.png 这个文件是作为 webs 程序的图标显示，如果没有一个文件的话将显示一个默认的图标


### webApp.json 文件说明

```json
{
    "name":"名称", // 程序的名称
    "version":"1.0.3", // 程序的版本
    "miniVersion":102, // 程序的最低运行版本
    "author":"COR", // 程序的作者
    "appid":"888888B8-8888-8888-8888-B88888888888" 
    // 这个是程序的id,可以在 webs 开发者服务中获取
    // 这个 appid 是程序的唯一标识，不可以和其他程序一起使用。
}
```




