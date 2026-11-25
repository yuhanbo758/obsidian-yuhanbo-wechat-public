# yuhanbo-wechat-public

Preview Markdown in a WeChat article layout. The desktop plugin supports customizable typography, themes, tables, and Mermaid previews.

## Installation

Download `main.js`, `manifest.json`, and `styles.css` from the same [GitHub Release](https://github.com/yuhanbo758/obsidian-yuhanbo-wechat-public/releases/latest). Place all three files in the vault's plugin directory under `plugins/yuhanbo-wechat-public/` and enable the plugin in **Settings → Community plugins**.

## Usage

Open the WeChat Markdown editor from the ribbon or command palette. Use **Refresh** to load the active note when automatic sync is off. Preview and **Standard copy** are free. To enable **WeChat copy** and **Table image copy**, open the purchase link in **Copy authorization** or go to the [Program Shop product page](https://shop.sanrenjz.com/obsidian/obsidian%E6%8F%92%E4%BB%B6-yuhanbo-wechat-public). Paste the license code you receive into the plugin settings and select **Activate**.

Rendering and license verification run locally. Copy actions write to the system clipboard. Remote images referenced in a note load from their original URLs. Selecting the purchase link opens the shop in the browser, where the shop handles payment and license delivery. The plugin does not collect telemetry.

将 Markdown 预览为微信文章排版，支持主题、字体、Mermaid 图表和表格图片复制。

## 功能与授权

- 免费：预览、普通复制、主题设置、路径复制。
- 需授权：微信复制、图表复制。图表复制将文章中的文字表格转为 PNG，其他内容保持富文本。
- 在插件设置「复制功能授权」中点击「前往程序小店购买授权码」。购买后将收到的授权码粘贴到设置中，再点「激活」。已有授权码可以直接激活。社区支付类型为 **Optional payment**，购买和发码由程序小店处理。
- 授权码离线验签，不要求登录、不采集设备信息；授权保存在本库 `data.json`，请勿公开。当前不绑定设备、不支持远程撤销，授权码可被转发。本地代码可被修改，签名校验不保证防破解。

## 安装

从 [最新正式版本](https://github.com/yuhanbo758/obsidian-yuhanbo-wechat-public/releases/latest) 下载 `main.js`、`manifest.json`、`styles.css`，放入库配置目录的 `plugins/yuhanbo-wechat-public/`，然后在第三方插件设置中启用。

桌面版适用，最低版本以 manifest 为准。社区目录需要另行审核；GitHub Release 可下载不代表已在社区上架。

旧测试版的安装 ID 为 `obsidian-yuhanbo-wechat_public`。社区版使用符合规范的新 ID `yuhanbo-wechat-public`，两者配置独立；迁移时自行备份配置，勿同时启用两个版本。

## 预览性能

自动同步开启时，仅在本插件侧栏可见时渲染，输入停顿 250ms 后更新。切到日历等其他侧栏或折叠侧栏后暂停。关闭自动同步后，点击“刷新”手动更新。

## 隐私与网络

复制只写入本地剪贴板，不向服务器上传笔记。授权校验不联网；没有遥测、追踪或授权服务器。Mermaid 随发行包打包，不再从 CDN 下载脚本。普通本地/远程图片按 Markdown 原有地址加载。绝对路径复制仅在用户点击时读取当前库的桌面路径。

## 源码与更新

本仓库提供安装包与使用文档。原始源码与构建工程由作者在私有 GitHub 仓库维护，使用 Obsidian 社区的私有源码审核流程。发行构建包含受各自许可证约束的第三方组件。

作者在私有源码仓库发布更新时，GitHub Actions 测试并构建安装包，再同步到本仓库的 Releases。社区上架后，Obsidian 可通过第三方插件更新界面获取新版本。

许可证：MIT，见 [LICENSE](LICENSE)。MIT 许可与用户此前获得的权利不因授权界面而被撤销。

## 作者与相关链接

余汉波 · [GitHub](https://github.com/yuhanbo758) · [三人聚智](https://www.sanrenjz.com)

- [在线文档](https://docs.sanrenjz.com)
- [插件商店](https://shop.sanrenjz.com)
- [联系我们](https://www.sanrenjz.com/contact_us/)

![三码合一](https://gdsx.sanrenjz.com/image/sanrenjz_yuhanbolh_yuhanbo758.png?imageSlim&t=1ab9b82c-e220-8022-beff-e265a194292a)

![余汉波打赏码](https://gdsx.sanrenjz.com/PicGo/%E6%89%93%E8%B5%8F%E7%A0%81500.png)
