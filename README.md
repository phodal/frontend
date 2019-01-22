# 大前端：前端的扩张

> 大前端是指通过 Web 开发相关的技术（WebView、JavaScript/TypeScript）所能开发、处理的领域。除了包含传统的 Web 前端相比，大前端还包含了——后端（Node.js 如 BFF 层、Serverless）、HTML 5 游戏、物联网、嵌入式应用、移动应用、桌面应用。它的显著特性是：**一次开发，多种平台**。


**适合对象**：任何级别的前端工程师。

**简介**：

## 引子

当我在知乎上回答了一个问题：坚持学前端的你，如今有什么感悟？，我的答案是：
 
----------------------------

 - 2015 年 GET 了 Three.js 和 Oculus，可以开发 VR 应用，于是有了 [oculus-nodejs-threejs-example](https://github.com/phodal/oculus-nodejs-threejs-example)
 - 2016 年 GET 了 Cordova，可以开发混合应用，写了开源应用 Ionic 版本的 [Growth](https://github.com/phodal/growth-ionic)
 - 2017 年 GET 了 React Native 和原生开发技能，可以开发跨平台应用，于是写了基于 React Native 的混合应用框架 [Dore](https://github.com/phodal/dore)
 - 2017 年 GET 了 Serverless，可以快速使用 Node.js 开发后台应用，于是有了 [Serverless](https://github.com/phodal/serverless) 系列的应用。
 - 2018 年 GET 了 Electron，可以写桌面应用了，于是有了自己的 Markdown 编辑器 [Phodit](https://github.com/phodal/phodit)
 - 2019 年 GET 了 Canvas，可以写游戏应用了，于是有了 [Milano](https://github.com/phodal/milano)

所以……VR 应用、移动应用、桌面应用、游戏应用、后台应用。

等等，你说这是前端相关的？方面看并非如此，可实际上却是如此。

----------------------------

喔，我好像不是一个前端，我好像是一个前端。哦，不对，我并不只是一个前端工程师，我是一个程序员，我是一个 Geek，我是一个作者。

总而言之，言而总之：

 - **我是一个程序员，然后才是一个前端。**
 - **我是一个程序员，然后才是一个前端。**
 - **我是一个程序员，然后才是一个前端。**

所以，放下前端程序员这个执念，让我们来看看：只凭现有的前端技术栈，我们又能做些什么呢？ 

## 目录

*   [前言](https://javascript.ren/#%E5%89%8D%E8%A8%80)
    *   [桌面浏览器](https://javascript.ren/#%E6%A1%8C%E9%9D%A2%E6%B5%8F%E8%A7%88%E5%99%A8)
    *   [移动设备浏览器](https://javascript.ren/#%E7%A7%BB%E5%8A%A8%E8%AE%BE%E5%A4%87%E6%B5%8F%E8%A7%88%E5%99%A8)
    *   [嵌入式设备浏览器](https://javascript.ren/#%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%AE%BE%E5%A4%87%E6%B5%8F%E8%A7%88%E5%99%A8)
*   [大前端](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF)
    *   [大前端：写给大家看的渐进式前端发展指南](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E5%86%99%E7%BB%99%E5%A4%A7%E5%AE%B6%E7%9C%8B%E7%9A%84%E6%B8%90%E8%BF%9B%E5%BC%8F%E5%89%8D%E7%AB%AF%E5%8F%91%E5%B1%95%E6%8C%87%E5%8D%97)
    *   [为什么会有大前端](https://javascript.ren/#%E4%B8%BA%E4%BB%80%E4%B9%88%E4%BC%9A%E6%9C%89%E5%A4%A7%E5%89%8D%E7%AB%AF)
        *   [JavaScript 的神奇魔力](https://javascript.ren/#javascript-%E7%9A%84%E7%A5%9E%E5%A5%87%E9%AD%94%E5%8A%9B)
        *   [无处不在的 WebView](https://javascript.ren/#%E6%97%A0%E5%A4%84%E4%B8%8D%E5%9C%A8%E7%9A%84-webview)
    *   [什么是大前端？？](https://javascript.ren/#%E4%BB%80%E4%B9%88%E6%98%AF%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9F%EF%BC%9F)
        *   [大前端的技术领域](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%E7%9A%84%E6%8A%80%E6%9C%AF%E9%A2%86%E5%9F%9F)
            *   [前端中的 Web 前端](https://javascript.ren/#%E5%89%8D%E7%AB%AF%E4%B8%AD%E7%9A%84-web-%E5%89%8D%E7%AB%AF)
            *   [前端中的 GUI](https://javascript.ren/#%E5%89%8D%E7%AB%AF%E4%B8%AD%E7%9A%84-gui)
            *   [前端中的游戏](https://javascript.ren/#%E5%89%8D%E7%AB%AF%E4%B8%AD%E7%9A%84%E6%B8%B8%E6%88%8F)
            *   [前端中的物联网（IoT）](https://javascript.ren/#%E5%89%8D%E7%AB%AF%E4%B8%AD%E7%9A%84%E7%89%A9%E8%81%94%E7%BD%91%EF%BC%88iot%EF%BC%89)
            *   [前端中的移动端](https://javascript.ren/#%E5%89%8D%E7%AB%AF%E4%B8%AD%E7%9A%84%E7%A7%BB%E5%8A%A8%E7%AB%AF)
            *   [前端中的 AR/VR](https://javascript.ren/#%E5%89%8D%E7%AB%AF%E4%B8%AD%E7%9A%84-arvr)
        *   [选题](https://javascript.ren/#%E9%80%89%E9%A2%98)
    *   [如何成为大前端？](https://javascript.ren/#%E5%A6%82%E4%BD%95%E6%88%90%E4%B8%BA%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9F)
*   [大前端：后端](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E5%90%8E%E7%AB%AF)
    *   [Node.js 打造后端服务](https://javascript.ren/#nodejs-%E6%89%93%E9%80%A0%E5%90%8E%E7%AB%AF%E6%9C%8D%E5%8A%A1)
    *   [Serverless](https://javascript.ren/#serverless)
    *   [BFF 层](https://javascript.ren/#bff-%E5%B1%82)
*   [大前端：IoT](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9Aiot)
    *   [传统的物联网](https://javascript.ren/#%E4%BC%A0%E7%BB%9F%E7%9A%84%E7%89%A9%E8%81%94%E7%BD%91)
    *   [嵌入式设备分类](https://javascript.ren/#%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%AE%BE%E5%A4%87%E5%88%86%E7%B1%BB)
        *   [两种前端类型](https://javascript.ren/#%E4%B8%A4%E7%A7%8D%E5%89%8D%E7%AB%AF%E7%B1%BB%E5%9E%8B)
            *   [嵌入式设备作为服务端](https://javascript.ren/#%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%AE%BE%E5%A4%87%E4%BD%9C%E4%B8%BA%E6%9C%8D%E5%8A%A1%E7%AB%AF)
            *   [嵌入式设备作为服务端和客户端](https://javascript.ren/#%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%AE%BE%E5%A4%87%E4%BD%9C%E4%B8%BA%E6%9C%8D%E5%8A%A1%E7%AB%AF%E5%92%8C%E5%AE%A2%E6%88%B7%E7%AB%AF)
        *   [嵌入式设备分类](https://javascript.ren/#%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%AE%BE%E5%A4%87%E5%88%86%E7%B1%BB-1)
            *   [低资源受限设备：编译型语言](https://javascript.ren/#%E4%BD%8E%E8%B5%84%E6%BA%90%E5%8F%97%E9%99%90%E8%AE%BE%E5%A4%87%EF%BC%9A%E7%BC%96%E8%AF%91%E5%9E%8B%E8%AF%AD%E8%A8%80)
            *   [普通嵌入式设备：](https://javascript.ren/#%E6%99%AE%E9%80%9A%E5%B5%8C%E5%85%A5%E5%BC%8F%E8%AE%BE%E5%A4%87%EF%BC%9A)
    *   [固件编写](https://javascript.ren/#%E5%9B%BA%E4%BB%B6%E7%BC%96%E5%86%99)
        *   [Johnny-Five](https://javascript.ren/#johnny-five)
        *   [IoT.js](https://javascript.ren/#iotjs)
    *   [Be Professinoal](https://javascript.ren/#be-professinoal)
        *   [Arduino 与 Processing](https://javascript.ren/#arduino-%E4%B8%8E-processing)
        *   [ESP866/ESP32 与 Lua](https://javascript.ren/#esp866esp32-%E4%B8%8E-lua)
        *   [C 语言](https://javascript.ren/#c-%E8%AF%AD%E8%A8%80)
*   [大前端：移动端](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E7%A7%BB%E5%8A%A8%E7%AB%AF)
    *   [混合应用](https://javascript.ren/#%E6%B7%B7%E5%90%88%E5%BA%94%E7%94%A8)
    *   [跨平台应用](https://javascript.ren/#%E8%B7%A8%E5%B9%B3%E5%8F%B0%E5%BA%94%E7%94%A8)
        *   [React Native](https://javascript.ren/#react-native)
        *   [Flutter](https://javascript.ren/#flutter)
        *   [Weex](https://javascript.ren/#weex)
    *   [小程序](https://javascript.ren/#%E5%B0%8F%E7%A8%8B%E5%BA%8F)
*   [大前端：桌面应用](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E6%A1%8C%E9%9D%A2%E5%BA%94%E7%94%A8)
    *   [跨平台 WebView 应用框架](https://javascript.ren/#%E8%B7%A8%E5%B9%B3%E5%8F%B0-webview-%E5%BA%94%E7%94%A8%E6%A1%86%E6%9E%B6)
    *   [跨平台框架](https://javascript.ren/#%E8%B7%A8%E5%B9%B3%E5%8F%B0%E6%A1%86%E6%9E%B6)
*   [大前端：VR/AR](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9Avrar)
    *   [VR](https://javascript.ren/#vr)
    *   [AR](https://javascript.ren/#ar)
*   [大前端：数据可视化](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E6%95%B0%E6%8D%AE%E5%8F%AF%E8%A7%86%E5%8C%96)
    *   *   [高级娄](https://javascript.ren/#%E9%AB%98%E7%BA%A7%E5%A8%84)
        *   [D3.js](https://javascript.ren/#d3js)
*   [大前端：游戏](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E6%B8%B8%E6%88%8F)
    *   [WebView 游戏](https://javascript.ren/#webview-%E6%B8%B8%E6%88%8F)
    *   [JavaScript 语言游戏](https://javascript.ren/#javascript-%E8%AF%AD%E8%A8%80%E6%B8%B8%E6%88%8F)
*   [大前端：前端](https://javascript.ren/#%E5%A4%A7%E5%89%8D%E7%AB%AF%EF%BC%9A%E5%89%8D%E7%AB%AF)
    *   [Web 应用](https://javascript.ren/#web-%E5%BA%94%E7%94%A8)
        *   [SPA （单页面应用）框架：A/V/R](https://javascript.ren/#spa-%EF%BC%88%E5%8D%95%E9%A1%B5%E9%9D%A2%E5%BA%94%E7%94%A8%EF%BC%89%E6%A1%86%E6%9E%B6%EF%BC%9Aavr)
        *   [MPA （多页面应用）框架](https://javascript.ren/#mpa-%EF%BC%88%E5%A4%9A%E9%A1%B5%E9%9D%A2%E5%BA%94%E7%94%A8%EF%BC%89%E6%A1%86%E6%9E%B6)
    *   [语言](https://javascript.ren/#%E8%AF%AD%E8%A8%80)
        *   [TypeScript](https://javascript.ren/#typescript)
*   [前端，永不止境](https://javascript.ren/#%E5%89%8D%E7%AB%AF%EF%BC%8C%E6%B0%B8%E4%B8%8D%E6%AD%A2%E5%A2%83)

## LICENSE

© 2019 [Phodal Huang](https://www.phodal.com/). This code is distributed under the Creative Commons Attribution-Noncommercial-No Derivative Works 3.0 License. See `LICENSE` in this directory.
