## What I have learned 
Record some fragmented knowledge or problems
### 2022-06-17
Linux install Verdaccio
```
// for open firewall 
firewall-cmd --zone=public --add-port=3000/tcp --permanent
firewall-cmd
```


### 2022-06-20
#### 正则匹配获取中间字符
```
// start: ?<= end: ?=
let str = 'http://127.0.0.1:8080';
const buildFilepix = /(?<=http:\/\/).*?(?=:)/;
const outputDirPix = str.match(buildFilepix)[0];
// outputDirPix result 127.0.0.1
```

#### Electron markdown tools
article: https://juejin.cn/post/7110941851103789069

project: https://github.com/andyqier88/omd

### 2022-06-22
weppack config otions for ignore a module, like this

```
module.exports = {
  //...
  resolve: {
    alias: {
      'ignored-module': false,
      './ignored-module': false,
    },
  },
};
```
```
// rollup.config.js

output: [{
        sourcemap: true,
        format: 'esm',
        file: pkg.module,
        paths: {
          '@/api/camunda/list': '/@/api/camunda/list'
        }
      }]
```

### 2022-06-27

test case website
https://jsbench.me/

### 2022-07-01
https://www.joshwcomeau.com/javascript/terminal-for-js-devs/#getting-set-up

1. 微软商店
2. serch linux
<img width="745" alt="linux" src="https://user-images.githubusercontent.com/10238991/176809102-a2a00752-8352-4199-b80d-240419a51837.png">

3. sudo apt-get install zsh 
<img width="744" alt="install zsh" src="https://user-images.githubusercontent.com/10238991/176809159-bf0b3430-d124-47e4-88b9-d30282b602c8.png">

### 2022-07-07
get dirs 
```
let fs = require('fs')
function getDirs(path){
  let dirs = []
  const files = fs.readdirSync('path')
  files.forEach(function (item, index) {
      let stat = fs.lstatSync(path + item)
      if (stat.isDirectory() === true) { 
        dirs.push(item)
      }
  })
  return dirs
}
```

### 2022-07-28

> 为什么要学习原理（不管是编程领域还是其他领域），因为世间无穷的现象都可以用有限的原理解释，如果只停留于现象就会陷入经验主义。

### 2022-09-13
https://css-tricks.com/cool-hover-effects-using-background-properties/

https://github.com/JuneAndGreen/tooltpl
