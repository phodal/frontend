# 大前端


## 什么是大前端？？

> 大前端是指通过 Web 开发相关的技术（WebView、JavaScript/TypeScript）所能开发、处理的领域。除了包含传统的 Web 前端相比，大前端还包含了——后端（Node.js 如 BFF 层、Serverless）、HTML 5 游戏、物联网、嵌入式应用、移动应用、桌面应用。它的显著特性是：**一次开发，多种平台**。

值得注意的是：对于某些领域而言，大前端技术并不是最好的技术，但是它是实现起来最快的技术，也因此特别适合于 **MVP 原型构建**。与此同时，前端技术的动态特性，特别适合于远程更新业务——只需要更新对应的代码，而不需要更新整个应用。



若是就这样领域，在前端里，我们可以分为多个领域。

### 大前端的技术领域

#### 前端中的 Web 前端

#### 前端中的 GUI

前端是软件 GUI（图形用户界面）的一种形式。从传统的应用厂商，到互联网应用的迁移，我们便可以看到相关的变化。

#### 前端中的游戏

#### 前端中的物联网（IoT）

#### 前端中的移动端

#### 前端中的 AR/VR

### 选题

**适合对象**：

**简介**：

# 大前端：前端

前端领域，在 2018 年已经趋于平衡，Angular、Vue、React 都没有出现太大的变化。

## Web 应用

### SPA （单页面应用）框架：A/V/R

架构选型上，也趋势于平衡。该用啥的还是用啥，偶尔还是会出现一些框架切换的新闻。尽管在 2019 年，会出现一些新的框架，但是还不太可能快引起变化。

### MPA （多页面应用）框架

## 数据可视化


## 语言

### TypeScript

TypeScript 真香。

前端，没什么好看——除了，娱乐新闻。

# 大前端：GUI

## 桌面浏览器

## 移动设备浏览器

## 嵌入式设备浏览器

# 大前端：后端

所谓的前端 in 后端，便是**在后端开发中，使用前端相关的语言和技术栈**。最典型的场景，便是使用 Node.js 开发后端服务。虽然 Node.js 已经有了 10 年的历史了，但是以我（Phodal）的角度来看，我更希望的是使用编译型语言，来开发后端服务。动态语言，无法使用编译器来检测错误，难以约束代码变动。

## Node.js 打造后端服务

从社区的探索来看，存在一些完全使用 Node.js 开发的后台服务。但是，也存在一系列由于代码不规范造成的问题。从社区的经验来看，Node.js + Express + MongoDB + Angular/Vue/React，便是一些不错的选择。当然了，也有相当多的应用，只是采用了 Node.js 来完成 BFF 层（Backend For Frontends）。在这一层业务上，它只做业务数据的中间处理。

虽然，我经常建议在一些关键的节点上，不要采用 Node.js 来打造后台服务。可一旦涉及到 SPA 的服务端渲染，我们就不得不使用 Express、Koa 等这样的服务端 JavaScript/TypeScript 框架，来解决这样的问题。

## Serverless

> Serverless 架构是指大量依赖第三方服务（也叫做后端即服务，即“BaaS”）或暂存容器中运行的自定义代码（函数即服务，即“FaaS”）的应用程序，函数是无服务器架构中抽象语言运行时的最小单位。在这种架构中，我们并不看重运行一个函数需要多少 CPU 或 RAM 或任何其他资源，而是更看重运行函数所需的时间，我们也只为这些函数的运行时间付费。[^serverless]

