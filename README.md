<!--
 * @Descripttion:
 * @version:
 * @Author: sueRimn
 * @Date: 2025-11-05 15:18:02
 * @LastEditors: sueRimn
 * @LastEditTime: 2025-11-05 15:19:16
-->

# unishop

uniapp + Vue3 + Ts + Vite5 + UnoCss + WotUI 驱动的跨端快速启动模板，使用 VS Code 开发，具有代码提示、自动格式化、统一配置、代码片段等功能，同时内置了大量平时开发常用的基本组件

## &#x1F4C2; 快速开始

执行 `pnpm i` 安装依赖
执行 `pnpm dev` 运行 `H5`
执行 `pnpm dev:mp` 运行 `微信小程序`

## 📦 运行（支持热更新）

- web 平台： `pnpm dev:h5`, 然后打开 [http://localhost:9000/](http://localhost:9000/)。
- weixin 平台：`pnpm dev:mp` 然后打开微信开发者工具，导入本地文件夹，选择本项目的`dist/dev/mp-weixin` 文件。
- APP 平台：`pnpm dev:app`, 然后打开 `HBuilderX`，导入刚刚生成的`dist/dev/app` 文件夹，选择运行到模拟器(开发时优先使用)，或者运行的安卓/ios 基座。(如果是 `安卓` 和 `鸿蒙` 平台，则不用这个方式，可以把整个 unibest 项目导入到 hbx，通过 hbx 的菜单来运行到对应的平台。)

## 🔗 发布

- web 平台： `pnpm build:h5`，打包后的文件在 `dist/build/h5`，可以放到 web 服务器，如 nginx 运行。如果最终不是放在根目录，可以在 `manifest.config.ts` 文件的 `h5.router.base` 属性进行修改。
- weixin 平台：`pnpm build:mp`, 打包后的文件在 `dist/build/mp-weixin`，然后通过微信开发者工具导入，并点击右上角的“上传”按钮进行上传。
- APP 平台：`pnpm build:app`, 然后打开 `HBuilderX`，导入刚刚生成的`dist/build/app` 文件夹，选择发行 - APP 云打包。(如果是 `安卓` 和 `鸿蒙` 平台，则不用这个方式，可以把整个 unibest 项目导入到 hbx，通过 hbx 的菜单来发行到对应的平台。)
