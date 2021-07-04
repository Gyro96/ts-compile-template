# 通过 rollup 将 ts 进行自动化打包并运行，方便学习和调试

## 安装依赖

- npm install

## 在 src/index.ts 中书写代码

## 运行命令

- npm run dev
  - rollup -cw: 表示使用配置文件进行打包并且实时监听

## 一些说明

### 使用 ts 需要安装 typescript

- npm install typescript -g
- tsc --init 生成 ts 配置文件

### 构建工具来处理 ts（ts 开发环境）

- 使用 rollup 将 ts 转换成 js 然后插入到页面中，自动运行
- 解析 ts 的方式：ts 插件 和 Babel
  - rollup 使用 rollup-plugin-typescript2 来进行解析
  - webpack 使用 ts-loader 或者 babel-plugin-typescript

### 本地直接通过 node 环境运行 ts

- VScode 安装插件：Code Runner
- npm 安装包：npm install ts-node -g

### 依赖

- rollup：打包
- typescript
- rollup-plugin-typescript2：让 rollup 可以识别 ts 并进行解析
- @rollup/plugin-node-resolve：让 rollup 支持引入第三方模块
- rollup-plugin-serve：开启一个服务器，进行预览
