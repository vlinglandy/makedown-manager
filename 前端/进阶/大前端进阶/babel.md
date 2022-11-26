## 使用过程

1. 首先定义一个node的项目nom init -y
2. 然后新建一个src目录，写上js文件
3. 配置.babelrc文件：{"presets":["es2015"],"plugins":[]}
4. 安装解码器：cnpm install --save-dev babel-preset-es2015
5. 生成编译文件babel src -d dist
