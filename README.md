# 自学Astro中

自学coding啊，了解了一点点基本语法之后，就应该找一个开源项目，fork下来之后自己拆解玩弄，然后给他来个翻新

## package.json

这个文件很神奇，运行下述指令时，npm会递归找这个文件，然后根据该文件里面的"dependenciecs"内容递归下载astro模块

```powershell
npm install astro@latest
```

## .astro

该目录为`npm run dev`的结果存放目录，区别于`npm run build`的结果存放在`dist\`目录

## `<title><title />`

很无语模板文件里面竟然有错误的闭合标签格式。正确写法是`<title></title>`

## 在浏览器打开页面时底部的开发者工具是哪里来的？

众所周知`npm run ${your command}`会在`package.json`文件里面的`scripts`字段寻找指令名，但是这些指令是在哪里实现的呢？
