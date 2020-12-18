# npm / yarn 配置镜像、使用方法

## npm 配置

**`NPM`** 默认 `registry`：[https://registry.npmjs.org/](https://registry.npmjs.org/)

**`NPM`** 中文文档：[https://www.npmjs.cn](https://www.npmjs.cn)

淘宝 `NPM` 镜像：[https://npm.taobao.org](https://npm.taobao.org)

`CNPM`：[https://cnpmjs.org](https://cnpmjs.org)

> 永久使用

```bash
npm config set registry URL　# URL 即为需要设置的镜像站点地址

# 设置配置
npm config set registry https://registry.npm.taobao.org --global # 淘宝镜像

npm config set disturl https://npm.taobao.org/dist --global # Node镜像

# 获取配置
npm config get registry # 返回 https://registry.npm.taobao.org 即设置成功

npm config get disturl # 返回 https://npm.taobao.org/dist 即设置成功
```

> 临时使用

```bash
npm install [pkg] --registry=https://registry.npm.taobao.org

# 例如: npm install cnpm -g --registry=https://registry.npm.taobao.org
```

> 使用 cnpm

```bash
npm install cnpm -g

# React Native 官网 搭建开发环境 不建议使用 cnpm
```

> npm 命令缩写

```text
-v: --version

-g: --global

-reg: --registry

-S: --save

-D: --save-dev
```

## yarn 配置

> 安装 yarn

```bash
npm install -g yarn
```

> 设置 yarn 镜像源

```bash
yarn config set registry https://registry.npm.taobao.org --global
yarn config set disturl https://npm.taobao.org/dist --global
```

> yarn 使用方法

- Installing all the dependencies 安装依赖

  ```bash
  yarn

  yarn install
  ```

- Adding a dependency 添加依赖

  ```bash
  yarn add [package]
  yarn add [package]@[version]
  yarn add [package]@[tag]
  ```

- Adding a dependency to different categories of dependencies 添加依赖到不同依赖项中

  ```bash
  yarn add [package] --dev  # dev dependencies
  yarn add [package] --peer # peer dependencies
  ```

- Upgrading a dependency 更新依赖

  ```bash
  yarn up [package]
  yarn up [package]@[version]
  yarn up [package]@[tag]
  ```

- Removing a dependency 移除依赖

  ```bash
  yarn remove [package]
  ```

- Upgrading Yarn itself 升级 yarn

  ```bash
  yarn set version latest
  yarn set version from sources
  ```

- Accessing the list of commands 访问命令列表

  ```bash
  yarn help
  ```

- Starting a new project 初始化项目

  ```bash
  yarn init
  ```
