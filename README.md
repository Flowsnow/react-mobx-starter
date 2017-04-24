# react-mobx-starter

## 来源

clone自comyn大神的[comyn-react-mobx-starter](https://coding.net/u/comyn/p/react-mobx-starter/git)。以下任何修改都遵循MIT License。

- 去掉package.json中的node-sass依赖
- 将初始示例的index.js修改为简易的hello world项目
- 完善README.md

## 使用

从仓库克隆

```shell
git clone git@github.com:Flowsnow/react-mobx-starter.git
```

使用npm安装依赖包，需要预先安装好nodejs，当前nodejs版本为7.9.0。

```shell
cd react-mobx-starter
npm install
```

启动项目

```shell
npm start
```

打开浏览器访问[http://localhost:3000](http://localhost:3000)查看效果

如果需要改为自己的项目，只需要修改package.json中和项目有关的项即可，比如项目名称，项目描述，仓库地址等等。

## 依赖介绍

### devDependencies

devDependencies  用于开发环境，不发布到生产环境

```json
"devDependencies": {
  	// babel6开始babel分为core和插件
    "babel-core": "^6.24.1",
    "babel-loader": "^6.4.1",
  	// 使用装饰器时需要依赖此插件
    "babel-plugin-transform-decorators-legacy": "^1.3.4",	//
    "babel-preset-env": "^1.4.0",
    "babel-preset-es2015": "^6.24.1",
    "babel-preset-es2017": "^6.24.1",
    "babel-preset-react": "^6.24.1",
    "babel-preset-stage-0": "^6.24.1",
  	// webpack的css依赖
    "css-loader": "^0.28.0",
  	// webpack依赖less和less-loader
    "less": "^2.7.2",
    "less-loader": "^4.0.3",
  	// 当项目文件修改时会自动编译，在浏览器上查看效果
    "react-hot-loader": "^3.0.0-beta.6",
  	// 便于调试，es代码转译得到es5代码，当报错时，source-map会显示es6代码的报错行
    "source-map": "^0.5.6",
    "source-map-loader": "^0.2.1",
  	// css依赖的loader
    "style-loader": "^0.16.1",
  	// 打包工具
    "webpack": "^2.4.1",
  	// 开发时webpack启动的server
    "webpack-dev-server": "^2.4.2"
  }
```

### dependencies

dependencies 用于生产环境的插件，打包时会发布

```json
"dependencies": {
  	// ant design 蚂蚁金服开源的 react UI 库
    "antd": "^2.9.1",
  	// js基于promise语法标准的http库
    "axios": "^0.16.1",
  	// 只用旧浏览器时，polyfill插件会对不支持api??
    "babel-polyfill": "^6.23.0",
  	// 状态管理库，替代redux
    "mobx": "^3.1.9",
    "mobx-react": "^4.1.8",
    "mobx-react-devtools": "^4.2.11",
  	// 从react中分离出来的prop-types替代React.PropTypes
    "prop-types": "^15.5.8",
    "react": "^15.5.4",
    "react-dom": "^15.5.4",
    "react-router": "^4.1.1",
    "react-router-dom": "^4.1.1"
  }
```