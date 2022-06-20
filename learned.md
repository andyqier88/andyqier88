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
