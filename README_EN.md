<!--
  Author: neuralpain
  Date: 2024-07-30 16:00:00 16:22:13
  LastEditors: neuralpain
  LastEditTime: 2024-07-30 16:22:13
-->

<h1 align="center">Simple mind map</h1>

[![npm-version](https://img.shields.io/npm/v/simple-mind-map)](https://www.npmjs.com/package/simple-mind-map)
![npm download](https://img.shields.io/npm/dm/simple-mind-map)
[![GitHub issues](https://img.shields.io/github/issues/wanglin2/mind-map)](https://github.com/wanglin2/mind-map/issues)
![license](https://img.shields.io/npm/l/express.svg)
[![GitHub stars](https://img.shields.io/github/stars/wanglin2/mind-map)](https://github.com/wanglin2/mind-map/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/wanglin2/mind-map)](https://github.com/wanglin2/mind-map/network/members)

[中文](./README.md)｜[English](./README_EN.md)

> Chinese name: 思绪思维导图。一个简单&强大的 Web 思维导图。

This project consists of two parts:

1. A js mind map library does not depend on any framework, and can be used to quickly complete the development of Web mind map products.

    Development documentation: https://wanglin2.github.io/mind-map/#/doc/zh/.

<!-- ! fix english here -->

2. A Web mind map, based on the mind map library, Vue2. Developed by X and ElementUI, it can operate local files on the computer, can be used as an online mind map application, and can also be self-deployed and developed for secondary use.

    Online address: https://wanglin2.github.io/mind-map/.

In addition, a client is also provided for download, with support for Windows, Mac and Linux

- [Github releases](https://github.com/wanglin2/mind-map/releases)
- [Baidu Cloud Disk](https://pan.baidu.com/s/1huasEbKsGNH2Af68dvWiOg?pwd=3bp3)

The client version will lag behind the online version. Please use the online version first to try the latest features.

<!-- ! ask for clarification  -->

> [!NOTE]
> ### Cloud storage version
> If you need a cloud storage version with a backend, you can [try another project or document we developed](https://github.com/wanglin2/lx-doc).

# Features

- [x] Plug-in architecture, in addition to the core functions, other functions are provided as plug-ins, which can be used on demand to reduce the packaging volume
- [x] Support logical structure diagram (left and right logical structure diagram), mind map, organizational structure diagram, catalog organization diagram, timeline (horizontal, vertical), fishbone diagram and other structures
- [x] Built-in multiple themes, allowing highly customized styles, and supporting registration of new themes
- [x] Node content supports text (normal text, rich text), pictures, icons, hyperlinks, remarks, labels, summaries, mathematical formulas
- [x] Nodes support drag and drop (drag and drop to move, free adjustment), a variety of node shapes; support expansion of node content, support the use of DDM to fully customize node content
- [x] Support canvas dragging and zooming
- [x] Support two multi-selection node methods: mouse button drag selection and Ctrl+left button
- [x] Support export as JSON, PNG, SVG, PDF, Markdown, xMind, TXT, support from JSON, xMind, Markdown
- [x] Support shortcut keys, forward and backward, association lines, search and replace, minimaps, watermarks, scroll bars, hand-painted styles, rainbow lines, markers, and frames
- [x] Provide a wealth of configurations to meet various usage habits in various scenarios
- [x] Support collaborative editing
- [x] Support demo mode

> [!NOTE]
> The following plug-ins are officially provided, which can be introduced according to the demand (the probability that a certain function will not take effect is because you have not introduced a corresponding plug-in). Please check the documentation for specific usage methods:
>
> - RichText (node rich text plug-in),
> -  Select (mouse multi-select node plug-in)
> - Drag (node drag-and-drop plug-in)
> - AssociativeLine (association line plug-in)
> - Export (export plug-in)
> - KeyboardNavigation (keyboard navigation plug-in)
> - MiniMap (small map plug-in)
> - Watermark (watermark plug-in)
> - TouchEvent (Mobile touch event support plug-in)
> - NodeImgAdjust (drag and drop to adjust the size of the node image plug-in)
> - Search (search plug-in)
> - Painter (node format brush plug-in)
> - Scrollbar (scroll bar plug-in)
> - Formula (mathematical formula plug-in)
> - Cooperate (collaborative editing plug-in)
> - RainbowLines (Rainbow line plug-in)
> - Demonstrate(Demo mode plug-in)
> - OuterFrame (outer frame plug-in)
> - HandDrawnLikeStyle (hand-painted style plug-in) [for a fee]
> - Notation (node marker plug-in) [for a fee]

> [!IMPORTANT]
> 
> Features that will not be implemented in this project:
> 
> 1. Free nodes, that is, multiple root nodes;
> 2. Continue to add nodes after the summary node;
>
> If you need the above features, then this library may not meet your needs.

# Install

```bash
npm i simple-mind-map
```

# Setup

Provide a container element with a width and height greater than 0:

```html
<div id="mindMapContainer"></div>
```

Set the CSS style:

```css
#mindMapContainer * {
  margin: 0;
  padding: 0;
 }
```

Then create an instance:

```js
import MindMap from "simple-mind-map";

const mindMap = new MindMap({
  el: document.getElementById("mindMapContainer"),
  data: {
    data: {
      text: "root node",
    },
    children: [],
  },
});
```

You can get a mind map.

Want to achieve more functions? You can view the development documentation.

# License

MIT. `mind-map` can be used commercially, as you like, as long is it retains the copyright notice. If you want a custom license for use within your organization, you can contact the author.

# WeChat Exchange Group

Because of the large number of people in the group chat, you will not be able to join via QR code. You can add the WeChat account of `wanglinguanfang` and ask to be added to the group. Questions related to mind maps can be asked in the group, so there is no need to chat with the author privately.

# Star the project

If you like this project, you are welcome to give it a star, which is very important to us.

[![Star History Chart](https://api.star-history.com/svg?repos=wanglin2/mind-map&type=Date)](https://star-history.com/#wanglin2/mind-map&Date)

# About customization

If you have personalized commercial customization needs, you can contact us. We provide paid development services, so whether it be front-end, back-end, or deployment, we can help you get it done in one stop.

# Invite the author for a cup of coffee

Open source is not easy. If this project is helpful to you, you can consider buying the author a cup of coffee. Your support is the biggest motivation for developers to continue maintenance!

> It is recommended to use Alipay, but an avatar is not available for WeChat. Please note "Mind Map" in the message/remark when committing the transfer.

<p>
  <img src="./web/src/assets/img/alipay.jpg" style="width: 300px" />
  <img src="./web/src/assets/img/wechat.jpg" style="width: 300px" />
</p>

<p>
    <span>
        <img src="./web/src/assets/avatar/Think.jpg" style="width: 50px;height: 50px;" />
        <span>Think</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/志斌.jpg" style="width: 50px;height: 50px;" />
        <span>志斌</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/小土渣的宇宙.jpeg" style="width: 50px;height: 50px;" />
        <span>小土渣的宇宙</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/qp.jpg" style="width: 50px;height: 50px;" />
        <span>qp</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/ZXR.jpg" style="width: 50px;height: 50px;" />
        <span>ZXR</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/花儿朵朵.jpg" style="width: 50px;height: 50px;" />
        <span>花儿朵朵</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/suka.jpg" style="width: 50px;height: 50px;" />
        <span>suka</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/Chris.jpg" style="width: 50px;height: 50px;" />
        <span>Chris</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/水车.jpg" style="width: 50px;height: 50px;" />
        <span>水车</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/仓鼠.jpg" style="width: 50px;height: 50px;" />
        <span>仓鼠</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/千帆.jpg" style="width: 50px;height: 50px;" />
        <span>千帆</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/才镇.jpg" style="width: 50px;height: 50px;" />
        <span>才镇</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/小米.jpg" style="width: 50px;height: 50px;" />
        <span>小米bbᯤ²ᴳ</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/棐.jpg" style="width: 50px;height: 50px;" />
        <span>*棐</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>Luke</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/布林.jpg" style="width: 50px;height: 50px;" />
        <span>布林</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/南风.jpg" style="width: 50px;height: 50px;" />
        <span>南风</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/蜉蝣撼大叔.jpg" style="width: 50px;height: 50px;" />
        <span>蜉蝣撼大叔</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/乙.jpg" style="width: 50px;height: 50px;" />
        <span>乙</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/敏.jpg" style="width: 50px;height: 50px;" />
        <span>敏</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/沐风牧草.jpg" style="width: 50px;height: 50px;" />
        <span>沐风牧草</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/有希.jpg" style="width: 50px;height: 50px;" />
        <span>有希</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/樊笼.jpg" style="width: 50px;height: 50px;" />
        <span>樊笼</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/达仁科技.jpg" style="width: 50px;height: 50px;" />
        <span>达仁科技</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/小逗比.png" style="width: 50px;height: 50px;" />
        <span>小逗比</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/天清如愿.jpg" style="width: 50px;height: 50px;" />
        <span>天清如愿</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/敬明朗.jpg" style="width: 50px;height: 50px;" />
        <span>敬明朗</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>飞箭</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/戚永峰.png" style="width: 50px;height: 50px;" />
        <span>戚永峰</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/moom.jpg" style="width: 50px;height: 50px;" />
        <span>moom</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/张扬.png" style="width: 50px;height: 50px;" />
        <span>张扬</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/长沙利奥软件.jpg" style="width: 50px;height: 50px;" />
        <span>长沙利奥软件</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/HaHN.jpg" style="width: 50px;height: 50px;" />
        <span>HaHN</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/继龙.jpg" style="width: 50px;height: 50px;" />
        <span>继龙</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/欣.jpg" style="width: 50px;height: 50px;" />
        <span>欣</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>易空小易</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/国发.jpg" style="width: 50px;height: 50px;" />
        <span>国发</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>建明</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/汪津合.jpg" style="width: 50px;height: 50px;" />
        <span>汪津合</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>博文</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/慕智打印-兰兰.jpg" style="width: 50px;height: 50px;" />
        <span>慕智打印-兰兰</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>锦冰</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/旭东.png" style="width: 50px;height: 50px;" />
        <span>旭东</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/俊奇.jpg" style="width: 50px;height: 50px;" />
        <span>俊奇</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/橘半.jpg" style="width: 50px;height: 50px;" />
        <span>橘半</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/pluvet.jpg" style="width: 50px;height: 50px;" />
        <span>pluvet</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/皇登攀.jpg" style="width: 50px;height: 50px;" />
        <span>皇登攀</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/风格.jpg" style="width: 50px;height: 50px;" />
        <span>风格</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>SR</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/逆水行舟.jpg" style="width: 50px;height: 50px;" />
        <span>逆水行舟</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>LiuJL</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/L.jpg" style="width: 50px;height: 50px;" />
        <span>L</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>sunniberg</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/在下青铜五.jpg" style="width: 50px;height: 50px;" />
        <span>在下青铜五</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/木星二号.jpg" style="width: 50px;height: 50px;" />
        <span>木星二号</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/阿晨.jpg" style="width: 50px;height: 50px;" />
        <span>阿晨</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>铁</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/庆国.jpg" style="width: 50px;height: 50px;" />
        <span>庆国</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/Alex.jpg" style="width: 50px;height: 50px;" />
        <span>Alex</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/子豪.jpg" style="width: 50px;height: 50px;" />
        <span>子豪</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/宏涛.jpg" style="width: 50px;height: 50px;" />
        <span>宏涛</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/最多5个字.jpg" style="width: 50px;height: 50px;" />
        <span>最多5个字</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/雨馨.jpg" style="width: 50px;height: 50px;" />
        <span>雨馨</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/ZX.jpg" style="width: 50px;height: 50px;" />
        <span>ZX</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/峰.jpg" style="width: 50px;height: 50px;" />
        <span>峰</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>协成</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/木木.jpg" style="width: 50px;height: 50px;" />
        <span>木木</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/好名字.jpg" style="width: 50px;height: 50px;" />
        <span>好名字</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/Kyle.jpg" style="width: 50px;height: 50px;" />
        <span>Kyle</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/lsytyrt.jpg" style="width: 50px;height: 50px;" />
        <span>lsytyrt</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/秀树因馨雨.jpg" style="width: 50px;height: 50px;" />
        <span>秀树因馨雨</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/buddy.jpg" style="width: 50px;height: 50px;" />
        <span>buddy</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>小川</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/Tobin.jpg" style="width: 50px;height: 50px;" />
        <span>Tobin</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/夏虫不语冰.jpg" style="width: 50px;height: 50px;" />
        <span>夏虫不语冰</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/晴空.jpg" style="width: 50px;height: 50px;" />
        <span>晴空</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/default.png" style="width: 50px;height: 50px;" />
        <span>黄泳</span>
    </span>
    <span>
        <img src="./web/src/assets/avatar/ccccs.jpg" style="width: 50px;height: 50px;" />
        <span>ccccs</span>
    </span>
</p>
