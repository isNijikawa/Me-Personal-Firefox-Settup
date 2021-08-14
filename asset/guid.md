我是安装教程详细版

## 准备在前
#### 约定
+ 你的火狐有一个 *资料目录*, 你可以通过访问 [about:support] 网页, 点击 "Profile Folder" 表格 的 "Open Folder" 进入.
+ 你的火狐拥有一个 *高级设置页*, 你可以通过访问 [about:profiles] 页进入, 上面有一个搜索框, 可以帮你快速查找设置选项.

##### 初始化
1. 进入 *高级设置页*. 
2. 搜索 "toolkit.legacyUserProfileCustomizations.stylesheets", 并将设置改为 true.
3. 进入你的 *资料目录* 并返回上一级.
4. 你会发现你的 *资料目录* 叫 "巴拉巴拉.default-release", 每个人的巴拉巴拉都不一样, 但是没有关系.
5. 删掉它!
6. 准备安装客制化👇

## 客制化
### 安装 win10 风格的滚动条
1. [下载仓库][3]
2. 解压文件, 然后进入 firefox 文件夹.
3. 把里面的 defaults 文件夹和 config.js 文件一并拖到 C:\Program Files\Mozilla Firefox 下 (即存放firefox.exe 的目录).
4. 进入 *资料目录*, 在里面创建一个文件夹, 起名为 "chrome".
5. 解压后的文件里有个叫 "profile" 的文件夹, 把里面的 "userChrome" 文件夹和 "userChrome.js" 文件一并放到第四步创建的 "chrome" 文件夹里.
6. 启动火狐, 如果提示你安装火狐便正常安装.
7. 重启浏览器, 你好了. 如果没好, 重复初始化过程的第一步和第二步.

退回原版:

修改userChrome.js 中

    userChrome.import("/userChrome/win10_scrollbars.uc.js", "UChrm");
    
到

    userChrome.import("/userChrome/custom_scrollbars.uc.js", "UChrm");
    
### 应用 Edge 风格化
1. [下载仓库][4].
2. 解压文件.
3. 把压缩文件里 chrome 文件夹下的所有内容放到 *资料目录* 的 chrome 文件夹里.
4. 重启浏览器, 你好了.

#### 可选项: 搜索框启用亚克力风格的高斯模糊效果
1. 进入 *高级设置页*. 
2. 把 "layout.css.backdrop-filter.enabled" 设置改为 true.
3. 重启浏览器, 你好了.

### 安装简化右键菜单
1. [下载仓库][5].
2. 解压文件.
3. 把解压后文件夹里的 "simpleMenuWizard" 文件夹放入 *资料目录* 的 chrome 文件夹里.
4. 重启浏览器, 你好了.

[3]: https://github.com/spencerwooo/firefox-overlay-scrollbar/archive/refs/heads/master.zip
[4]: https://github.com/isNijikawa/MaterialFox-in-Microsoft-Edge-Style/archive/refs/heads/master.zip
[5]: https://github.com/isNijikawa/simpleMenuWizard/archive/refs/heads/master.zip
