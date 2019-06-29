
nvm 安装
https://www.jianshu.com/p/8cd132c47380
https://github.com/coreybutler/nvm-windows/releases/tag/1.1.7

```
nvm  list available
nvm uninstall 8.12.0
nvm npm_mirror https://npm.taobao.org/mirrors/npm/
nvm install 8.12.0

nvm node_mirror https://npm.taobao.org/mirrors/node/
nvm npm_mirror https://npm.taobao.org/mirrors/npm/
```
$ npm install -g cnpm --registry=https://registry.npm.taobao.org

- 别人的工程下载下来总是有各种问题执行不起  
  **解决**  安装yarn 用yarn来运行
- 用nvm不能安装npm  
  **解决**  配置镜像，且在npm下载到temp解压的时候  把压缩包拷贝出来到对应版本的moudel下面并且 把bin 里面的东西直接拷贝到 该版本node.exe同目录