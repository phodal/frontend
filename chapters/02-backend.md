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
