# 如何安装 Vue 调试工具 Vue Devtools

### Vue2.0

推荐在浏览器（Chrome）安装 Vue Devtools 调试工具，可以快速查看 Vue组件和状态管理 Vuex 等的数据。
下面提供几种安装方法：
- 方法一：如果有梯子，可以直接在 Chrome 的应用商店下载；
- 方法二：从 Github 上 clone（很多资料的说法，亲测有问题，可能是项目版本的问题）：

1. 从 Github 上 clone 项目：
   
```sh
git clone https://github.com/vuejs/vue-devtools.git
```

2. 进入 `vue-devtools` 目录下，安装依赖（推荐使用 cnpm 代替 npm 命令）：

```sh
cnpm install
```

3. 构建工具
   
```sh
npm run build
```

4. 打开 Chrome 扩展程序，开启“开发者模式”，点击“加载已解压的扩展程序”，选择 vue-devtools 的目录下的 `shell/chrome`

5. 重新打开 Vue 项目，打开 Chrome 的调试工具，可以看到工具栏多了 Vue 选项，证明 vue-devtools 已经安装完成：

![image](/docs/images/devtools.png)

- 方法三：使用 npm 安装（推荐）：
  
1. 使用 npm 安装：
   
```sh
cnpm install vue-devtools -g
```

2. 通过 `npm config get prefix` 找到 npm 的全局安装目录，然后同方法二的第4步，只不过加载路径更改为：`node_moudules/vue-devtools/vender`

3. 同方法二的第5步

### Vue3.0 devtools

- Chrome：vue-devtools-6.0.0.beta21.crx 插件已上传，打开 chrome 浏览器扩展程序页(chrome://extensions/)，将 .crx 拖拽到当前页即可。
- Edge：打开 [Edge 加载项页面](https://microsoftedge.microsoft.com/addons/Microsoft-Edge-Extensions-Home)，搜索 vue devtools，安装 Beta 版本的插件即可。