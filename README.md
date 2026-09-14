# 明日方舟香草杯

明日方舟全角色淘汰赛生成器。打开即可使用，无需安装。

**在线体验：https://stedean-sawamura.github.io/Ark_vanilla_cup/**

## 使用方式

直接访问上方链接，或下载后在浏览器中打开 `index.html`。

所有数据已预缓存在仓库中，打开即用；页面会自动检查 PRTS 是否有新增内容，有则增量更新。

## 角色池

| 池 | 数量 | 说明 |
|---|---|---|
| 干员 | 460+ | 全部可获取干员，含头像 |
| 敌人 | 1800+ | 全部关卡敌人，含头像 |
| 剧情角色 | 520+ | 剧情中登场的 NPC，立绘裁剪为头像 |
| 道具 | 1380+ | 全部游戏道具，含图标（趣味赛） |

设置面板中可任意勾选组合，支持混池或单独比赛。

## 功能

- **四大角色池** 可任意组合：干员 / 敌人 / 剧情角色 / 道具
- **按性别分组** 或 **全员混战** 或 **按道具分类**
- **满编 / 均分** 两种分组方式
- **异格干员** 可选独立参赛或合并为同一角色
- **同名去重** 自动合并跨池同名角色
- **排除关键词** 过滤卫戍协议、预备干员等，支持自定义
- **overwrites.json** 手动覆写角色属性（已预填 637 个角色性别）
- 自定义每组人数上限，自动拆分 Tab + 总决赛
- 左右对称淘汰赛布局，冠军在正中汇合，金色虚线连接
- 点击空位选择胜者，支持清除和级联重置
- 轮空均匀分散，避免同对位双轮空
- 🎲 打乱全部 / 只打乱当前组
- 📤 分享：截图当前赛区 / 生成文字战报
- 💾 保存 / 读取进度（localStorage）
- 鼠标拖拽 + 滚轮缩放 / 手机触屏拖拽 + 双指缩放

## 数据文件

| 文件 | 说明 |
|---|---|
| `operators.json` | 干员数据（名称/性别/头像/charId） |
| `enemies.json` | 敌人数据（名称/头像） |
| `story_chars.json` | 剧情角色数据（名称/立绘） |
| `items.json` | 道具数据（名称/图标） |
| `overwrites.json` | 手动覆写（性别等），不会被数据更新覆盖 |

所有数据来自 [PRTS Wiki](https://prts.wiki)（明日方舟中文 Wiki）。

---

# Arknights Vanilla Cup

An all-character elimination tournament bracket generator for Arknights. No installation required.

**Live Demo: https://stedean-sawamura.github.io/Ark_vanilla_cup/**

## Usage

Open the link above, or download and open `index.html` in a browser.

All data is pre-cached in the repository. The page automatically checks PRTS for updates and fetches incrementally.

## Character Pools

| Pool | Count | Description |
|---|---|---|
| Operators | 460+ | All obtainable operators with avatars |
| Enemies | 1800+ | All stage enemies with portraits |
| Story Characters | 520+ | NPCs from story chapters, art cropped as avatars |
| Items | 1380+ | All game items with icons (fun bracket) |

Mix and match pools freely in the settings panel.

## Features

- **4 character pools** — operators / enemies / story NPCs / items
- **Group by gender**, **free-for-all**, or **by item category**
- **Full / even split** modes for sub-groups
- **Alter operator** merge (combine alternate versions of the same character)
- **Same-name dedup** across pools
- **Exclude keywords** — filter out Stationary Security / Reserve Operators, etc.
- **overwrites.json** — manually override character attributes (637 genders pre-filled)
- Custom group size, auto-split into tabs + grand finals
- Symmetric L/R bracket layout, champion at center with gold dashed connectors
- Click empty slots to pick winners, with clear and cascade reset
- Byes evenly distributed, no same-match double byes
- 🎲 Shuffle all / shuffle current group only
- 📤 Share: screenshot or text report
- 💾 Save / load progress (localStorage)
- Mouse drag + scroll zoom / touch drag + pinch zoom

## Data Files

| File | Description |
|---|---|
| `operators.json` | Operator data (name, gender, avatar, charId) |
| `enemies.json` | Enemy data (name, portrait) |
| `story_chars.json` | Story character data (name, art) |
| `items.json` | Item data (name, icon) |
| `overwrites.json` | Manual overrides (gender, etc.), survives data regeneration |

All data sourced from [PRTS Wiki](https://prts.wiki) (Arknights CN Wiki) via MediaWiki API.
