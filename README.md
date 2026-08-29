# 方格记忆卡

方格作文纸 × 朱红批改印章风格的英语六级词汇记忆卡(SRS 间隔重复),PWA 适配 iPhone。

在线版:https://2357-qaz.github.io/fangge-cards/

## 功能

- **今日任务**每天自动安排:错词前 10(最久未复习优先)+ 全部到期复习 + 20 个新词(全词库按列表序)
- 24 组共 2345 词(每组 100),简版 SM-2 间隔重复,错词单独进第二轮
- 手机手势:**左滑** 不认识 · **右滑** 认识 · **下滑** 眼熟 · **左屏缘右滑** 返回
- 进度存本机(localStorage),「导出进度 / 导入进度」JSON 备份搬家

## 安装到 iPhone 主屏(强烈建议)

Safari 打开 → 分享按钮 → **添加到主屏幕**。

为什么:home-screen PWA 不受 Safari「7 天未访问即清空站点数据」限制,进度才留得住;tab 模式下浏览器自带的左缘返回手势优先于页面手势(standalone 模式无此问题)。

## 文件

- `index.html` — 站点入口(由外层 `gen_decks.ps1` 从模板生成)
- `manifest.webmanifest` + `sw.js` — PWA 清单与离线缓存
- `icon-192.png` / `icon-512.png` / `maskable-512.png` / `apple-touch-icon.png` — 「记」印章图标(由外层 `gen_icons.ps1` 生成)
