# 为你的软件工程团队编译飞行规则

> 原文：<http://www.effectiveengineer.com/blog/flight-rules-for-software-engineering>

在他的书《宇航员在地球上的生活指南 中，克里斯·哈德菲尔德分享了他从成为第一个在太空行走的加拿大人的看似不可能的旅程中学到的感悟。他讲述了他为太空做准备而进行的现实模拟的故事，讲述了他在国际空间站 6 个月任务中的日常生活，甚至讲述了宇航员如何在太空刷牙的机械原理。

给我留下特别深刻印象的是哈德菲尔德描述的一部惊人的知识巨著，一部人类花了几十年才完成的巨著。“自 20 世纪 60 年代初以来，美国国家航空航天局一直在记录我们的失误、灾难和解决方案，”他写道，“当时水星时代的地面团队首次开始将‘经验教训’收集到一份简编中，现在列出了成千上万个有问题的情况，从引擎故障、舱门把手破裂到计算机故障，以及他们的解决方案。”

这个概要被称为*飞行规则。令人惊讶的是，你可以在网上找到这些规则 A 卷 2200 多页的副本。给定一组特定的环境，手册一步一步地列举，做什么和为什么。冷却系统出现故障？*飞行规则*一步一步告诉你怎么修，以及每一步的基本原理。燃料电池问题？*飞行规则*告诉你发射是否需要延期。“它们是非常详细的，特定场景的标准操作程序，”哈德菲尔德继续说道，包含了从过去的任务中吸取的所有经验教训。*

这么多有价值的知识可以塞进一本手册，这让我不禁想知道:在一家软件工程公司，类似的手册会是什么样的？拥有一本手册会让我们做些什么？当然，它会为我们的系统制定一步一步的操作规则。MySQL 数据库故障？*飞行规则*会告诉你如何从主设备故障转移到从设备。服务器因流量超载而超载？规则会告诉您运行哪些脚本来增加额外的容量。

但是它也可以有更多如何运行项目的通用模式。项目进度落后？*飞行规则*可以告诉你[过去不同的项目团队加班时发生了什么](/blog/why-overtime-doesnt-work)，那些团队认为他们最终成功或失败的主要贡献者是什么，以及团队成员是否精疲力竭。有新的排名算法的想法吗？你可以在*飞行规则*中找到过去所有 A/B 测试的汇编，假设是什么，以及实验是确认还是拒绝这些假设。

这样的资源看起来非常有价值，尤其是对于新加入团队或公司的人来说。那么，怎样才能到达那里呢？

NASA 的“文化主食”是任务汇报。任务后的汇报提供了回顾任务的机会，以找出哪里出了问题，哪些地方可以做得更好。它们也非常强烈。专家们连珠炮似的提问，每一个动作都被标记出来，并分析出哪里出了问题。4 小时的模拟之后可能会有 1 小时的汇报。太空飞行之后会有一个月或更长时间的全天汇报。你必须稳住自己，等待反馈，记住目标不是让你的错误蒙羞，而是最大化集体智慧。

鉴于发射一架航天飞机的每项任务成本为 4 . 5 亿美元，不难理解为什么美国宇航局认为全面的任务汇报是必要的——无论是从纳税人的钱还是宇航员的生命来看，每个错误都是昂贵的。

大多数工程公司不从事像太空飞行这样的关键任务。许多公司对灵活性的要求和较低的失败成本使得 NASA 的严格程度不可行，就像使用 [*精益创业*](http://www.amazon.com/The-Lean-Startup-Entrepreneurs-Continuous/dp/0307887898?tag=theeffeengi-20) 方法对 NASA 来说不是最好的方法。

但是专注于将集体智慧构建成一套*飞行规则*仍然是一种我们可以在软件工程中更广泛采用的模式。

进行工程事后分析——类似于美国宇航局的任务汇报——是一种相当著名的做法。在站点停机、高优先级错误或基础架构问题之后，工程团队会跟进详细的书面记录，解释发生了什么、如何发生以及为什么会发生，以及我们可以采取什么措施来防止它发生。如果这种情况是不可避免的，建立一个工具来使恢复更容易，或者写一个分步文档来解释下次如何处理这种情况是一个合理的替代方案。许多团队已经倾向于这样做，只是严格程度不同。一些公司如 Asana 和 Amazon 采用类似丰田的“五个为什么”的方法来理解运营问题的根源。

不太常见的是对项目和发布引入相同级别的回顾，并为未来的产品任务汇编经验教训，在整个组织中共享。随着 TechCrunch 的报道，一个功能启动了，香槟杯被碰杯，每个人都为出色的工作而庆祝。但是，这种努力对于实现团队目标的效果如何呢？或者一个团队重写基础设施代码，并在几个月的工作后使其速度提高 5%。这真的是对团队时间的最佳利用吗？如果没有停下来听取汇报和查看数据，很难知道答案。

当然，做得更好会有一些摩擦。团队可能没有为发布定义一个明确的目标或衡量标准，从而很难评估它是否成功。他们可能已经结束了任务汇报，并犹豫是否与组织的其他人分享经验，因为他们不想宣布他们几个月的工作是失败的。或者他们可能只是觉得有太多的事情要做，以至于没有时间思考——这是初创公司常见的情况。我知道我自己也因为加入这些不同的团体而感到内疚。

结果是失去了积累集体智慧的机会。吸取的教训没有被汇编成像*飞行规则这样的概要，*被孤立在少数人的头脑中。代价高昂的错误不断重复。而人走了，集体智慧就减少了。

弥补这种损失需要努力。你必须采取一种开放和接受反馈的心态。你必须专注于增加集体智慧，而不是推卸责任。如果你周围的人也这样做，它可以成为[工程文化](/blog/what-makes-a-good-engineering-culture)的一部分，并减少摩擦，否则这可能是一个可怕的练习。你必须养成回顾自己使命的习惯。