[^serverless]: [https://serverless.ink/](https://serverless.ink/)

作为一种折中方案，也是我最喜欢的方案。Serverless 架构是指大量依赖第三方服务（也叫做后端即服务，即“BaaS”）或暂存容器中运行的自定义代码（函数即服务，即“FaaS”）的应用程序，函数是无服务器架构中抽象语言运行时的最小单位。

对于没有后台经验的前端开发人员来说，使用 Node.js 开发后端应用是一种相当大的挑战。大多数非科班的前端程序员，不知道从数据库到 RESTful API 的一系列操作，并且还需要了解到部署等一系列的系统底层知识。因此，使用 Serverless 这种不关心基础设施的技术，可以进一步地降低开发成本。


采用 Serverless 架构，也就意味着，我们提取出了大量的基础设施。而使用 Node.js + JavaScript 作为胶水，来快速连接不同的服务，以形成一个快速有效的方案。并且，编写更少的代码，也意味着更安全、快速。

使用 AWS 来运行大量的 Serverless 计算的成本很高，但是自己搭建一个 Serverless 服务器，来运行自己的 Serverless 应用，则变成了一种更廉价的方式。除了直接基于 AWS 的 Serverless Framework 框架的方案，还有 OpenFaaS、Kubeless、OpenWhisk、Fission 等不同的 Serverless 框架。

## BFF 层

> BFF，即 Backends For Frontends (服务于前端的后端)，也就是服务器设计 API 时会考虑客户端的使用情况，在服务端根据不同的设备类型，返回不同客户端所需要的结果。BFF 模式，这种模式不会为所有的客户端创建通用的 API。而是创建多个 BFF 服务：一个用于 Web 前端、一个用于移动客户端（甚至一个用于 iOS，另一个用于 Android）等等。[^aofe]

[^aofe]: 前端架构：从入门到微前端

# 大前端：游戏

随着移动端的性能不断变好，在 2019 年，我开始看好使用 HTML 5 技术来开发一些游戏。当然了，主要原因还是微信小游戏的出现。但是，不管怎样，我开始尝试在这个领域的探索。

## WebView 游戏

## JavaScript 语言游戏

# 大前端：IoT

我刚实习的时候（2013 年），项目里使用的是 Backbone，作为单页面应用框架的核心来打造 Web 应用。这时，我开始关注于 Node.js，使用它实现物联网应用的可能性。当时，已经有了物联网协议 MQTT 和 CoAP 相关的库，便照猫画虎地写了一个支持 HTTP、CoAP、WebSocket 和 MQTT 的物联网。由于，当时缺乏一些大型应用的开发经典，所以做得并不是很好，但是已经可以看到 JavaScript 在这方面的远景。

一年多后，Ionic 也还没推出正式版，便发现到了这个框架真的很棒——它自带了一系列的 UI 组件，还用 NgCordova 封装了一系列  Cordova 的插件。便开始使用 Ionic 写了一些移动应用，发现还挺顺手的。接着，便拿这个框架尝试写物联网应用，这需要一些原生的插件，如 BLE、MQTT。后来，我也写了一个简单的 CoAP 插件。

后来，我们不再需要编译 Node.js（早期，使用的是 Raspberry Pi 来运行 Node.js），就可以在 ARM 处理器上运行 Node.js。并且我们已经有 Tessel、Espruino、Kinoma Create、Ruff 这些可以直接运行 JavaScript 的开发板。三星还推出 IoT.js，可以让更多的嵌入式设备，直接使用 JavaScript 作为开发语言。

人们开始在硬件上使用 JavaScript 的原因有很多，如 Web 的开发人员是最多的，而 JavaScript 很容易上手。

## 嵌入式前端

Android 是用得最多的嵌入式系统，。

OpenWRT 是用得最广泛的嵌入式系统之一，

在某些资源受限的设备上，我们无法运行一个带着完整 JavaScript 引擎的 WebView——出于软件体积、运行内存等因素的限制，去除了这些特性。诸如 CSS 3 中的动画特性，会占用大量的运算资源，算去掉了相应的支持。

## 固件编写

### Johnny-Five

### IoT.js

# 大前端：移动端

## 混合应用

依我的角度来看，使用什么跨平台框架来看，区别并不是太大。目前主流的方案，仍然是原生（含跨平台框架） + HTML5 应用。从业务的角度上来看待这个问题，那么还是希望，可以用 HTML 5 的地方多——更新功能方便。

也因此，虽然在过去，笔者写过基于 React Native 的混合应用框架 Dore。我相信：Flutter 也会出现这样的混合应用框架。不过，对于有原生开发能力的团队来说，它们的框架还会是三部分：

 * 原生功能部分
 * 原生 + H5 的频繁更新部分
 * Fultter 的跨平台部分

写业务嘛，框架都只是工具。

## 跨平台应用

### React Native

### Flutter

### Weex

## 小程序

小程序，即 HTML5 小程序，即无需安装即可下载运行的应用程序。与普通的移动 Web 应用不同的是，**小程序相当于是高阶版的混合应用**。

如果只是从这一点上来看，其实是不是和微信一样的定制型小程序，并不是那么重要。重要的，在于与原生**界面结合，并提供离线使用功能。**它也是小程序与普通的 HTML 应用的区别。

# 大前端：桌面应用

## 跨平台框架

## 跨平台框架

# 大前端：VR/AR

## VR

## AR


