# uniapp + vite + pinia + ts + axios 项目模板快速开发

该模板是基于 uniapp + Vue3 + vite + pinia + ts + axios 项目模板快速开发，适用于小程序开发 h5。有问题可以**提 issue**或者**pull request**

> 注意：目前最新 vite5 + 该项目模板为了更好兼容用了 vite4 最新。如果项目需要使用 vite5，需要改某些包的语法即可。vite 有语法更改。

## 项目介绍

- 项目基于 uniapp + Vue3 + vite + pinia + ts + axios 项目模板快速开发，适用于小程序开发 h5。
- 项目使用了 vite 作为开发工具，支持 esm、cjs、iife 三种打包方式，支持按需加载，支持热更新。

## 项目运行

```bash
# 安装依赖
npm install

# 启动服务
npm run dev:h5  # 启动 h5 开发服务
npm run dev:mp-weixin  # 启动微信小程序开发服务

# 打包
npm run build:h5  # 打包 h5 项目
npm run build:mp-weixin  # 打包微信小程序项目
```

## 项目结构

```
├─ src
│  ├─ App.vue                                 # 入口页面
│  ├─ components                              # 公共组件
│  │  └─ ZmTabs.vue
│  ├─ config
│  │  └─ env.host.ts                          # 环境配置文件
│  ├─ main.ts                                 # 入口文件
│  ├─ manifest.json                           # 小程序 manifest 文件
│  ├─ pages                                   # 主包目录
│  │  ├─ cart
│  │  │  └─ cart.vue
│  │  ├─ category
│  │  │  └─ category.vue
│  │  ├─ index
│  │  │  ├─ cpns
│  │  │  │  └─ CustomNavbar.vue
│  │  │  └─ index.vue
│  │  └─ my
│  │     └─ my.vue
│  ├─ pages.json                              # 页面配置文件
│  ├─ plugins                                 # 插件目录
│  │  ├─ index.ts
│  │  └─ uview-plugins                        # uview插件目录
│  │     └─ index.ts
│  ├─ services                                # 服务目录
│  │  └─ user.ts
│  ├─ static                                  # 静态资源目录
│  │  ├─ images
│  │  └─ tabs
│  │     ├─ cart_default.png
│  │     ├─ cart_selected.png
│  │     ├─ category_default.png
│  │     ├─ category_selected.png
│  │     ├─ home_default.png
│  │     ├─ home_selected.png
│  │     ├─ user_default.png
│  │     └─ user_selected.png
│  ├─ stores                                  # 状态管理目录
│  │  ├─ index.ts
│  │  └─ modules
│  │     └─ user.ts
│  ├─ subPackages                             # 子包目录
│  │  └─ login
│  │     └─ login.vue
│  ├─ types                                   # 类型声明目录
│  │  ├─ auto-components.d.ts
│  │  ├─ auto-imports.d.ts
│  │  ├─ components.d.ts
│  │  └─ env.d.ts
│  ├─ uni.scss                                # uni-app的全局scss样式文件
│  └─ utils
│     ├─ assets                               # 静态资源工具类
│     │  ├─ localAssetURL.ts                  # 本地资源URL工具文件
│     │  └─ remoteAssetsURL.ts                # 远程资源URL工具文件
│     ├─ http.ts                              # HTTP请求工具文件
│     ├─ uniModals.ts                         # 弹窗工具文件
│     └─ uniStorage.ts                        # 存储工具文件
├─ tsconfig.json                              # ts编译配置文件
├─ uno.config.ts                              # unocss配置文件
└─ vite.config.ts                             # vite配置文件

