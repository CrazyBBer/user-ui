# 如何选择合适的框架

![公平](./logo.png)

## 我为什么从不公开进行比较？

无论是在公司还是社区，都曾有人让我拿Angular和React进行比较。而我的答案只有一个：我没法告诉你。

原因有三：

1. 我不是React的专家。除非我的React水平和Angular的水平相同或更高，否则我没有资格做出比较。
2. 我无法绝对客观。即使我的React水平和Angular水平一样高，有了比较的资格，我也不愿意公布这些比较。原因很简单，我无法做到绝对客观，而带着主观偏见做出的比较会误导使用者。
3. 我的情况不适用于你。每个人都有他自己的技术背景，对我来说最好的选择，对你未必最好。

如果有一天我把Angular和每一项竞争技术都做了比较，并且让你一看就决定选择Angular而觉得其它技术都很Low，那么只会有一个原因：我被盗号了。

作为一个崇尚客观、公正、理性的程序员，我无法容忍自己堕落到那种程度。

## 任何刻意的比较，都是诡辩术

事实上，只要剥离了应用场合和使用者背景，宣扬优点并隐瞒一切缺点，那么我很容易就能让新手们相信jQuery胜过一切前端框架。不信？来看这个 <http://vanilla-js.com/> 。如果你是初出茅庐的新手，而某个骨灰级老鸟给你一个片面的观点，那么你很容易被误导，更何况诡辩者本来就是从你这个阶段走过来的，很容易利用人性的缺点击败你。

然而，新手虽菜，却不傻。

有一天你会发现：

- 宣称简单的框架可能扩展性很成问题，而被贬低的框架已然经历了很多年的实践检验。
- 宣称资源丰富的框架可能只有一系列低质量库，而被贬低的框架实际上不需要第三方资源就能完成大部分工作。
- 宣称代表了技术趋势的框架可能招不到几个可用的人才，而被贬低的框架可以让从刚毕业到资深的团队成员都能充分贡献自己的力量。
- 宣称轻量级的框架在复杂场景中可能很快会成长为恐龙，而被贬低的框架越是在复杂的场景中越如鱼得水。

所以，广告法中明令禁止贬低对手，其实正是为了保护消费者，防止不够知情的消费者被误导和伤害。然而软件业并没有这样的法律，但我们至少要有公共的职业道德和个人的内心操守 —— 我们都是骄傲的程序员，一切靠事实说话，不屑于玩弄诡辩术。

## 我们应该怎么做？

1. 我们可以热情洋溢的宣扬自己喜欢的技术，但是不要对其它技术进行贬低 —— 就算你真是双料专家，你也做不到客观公正。

1. 不要玩儿那种“断章取义”或“攻其一点，不及其余”之类的诡辩术。

1. 不要撒谎！知道的就说知道，不知道的就说不知道，不要利用语言上的模糊性和歧义去误导他人。论文学，估计没几个程序员赶得上我，但是我在技术文章中总是力求精确表达，不屑于玩弄文字游戏 —— “你没看懂，怎么能怪我”这种话我可说不出口。

1. 不要隐瞒！由于侧重点不同，可能不会每一篇文章都面面俱到，既谈论所有优点又谈论所有缺点，但是总体上要平衡。你是某项技术的专家，不可能不了解他的缺点，隐瞒缺点不说，事实上就是在坑新手。这种事情，配不上我高傲的心。

1. 场景！场景！场景！任何一项技术都有自己适用的场景，在不同的场景下，其应用效果也不同。包治百病的神药只有大力丸。

1. 背景！背景！背景！不同的技术对于不同背景的程序员，其适用程度也不同，如果你觉得某种背景对于你掌握这项技术有加分项，那么请明确说出来，以便别人更加准确的判断它对自己是否同样有参考价值。

1. 基于事实而非“感觉”。这是对专业性的基本要求。“感觉”是一种主观臆断，如果谈论“感觉”，那么永远不会有结果，而是会陷入像语言大战那样的“信仰战争”、“口水战”。只有事实才能帮新手们判断“这是否适合我”，而不是“我喜欢这个演讲者，所以我选这项技术”，然后掉在坑里。

## 范例：Angular 2技术选型指南

### 下列情况下请“不要”选择Angular 2

#### 需要支持IE8

Angular 2明确放弃了IE8，如果你不得不支持IE8，请选用支持它的技术。

#### 内存敏感的应用

Angular 2的应用至少需要占用30M内存，更复杂的应用会占用更多。如果在你的应用场景中30M内存已经非常珍贵，请慎用Angular。

#### 开发团队缺乏后端背景且缺乏Angular 1背景

Angular 2引入了很多来自后端编程领域的实践，这些对于缺乏后端背景并缺乏Angular 1背景的开发团队来说可能会有很高的学习成本。

