### v3.0
 - 更新本地化文件至`1.6.0 (Early Access)[2880b4a6]`
 - 使用 `font.setFallbacks()` 方法为 main、digitalDisco、digitalDiscoGlitched、mainGlitched 字体设置中文回退字体，而不是替换它们
 - 用 unifont 字体替换 JF-Dot-jiskan16s-2000 字体；用 fusion-pixel-12px 字体替换 JF-Dot-K14-2004 字体
 - 对于 Glitched 字体不支持渲染中文文本导致的崩溃，修改了修复的方法。改为为 Glitched 字体设置回退使其支持中文
 - 修复渲染 Glitched 界面时用 `#` 按字节切割中文而产生非法字符
#### 已知问题
 - 因 LOVE2D 引擎的 bug，使用回退字体时字符顺序会错乱（[love2d/love#1990](https://github.com/love2d/love/issues/1990)），引擎已修复（[love2d/love#2277](https://github.com/love2d/love/pull/2277)），需要游戏更新引擎版本

### v2.1
 - 修改加载本地化文件的方法，不再依赖 lovely 获取 mod 目录

### v2.0
 - 更新本地化文件
    - 添加更新的文本与翻译
    - 修改部分翻译
        - Note 名使用原文（Block, Hold, Tap, Side...）
        - 判定使用原文（Perfect, Barely, Miss）
        - 难度使用原文
 - 修改加载本地化键与值的方式
     - 根据游戏提供的键的列表加载对应语言的值，没有对应语言的值将设置为 'en' 的值
 - 修正“玩笑”设置的位置
 - 修改字体
    - 移除原有的凤凰点阵体
    - 添加[缝合像素字体](https://github.com/TakWolf/fusion-pixel-font)、[长坂点宋 16](https://github.com/yzdnn/ChangBanDianSong-16)
    - 修改替换字体的方式
    - 修改加载字体的方式，不再写入文件系统
 - 实现中文换行
 - 修复《Era Chimæra》中的崩溃
    - 在解锁《Era Chimæra》时的 AotmMap 界面和《Era Chimæra》的最后会用 Glitched 字体渲染文本，不支持中文。在会用到 Glitched 字体时获取的本地化键值使用 'en' 的值
