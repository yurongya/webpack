## 什么是webpack
webpack是一个javascript应用程序的静态模块打包器（static module bundler）。在webpack处理应用程序时，它会在内部创建一个依赖图（dependency graph）(在webpack中一切皆模块)，用于映射到项目需要的每个模块，然后将所有这些依赖生成到一个或多个bundle（浏览器可识别的一个或者多个文件）。

##  webpack和其他前端自动化构建工具的区别在哪？
  
  * gulp:前端自动化构建工具，以任务的形式进行构建，css的编译，js编译，启动服务，手动配置，对文件进行操作
  
  * grunt:类似于gulp也是自动化的构建工具，减轻手动构建的效率低下的问题
  
  * wepack:以模块为入口，使用loader,plugins对文件进行编译，在webpack中所有内容都是模块
  
  
