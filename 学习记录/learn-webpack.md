------
# webpack是什么
- 一个打包工具
- 可以解析依赖，合并代码，压缩代码


------
# webpack初体验

### 安装
```
npm install --save-dev
```

### 使用
```js
// 在npm script 中定义指令，如:
"build": "webpack-dev-server  src/app.js  dist/bundle.js"

// 运行指令，即可在dist文件夹下生成打包文件bundle.js
npm run build

// 也可以指定参数 -p 打包生产环境下使用的最小代码
"build-prod": "webpack  src/app.js  dist/bundle.js -p"

// 打包成功后，最终使用dist/bundle.js就行了
```

------
# webpack-dev-server 初体验

