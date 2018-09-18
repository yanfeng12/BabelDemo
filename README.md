# BabelDemo
## Babel使用
### 1.Babel	是⼀个JavaScript编译器，它使⽤⾮常⼴泛，可以将es6转换成es5，从⽽在⼀些不⽀持es6的 浏览器中运⾏，这意味着你写es6代码的时候就不需要去关⼼浏览器是否⽀持es6
### 2.[babel中文文档](https://www.babeljs.cn/)
### 3.初始化项目npm	init -y
### 4.安装babel-cli,运行npm	install	babel-cli --save-dev.babel-cli是命令⾏⼯具，安装以后我们就可以在命令⾏中通过babel命令来转码
### 5.为了测试babel，新建index.js
```
()	=>	console.log("hello world")
//npm install babel-plugin-transform-es2015-arrow-functions --save-dev 

class demo{}
//npm install babel-plugin-transform-es2015-classes --save-dev 

//npm install babel-preset-es2015 --save-dev
//npm install babel-preset-env --save-dev

```
### 6.可以通过./node_modules/.bin/babel	index.js运行index.js或者修改package.json文件,运行npm	run	build
```
{
  "name": "babel-demo",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "node_modules/.bin/babel index.js"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "devDependencies": {
    "babel-cli": "^6.26.0",
    "babel-plugin-transform-es2015-arrow-functions": "^6.22.0",
    "babel-plugin-transform-es2015-classes": "^6.24.1",
    "babel-preset-env": "^1.7.0",
    "babel-preset-es2015": "^6.24.1"
  }
}

```
### 7.babel安装插件.运行npm install babel-preset-env --save-dev，新建.babelrc文件
```
{
	"presets":["env"]
}
```
### 8.运行npm run build

