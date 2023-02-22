## 新增的一些知识点
---
### 软件需求(Software Requirements)的各种范围
- 软件需求范围的大小排序：**Epics > Features > Product Backlog Items > Tasks**
- ***Epic***: Epic是最大的一个需求范围，这个范围是可以被分割成各种小需求的，它是对customer requirement/demand的一种更高级的描述（不过这个我还不懂它指的high-level是啥意思），而且这个范围的东西是可以对stakeholder这个级别的利益相关者讲工作原理的，举个例子：====在网上书店中，顾客可以购物、购买书籍；店长可以管理店铺的整体运营，使店铺运营顺畅，让顾客对服务感到满意；管理员（指网站技术层面的）可以维护整个站点，使书店的运行安全可靠====。然后整个Epic层次需要遵循SLAP原则，即单一抽象层次原则，这个站点讲得比我更好：[聊聊软件开发的SLAP原则 - 掘金 (juejin.cn)](https://juejin.cn/post/7082951399058702343)
- ***Feature***: Feature就是一种比Epic小的需求范围了，是客户所需要实现的需求，比如====客户想要在网上书店中能够实现在线支付====，应该还是比较好理解的
- ***Product Backlog Items, AKA PBI***: 比Feature更小的一个范围，进一步详细定义实现这个Feature需要做啥，比如====客户想要在这个网上书店里用支付宝支付====，这个范围是可以在一个Sprint（这个玩意的定义见[[一些Y3S1讲过的知识点和开发可能要用到的方法]]）里被实现的
- ***Tasks***:这个就好理解了，就是做啥来实现PBI中的要求，比如====我要在支付界面加入支付宝支付的选项====，这些在课件里也是有例子来解释的
### PBI是什么/PBI里面包括了哪些东西？
- PBI ID
- Priority
- Effort
- Title
- Story
- Acceptance Criteria(验收标准)
- Grooming Information(就是增加一些前面环节被遗漏掉的信息)
- 一些会包括Discussion和Related PBI
### PBI的大小到底有多大？
- 小的一逼啊，小到可以直接在一个Sprint里完成，或者说，一个Sprint里面应该有好多个PBIs。一个PBI是易于理解和实施的，一个PBI只有一个要完成的目标
### 验收标准里面包括了什么？
- 验收标准是一段充分列举了用户需求和产品所有应用场景的文字，是用来呈现用户意图而不是解决方案的，它描述了可以实现的合理的需求，是产品要实现的最小的功能块，举个例子：====User story说作为一名注册用户，希望在计费页面上能够看到会员到期日期，以便知晓何时需要手动续费会员或者开启自动续费====，那么验收标准便是====计算会员到期日期；显示会员到期日期；日期格式是YYYY-MM-DD；如果用户未注册/认证，那么就不会显示会员身份的详细信息====，Formatted地说就是====如果注册用户在访问计费页面时经过认证，那么系统将以YYYY-MM-DD格式计算并显示会员到期日期====。课件page26有一个比较详细的例子
### Sprint
- 关于Sprint，在[[一些Y3S1讲过的知识点和开发可能要用到的方法]]已经提到了一部分
- Sprint是很典型的Agile method，一个Sprint周期一般也就从W1D1开始到W2D7结束，满打满算14天的流程，也有一些3 weeks和4 weeks的Sprint（--课件，我在youtube上面看到的好像不是这个时间长度，不过也差不多就是了），在一整个周期中有**Sprint Planning, Sprint Execution, Sprint Review, Sprint Retrospective**这四个环节。按顺序来，====Sprint Planning在所有行动开始前执行，在三小时内完成，整个开发团队都要参与，会议内容包括当前Sprint所要达成的目标、要在当前Sprint完成的PBI、谁来完成，需要多少时间来完成每个涉及到的PBI、然后参考模板，在Sprint Backlog里记录下所有的信息====。之后就是执行，然后是Review，====Review是开发团队和stakeholders之间的会议，来审查当前Sprint的结果，但是我们这个小bAssignment是没有stakeholders的，所以我们自己做review。一个review两小时内完成，主要审查结果是否符合要求，如果不符合可以要求在之后的Sprint重做那些不符合要求的PBI部分。====Review基本上就是对内容的审查，后面的Retrospective部分才是对这个做的过程的总结。====这一部分主要包括的是对整个Sprint大伙的完成情况、态度、Sprint流程合理性啥的进行总结，和Review部分不同的是这个part不是审查技术，而是总结经验的。在这个part里还有一部分要做的事情就是确定意见和建议，并且提出在下一个即将要做的Sprint里要改进的三个点，也是在两小时内，最好可以控制在一小时内完成。====

`Sprint部分有点长，但是Lecture 1的内容到这里就结束了。`
`LMO已经上传了我们会用到的几个文件：Sprint Backlog Template，Product Backlog， Product Backlog Item Template，Individual Contribution Form`