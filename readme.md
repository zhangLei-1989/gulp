安装依赖 ----------------------------------------------
1.安装node 环境
2.在package.json 所在文件目录运行 npm install 命令  安装插件包
3.全局安装gulp 运行命令          npm  install gulp  -g
4.安装安装插件包     npm install rimraf -g

使用 --------------------------------------------------

1. 使用npm run dev    命令将对应执行gulp dev命令；
2. 使用npm run build  命令可以先删除生成后的文件，再重新打包生成
2. 使用npm run clean  命令删除生成后的文件。

文件组织目录结构 ----------------------------------------
 - project
  |- build   //构建脚本
  |- dist // 打包文件夹
  |- src  // 源文件夹
  | |- assets // 放置一些第三方文件，如bootstrap
  | |- css
  | | - index.css
  | |- images
  | |- js
  | | - index.js
  | |- sass
  | | - index.scss
  |- gulpfile.js
  - package.json

脚本文件配置(默认以配置好)----------------------------------
package.json 中定义的脚本
"scripts": {
    "dev": "gulp dev",
    "build": "rimraf dist && gulp build",
    "clean": "rimraf dist "
}