#### 极客团队

Angular 2倾向于采用成熟、大众化的技术，虽然把AoT等技术引入前端也算新颖，但是这可能无法满足极客团队的追求与探索欲望。

Angular 2在设计上内置了很多最佳实践，这些最佳实践对极客团队来说可能是一种束缚，而如果试图突破束缚可能会导致烂代码。

### 下列情况下你不需要有顾虑

#### 性能

如果你曾用过Angular 1，可能有性能方面的顾虑，但是Angular 2升级了实现原理，主观的说：提高了500%的性能，客观的说，在Table-Report等测试中处于第一梯队，与React等在性能上胜负各半。

#### 难度

Angular 2大幅简化了Angular 1的概念模型和编码方式。

Angular 2也引入了AoT等很多新技术，但它们都是Nice to have的，可以等你的产品需要追求极致时再去研究。

#### 你的“信仰”

如果你是Redux的信徒，那么不用担心，Angular 2可以很好地与Redux集成。

如果你是ReactNative的信徒，那么不用担心，Angular 2可以很好地与ReactNative集成。

### Angular 2适用于下列情况

注意：说“Angular 2适用”并不代表其它框架不适用或更差，请自行判断。

#### 需要长期保持API稳定的系统

事实：

1. Angular 1保持着良好的语义化版本（semver）维护记录，从1.2可以轻松升级到最新的1.5，而不会被迫修改代码。
1. Angular开发组给出了关于版本升级策略的明确承诺。他们采用的是在后端世界经过多年检验的最佳实践，参见 [流言终结者！Angular的版本与发布](../流言终结者！Angular的版本与发布)。

期待：

1. 你可以期待Angular开发组今后会按照可预测的方式进行升级和维护。
1. 你可以期待Angular的当前主版本会有一个稳定的生态圈。
1. 你可以期待Angular的下一个主版本的生态圈会同步成长，与Angular的新版本同步或稍后推出。

#### 具有深度后端背景的团队

事实：

1. Angular与后端世界共享了很多概念，如依赖注入、注解/装饰器、强类型、接口、TDD等，具有后端背景的程序员可以很快掌握这些核心概念。
1. Angular采用了从传统的MVC模型衍生出的MVVM模型，熟悉Spring等框架的程序员可以很快理解它。

#### 人员流动性较高的团队

事实：

1. Angular默认采用TypeScript语言，具有强烈的类型约束，可以防止新人提交低质量的代码。
1. Angular有一份官方发布并维护的风格指南（有中文版），其中包括了一系列最佳实践及其考量，这让Angular程序员很容易达成共识，具有相似的代码风格。

#### 由少量高手和较多新手组成的团队

事实：

1. Angular通过依赖注入体系分离了服务和组件，并在架构中广泛使用了AOP风格的设计（如路由器的Guard），这让不同水平的程序员可以很容易的实现分工，实现杠杆效应。
1. Angular是高度模块化的。不同模块之间隔离得很充分，不会相互干扰。除了由高手维护的公用模块之外，应用模块的错误不容易扩散。
1. Angular是高度局部化的。组件的逻辑和CSS样式封装很严，组件之间不会互相干扰。
1. Angular的官方文档非常全面，而且有与官方文档同步更新的中文文档，非常适合新手入门或作为参考资料。

### 其它信息

#### 充满活力的社区

事实：

1. 我们的微信公众号在Angular刚发布后的这一个月内增长了2000多位关注者。
1. 我们的微信公众号的“查看/关注”比大约是25%，这说明我们推送的文章阅读率很高。
1. 我们在一个月时间内招募了50位驻站作者及见习作者，这说明我们的社区参与热情很高，可持续性比较强。

期待：

1. 你可以期待Angular中文社区继续茁壮成长。虽然Angular在2016年中秋才正式发布，但是我们有Angular开发组和谷歌技术推广部的大力支持，有充满技术热情的推广者和写手，你可以期待等到它一周年的时候会交出一份令人震撼的成绩单。
1. 你可以期待Angular中文社区的成败不会取决于某一个人。我们已经初步建设了一个社区人才梯队，分工体系也正在形成，未来会逐步脱离个人的推动而实现自主运营。

#### 大量的潜在人才

事实：

1. 我们的Angular中文官网在Angular发布一个月之后达到了每日20000+的PV，这说明有很多人对此项技术感兴趣。
1. 如前所述，Angular适合传统后端学习，从而转型为全栈工程师，增加了团队配置的灵活性。

期待：

1. 你可以期待未来会有大量基于Angular技术栈的新前端。
1. 你可以期待未来会有大量资深后端转型而来的前端，他们的设计感、架构观等放在前端也同样是资深的。而前后端的API协商成本为零。
