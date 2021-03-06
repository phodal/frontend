# 前端地位

> 前端困境三步曲之前端地位

最近的，最远的最近，或者说在过去的几个月里，我与几个前端同事，一直在讨论一个话题：『作为一个前端开发人员，我们面临怎样的困境？又该如何去解决？』。

而在较老的一次历史讨论（可能是在 6 小时以前）里，我便想重新理清一次其中的思路，也就有了这篇文章。

## 前端是不是没有地位？

答案：不是，也是。

当我们在技术领域，技术团队，讨论地位的时候，说的实际上是话语权——技术的话语权，KPI 的话语权。技术话语权，是因人而异，当你可被信赖时，你就有了话语权。而 KPI 话语权，实际上指的是 title。

1. **来得晚的前端没有 Title**。Title 是一个很有意思的东西：**先到先得**，你去了一家高速发展的创业公司，你的 title 就升得很快——站在风口，大象都能飞。而，大部分 Web 应用，前期注重的往往都是应用的功能，这也导致了：这些组织在前期并不需要优秀的前端开发。而发展起来之后，便开始追求用户体验、视觉效果、多平台，到了这个时候呢，关键的坑位已经被后端占据了。毕竟好的前端很贵，但是能实现页面的前端到处都是——甚至是后端也是。

2. **后端懂点前端，而前端不懂 CRUD**。事实上，大部分的组织对于团队负责人，都有一个默认的要求：『精通』整个系统——无论是前后端。这就意味着，前端需要懂后端，后端也需要懂前端。所以，一个不懂后端的前端，站不到 title 上；一个不懂前端的后端，站不到 title 上。可是呢，对于普通的开发人员来说，要达到中等前端水平的时间花费，要比后端少得多。而如果放到大前端的领域来考虑，这个问题就需要额外商榷了。

PS：懂后端也并不要求，你精通后端。因为最好的篮球教练，并不要求会打篮球。而打篮球最好的不一定会当技术负责人/Coach，比如——科比被女儿怼：“你不会打篮球，教练是这么教我的” 。当然了，有技术底子是最好的，但是它也可能在一定程度上限制你。

3. **需求导向**（可选）。对于服务型公司，如我司，需求方决定了架构的复杂性，决定了其所需要的 title。而需求方对于架构、复杂度的考量，往往是来自于整个市场的平均知识水平。也就是说，一旦业务方需求不复杂，也就不需要高级的前端开发，便谈不上就不话语权。

综上所述，若是想争取地位需要：去得早，懂后端，机会好。

扯太远了，那么继续往下扯。

## 5 个因素决定前端

### 1. 复杂度，决定前端

同样是做一个手机，诺基亚的功能机，和 iPhone 有不一样的成本。

项目的业务人员/产品经理/产品负责人对于产品的需求，出因此决定了应用/产品的复杂度。诸如于，同样是一个搜索功能，它有不同的实现方式：

1. 普通模式。前端生成搜索的 URL，跳转到对应的搜索结果页。
2. 标签搜索 + 普通搜索。后端返回标签
3. AutoComplete + 普通搜索
4. AutoComplete + 标签搜索 + 普通搜索
5. AutoComplete + 地图搜索 + 标签搜索 + 普通搜索。对了，还要有地图和标签的联动。
6. AutoComplete + 地图搜索 + 标签搜索 + 普通搜索 + 热门搜索。
7. ……

复杂度，决定了对于优秀前端工程师的需求。也因此在某种程度上，决定了前端的话语权。比如说，『出于设计上的需要，决定了后端应该这么做 xxxx』

也因此，诸如于腾讯这样的产品型公司，前后端都没有地垃。

但是，它避免了后端决定了前端需求的要素——这一点非常重要。在产品话语权不高的团队，必然是先到先得的后端管理者，决定了整个产品的走向，也由后端决定了前端的设计。

### 2. 团队规模，决定前端

只有组织内的前端团队达到一定的规模，才能迫使组织的管理者意识到：『我们需要更优秀的前端开发，才能解决当前的瓶颈』。

按 xx 划分：

 - HTML 5 广告页
 - 小型前端应用（微信小程序）
 - 中型前端应用（普通的 Web 应用）
 - 大型前端应用（toB）

按团队规模来划分：

 - 页面级
 - 6 人团队
 - 两个 Pizza 团队级
 - 组织级

所以，如果你只是在切图，如果你只是在画 HTML5

### 3. 流水线式开发

大型组织，需要更明确的分工，以便于机械工的生产更多的应用。

也因此需要更明确的分工，来解决效率的问题。

 - 工具支撑团队
 - 框架开发团队
 - 业务开发团队
 - DevOps 团队

### 4. 客户端多样式

在最近的几年里，前端走向大前端的原因也在于此，对于多种客户端开发的需求：微信小程度、桌面客户端、跨平台应用等等。使得一个个前端开发人员，身为多技。

作者手疼，省去了几十个字。

### 5. 新的领域

嗯，只有新的领域，才存在更多的机会。

1. 边缘计算
2. 区块链
3. 客户端计算
4. ……

作者手疼，省去了几十个字。

### 6. 业务熟悉度

如果你不关心业务，对业务不了解，那么你哪来的自信，去领导整个前后端团队。

作者手疼，省去了几百个字。

## 结论

言而总之，总而言之：只有优秀的前端，才有必要讨论地位。抱怨，解决不了问题——只有起而行动，才能有效地解决问题。

这些也意味着，我们需要更深入的学习。笑~ :)

可是，到底从哪里开始学呢？有没有一本书，能解决这样的问题。

