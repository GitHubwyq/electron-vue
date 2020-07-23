# electron-vue

## 安装依赖
```
yarn install
```

### 启动服务
```
yarn electron:serve
```

### 打包成  .exe桌面文件
```
yarn electron:build
```


#### 注：后台地址来源于：https://github.com/lin-xin/vue-manage-system  

---------------------------------------------------------------------------------

如果想尝试自己上手electron，安装步骤如下：


### 推荐使用yarn安装
```js
全局安装yarn
npm install -g yarn

```

### 1、安装vue及vue-cli（vue-cli可以安装新版的3.0及以上）
```js
//安装vue
yarn add vue

//安装@vue/cli
yarn add -g @vue/cli
```

### 2、创建项目
```js
vue create ele-demo
```

### 3、安装electron-builder
```js
vue add electron-builder
```

### 4、启动/打包
```js
// 启动
yarn run electron:serve

// 打包
yarn run electron:build

```

#### 注： 开发dev状态的话，electron的开发者工具，也是可以使用快捷键呼出的。win下的快捷键是：ctrl+shift+i，mac下的快捷键是：alt+花+i。这两个快捷键和chrome的定义，是有所区别的，这个请大家注意一下即可。

### 卡住解决方案

#### 修改~/.npmrc 或者 .yarnrc 文件，加入如下代码

```js
registry=https://registry.npm.taobao.org
electron_mirror="https://npm.taobao.org/mirrors/electron/"
```
