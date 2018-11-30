## 什么是webpack
webpack是一个javascript应用程序的静态模块打包器（static module bundler）。在webpack处理应用程序时，它会在内部创建一个依赖图（dependency graph）(在webpack中一切皆模块)，用于映射到项目需要的每个模块，然后将所有这些依赖生成到一个或多个bundle（浏览器可识别的一个或者多个文件）。

##  webpack和其他前端自动化构建工具的区别在哪？
  
  * gulp:前端自动化构建工具，以任务的形式进行构建，css的编译，js编译，启动服务，手动配置，对文件进行操作
  
  * grunt:类似于gulp也是自动化的构建工具，减轻手动构建的效率低下的问题
  
  * wepack:以模块为入口，使用loader,plugins对文件进行编译，在webpack中所有内容都是模块
 
## webpack的核心概念
  
  * 模块解析规范，在webpack中模块是按照nodejs commonjs规范定义，也可以自己配置（resolve）
  
  * 入口（entry）
  
  * 出口（output）
  
  * 解析规则（loader）

  * 插件（plugins）
  
  * devServer

## 安装
  npm install webpack webpack-cli -g 或者 yarn global add webpack webpack-cli 然后就可以全局执行命令了 webpack-cli 是使用 webpack 的命令行工具，在4.X版本后不再作为webpack的依赖了，我们使用时需要单独安装这个工具
  
 ## 入口 entry
 
  入口起点（entry point）指示webpack应使用哪个模块，来作为构建其内部依赖图的开始，webpack会找出有哪些模块和library是入口起点（直接和间接）依赖的。
  
  ```
    语法： entry: string | [string] | object { : string | [string] } | (function: () => string | [string] | object { : string | [string] })
    
  ```
  传递一个字符串代表一个入口
  传递数组(Array) 或者对象(Object),代表一个或者多个入口
  
  示例
    
   ```
    module.exports = {
      entry:'app.js'
    }
   ```
