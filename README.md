个人博客 | 技术 · 杂谈 · Java、Clojure、Nodejs、Python、算法

http://liujiacai.net/

本博客的目的就是记录自己学习过程中的所得所想，我觉得所有事情都可以用感性的直觉去理解。如果自己在两三句话向一个陌生人讲不清楚某个知识点，说明我也是没懂。


## 部署

Node 6.10.3，其他版本会遇到各种依赖问题

hexo 3 + maupassant

```
# 解决 ../src/sass_context_wrapper.h:8:10: fatal error: 'sass/context.h' file not found
brew install libsass

npm install

# 如果安装了 libsass 还是报头文件的错，直接下载 sass binary 文件
SASS_BINARY_SITE=https://npm.taobao.org/mirrors/node-sass/ npm install node-sass
rm -rf node_modules
npm install
```
