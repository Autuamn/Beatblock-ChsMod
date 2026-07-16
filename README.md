# Beatblock 简体中文汉化 Mod

![Beatblock](https://img.shields.io/badge/Beatblock-1.7.1-blue)

为节奏游戏 [**Beatblock**](https://bubbletabby.com/) 制作的简体中文汉化模组。

基于 [TowaNoah](https://github.com/Lilyltt) 的[汉化工具](https://www.bilibili.com/video/BV1MgsHzpEgw)内的 ChsMod 修改

## 安装

### 安装 lovely-injector

1. 下载 [lovely-injector](https://github.com/ethangreen-dev/lovely-injector/releases)
2. 对于 Windows 平台，将解压的 `version.dll` 文件放到 Beatblock 根目录：
    ```
   steamapps/common/Beatblock/
                    ├── Beatblock.exe
                    ├── version.dll
                    └── ...
   ```
   其他平台详见 [Manual Installation](https://github.com/ethangreen-dev/lovely-injector#manual-installation)

### 安装 ChsMod

1. [下载](https://github.com/Autuamn/Beatblock-ChsMod/archive/refs/heads/main.zip)本仓库
2. 在 Beatblock 存档目录下的 `Mods` 文件夹中创建 `ChsMod` 文件夹，将解压出的内容放置于此，最终的目录结构应为：
   ```
   beatblock/
   ├── ...
   ├── savedata/
   └── Mods/
       └── ChsMod/
           ├── localization.json
           ├── optionsMenuItems.json
           ├── lovely.toml
           ├── fonts/
           └── icons/
   ```
    存档目录可能的位置：
    - **Windows**: `%AppData%/beatblock/`
    - **Linux**: `~/.local/share/beatblock`
    - **Mac**: `~/Library/Application Support/beatblock`

### 修改设置

启动游戏，在「Settings → Language」中选择「简体中文」，重启游戏即可生效。

#### 字体模式说明

在「设置 → 语言」中可切换字体模式：

- **替换** — 将游戏主字体（`main` 和 `digitalDisco`）直接替换为「缝合像素字体」
- **设置回退** — 在主字体缺少字符时自动使用「缝合像素字体」显示

> 更改字体模式需要重启游戏才能生效。由于 LOVE2D 引擎的 [bug](https://github.com/love2d/love/issues/1990)，使用「设置回退」模式有时可能导字符顺序错乱等问题。

## 使用的字体

 - [**缝合像素字体**](https://github.com/TakWolf/fusion-pixel-font) — 界面主要字体
 - [**长坂点宋 16**](https://github.com/yzdnn/ChangBanDianSong-16) — 钓鱼时鱼的描述
 - [**Unifont**](https://unifoundry.com/unifont/) — 替换 JF-Dot-jiskan16s-2000
 - [**精品点阵体7×7**](https://github.com/scott0107000/BoutiqueBitmap7x7) — TerabyteIntro


## 更新日志

各版本变更详见 [`Changelog.md`](Changelog.md)。
