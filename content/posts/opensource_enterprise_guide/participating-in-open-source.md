---
categories:
- 开源
- 企业指南
date: 2018-10-30T23:04:26+08:00
description: "企业想拥抱开源，就像是中国古代武术界的“江湖”，你首先得证明自己是心甘情愿要融入这个生态的，而不是上来就是另外成立门户，说自己的项目开源了，一副救世主、施舍的样子，这样失败的几率太大！所以要去贡献！证明自己！"
keywords:
- Open Source
- Culture
- Reading
- News
tags:
- 开源企业指南
- 开源之道
title: "Linux基金会企业开源指南系列之五 —— 公司如何以利益最大化的姿态参与开源社区"
url: ""
---
## 特别声明

本文拥有创作共用授权之相同方式共享授权4.0版国际许可协议（Creative Commons Attribution ShareAlike 4.0 International License）授权许可。 开源之道独立精心翻译分享，欢迎同道中人商讨。


# 参与到开源社区

开源已经是构建软件的事实上的方式，这不仅体现在 IT 技术本身，而且跨多个行业。那么企业一旦使用开源代码来构建他们自身的商业产品和服务，那么就应该考虑参与到项目中去，而且要提高到战略的高度。

那么问题来了，如果没有正确的理解项目、社区，以及开源项目是如何运转的，就开始参与开源，就可能会带来不好的影响，不仅是贵公司，甚至也会波及到社区。就开源而言，一家公司若是没有将之列为战略上的考虑，就冒然的去进军开源，可能会犯错，进而影响公司在开源社区的声誉，甚至会招来法律上的风险。

本指南涵盖了作为一个组织去贡献开源，以及如何成为一个好的企业员工。并且会说明一些其它开源相关知识，如开源项目的组织结构、如何做贡献、为什么说内部的开发者参与开源是有益的、以及为什么说开源的参与和管理提高到战略高度是非常重要的事情。

## 为什么要贡献开源？

如今已经几乎不可能找到没有从开源软件受益的公司或组织了。有些公司如Intel、IBM、三星等，均是设立了专门的开源项目部门去专门贡献开源社区的，而还有的公司之所以成为了开源的用户，完全是因为他们的系统管理员或开发者在工作中出乎意料的引进的。

很多公司都在商业上依赖开源软件，而且还获得了很大的成功，所以他们也懂得和明白为开源软件项目做贡献。我们来看一组数据，从2005年，截止到现在，单单Linux内核一个项目，就有来自1300个不同的企业的13500位开发者参与了贡献。

> “对于很多大型项目来说，红帽知道我们大多数的贡献者均是来自实际使用开源项目的其它公司的人们，如Ceph、Gluster等。红帽有自己的客户，而且这些客户也经常会贡献项目，因为他们在使用这些项目。红帽认为无论是个人参与还是公司参与，都是值得诉说的成功。” [Stormy Peters](https://twitter.com/storming) – Red Hat开源社区领导者高级经理

![](https://linuxfoundation.cn/wp-content/uploads/2017/08/Linux-kernel-contributors-graph.jpg)

或许有一部分的企业的贡献仅仅是为了回馈社区，但是仍然有很大一部分企业有更为充足的理由去贡献开源项目的，因为内部使用了相应的项目贡献会获益更多。这里列出几个贡献上游的益处：

* **吸引人才：** 当贵司依赖开源软件，那么寻找人才最好的地方莫过于熟悉项目内部本身，而且还是项目社区成员。通过在社区的公开的工作，贵司可以吸引到一些既是做自己喜欢的工作，还能获得一定报酬的人。尤其重要的一点，贵司现有的项目参与的员工，每天都会和他们在一起打交道，自然是非常熟悉的，找到他们也很容易。（更多详情，请参考招聘开发人员指南系列）
* **降低维护成本：** 如果一个企业开始在本地的分支做缺陷修复、增加新的功能，然而却没有将这些代码提交到上游的开源项目中，那么很快维护本地的分支，将成为该公司的一个成本噩梦。将上游作为优先的提交缺陷修复和增加新功能是最为明智的做法，因为这样的维护成本最低。
* **项目影响力：** 在一个开源的项目中，新的特性或功能来自社区的贡献，那么这些贡献就会影响到项目的走向，如果你认为为项目所贡献的新功能对于贵司非常的重要，那么你应该去安排积极的贡献者对这些功能进行开发和实现。通过贵司的贡献，自然而然就可以影响到项目的走向（只要你的变更符合项目本身的目标）。

当然，参与社区是需要适当的方式方法的，若是方式不当的话，那么就可能出现不可预料的问题，即使真正的做了贡献。每个开源项目在具体的规范、期望和流程上都有一些细微的差别，所以贵司在参与一个项目之前，首先要做的就是去了解这些项目。这点可以有多种方式来完成，如先安排员工加入社区并花时间和精力去实地的考察，又或者是直接在该社区招聘已经有了贡献记录的参与者，进而了解项目本身。

## 开源项目是如何被管理的？

如果你是第一次接触开源项目的话，可能看起来它们混乱不堪。对于开源完全不了解的人来说，一群来自世界各地的"乌合之众"，将那些不知道是什么的代码“扔”在一起，竟然能够开发出让数百万人使用的稳定产品。但是，当他进入到开源的世界，了解了一阵子之后，会发现，开源软件的开发和维护工作也是有理可循的。其实几乎每个开源项目都有良好的组织架构，而且优秀的项目往往会在其项目主页或文档中清晰的将组织架构和社区治理方式描述出来。（GitHub 的开源指南有针对贡献者提供的良好的[项目分析](https://ocselected.github.io/open-source-guide/how-to-contribute/#orienting-yourself-to-a-new-project))。

虽然说各个项目的治理模式有着千差万别，但是综述起来，它们还是有一些共同点的：

* **领导者：** 一个项目，必须要有人承担起决策的事情，如特性、发布、以及日常活动。最为极端的情况，某些开源项目就仅仅是一个人，比如 Linus Torvalds，作为内核的创始人，对于Linux Kernel相关的任何事务都拥有最终话语权。然而在另外的一些项目中，可能有一个或多个委员会负责项目的各个方面，如 Node.js 项目采用的是核心技术委员会机制（the Core Technical Committee）。
* **维护者：** 大多数开源项目的领导者（上一条）会将一些决策委托给负责维护项目特定部分的开发者，而在大型项目中，这些维护人员还可能将其中部分工作委托给其他负责人员。例如，Linus Torvalds将 Linux Kernel 文件系统的相关决策权就委托给 Jonathan Corbet。
* **提交者：** 有一些开源项目还会设置一组可以直接提交代码到主干的人，他们已经证明了自己可以胜任工作并且靠谱，而且往往并不是先去提交给维护者去进行审核。当然，作为提交者，仍然对于代码没有最终的决定权，维护者或项目的领导者如果发现了什么，还是可以将提交的内容打回去的。
* **贡献者：** 有很多人为开源项目贡献代码、文档、以及其它事项，这些贡献通常都需要更为有经验的提交者或维护者进行审核之后方能合并的。这也就意味着贡献者的决定权范围更小一些。
* **使用者：** 其实从某种程度上讲，开源项目的实际使用者才是对项目的成长和开发是最为重要的，这些使用者或者称用户的人们，为项目提供了终极目标，并且帮助项目持续的进化，他们作为社区成员最具价值的部分莫过于针对功能提供反馈、报告缺陷、并建议些什么。

社区对于开源项目来说，犹如古人说的：“水能载舟亦能覆舟”，社区对于开源项目的成功至关重要，但是若是做的不好的话，它同样可以让一个项目置于死地。所以，要努力的去建设一个强大的、充满活力的且多样化的开源社区，这是项目的成功充分必要条件。以上列出的这些角色也是属于社区的一个部分而已，这里未列出的其它重要角色还有文档、营销人员、技术支持等等。

## 贡献是怎么进行的

贡献的流程要视具体的项目而定，可谓是五花八门，缤纷世界。这里仅列举其中一些较为典型的例子：

* 一般项目会针对代码风格、语言、格式、bug/ticket 号、发布时间等等信息给出相应的向导和指南。
* 有些项目会让贡献者签署一个协议，而有些项目会要求署名，也有其它各式各样的。
* 还有一些较为古老的项目是使用邮件列表来提交补丁的，当然现在很多项目都使用 GitHub 的 PR 了。

以上只是列举出来不同的贡献风格的其中一小部分内容，所以作为贡献者的你，想要明白具体项目的具体规则，还是去读一读实际的文档吧。很多项目均在代码仓库的主目录下包含了 **CONTRIBUTING** 这个文档，也有的是直接写到了 **README** 文件中的，有的或许需要你去深入文档或者是网站介绍社区的部分才能发现具体的规则。这样也好，让你去阅读一下整个项目的文档，如社区指南、行为准则等等，这样能够确保你更加完整的理解特定的项目。

如果你是头一次为开源项目作贡献，你或许应该考虑寻找一位导师，或者更有经验的项目成员，他们可以审核你的工作，并为你提供一些反馈，尤其是在准备阶段。

当在文档中详细说明了提交贡献的流程之后，那么接下来要做的事情，就是倾听反馈的声音，并要做到响应及时。常见的反馈包括一些诸如某些事项是如何运行的、为何选择此类方式等等问题，还有就是一些改进的建议或变更请求。有的时候，人们会问一些刁钻的问题，可能回答起来比较的棘手，不过没有关系，凡是要往好处想，这些人之所以提交这些反馈，是因为他们是很在意这个开源项目的，你真实而坦率的回答即可。要避免采取不理睬的姿态处理。

当人们提交了代码之后，在正式被采纳并合并到主干，是需要经历一番波折的，甚至会有被拒绝。这都是常见的合理的现象，维护者一般均会给出合理的解释，假如被拒绝了，没有关系，及时的进行沟通，要去虚心的了解自己的被拒绝的真实原因，通过进一步的修正，争取下一次被采纳。

这里仍然要提醒的是，请记住，如果你的共享被采纳了，后续的维护工作还需要你来做。这对于相对比较大的贡献，如新的功能特性或者是独立的代码模块显得尤为重要，拿Linux内核来说吧，比如提交的是一个特定的硬件的驱动程序。当然，如果相对较小的贡献，如修复一个字符串的拼写错误之类的，就没有必要进行长期的维护。

## 企业参与贡献意味着什么

多年以来，关于开源项目、使用或参与贡献该项目的公司之间的关系并非是那么的明朗。这其中一大原因就是，公司通常建立业务关系的方式并不适合于开源项目，所以，一些公司对于如何富有成效的为开源做贡献是很犯难的。

还有另外一个大的挑战就是，当公司自身的需求和开源项目的需求并不一致的时候，企业会做出利己的决定，或者是认为是烫手的山芋而置之不理。那么这样就会导致开源合区对该公司背后的动机产生怀疑。过去大量的实践验证，确实有很多的案例说明一些公司曾经尝试做出和开源项目目标不一致的地方，而且在其中某些项目中，还确实发生了社区对公司严重的信任危机。

然后，历史的结果证明，还是有很多个成功的案例的。其中之一就是大名鼎鼎的 Linux 内核项目，在此项目中，各家公司以卓有成效的方式进行着积极的贡献。所谓的公司为开源项目做贡献，最为常见也是最为简单的方式就是让自己的员工花大部分甚至的全职的时间到开源项目中，而且公司为这些员工提供薪酬。当然，为了让这样的方式行之有效，这些属于公司的员工需要了解开源项目的贡献流程和行为准则，从而提高他们的贡献被采纳的几率。

如果贵司是刚刚开始接触开源项目，或者干脆是刚接触开源，那么应该考虑招聘一些拥有相关经验的，而且在贵司想要参与的项目中拥有一定知名度的人，如果能够幸运的招聘到他们，那么就会大大加快贵司参与项目的速度。不要有什么顾虑，那些社区的工作者可能非常愿意作为导师来帮助你的员工，因为他们也希望自己的职业生涯更为的顺畅。（更多招聘内容，请参考招募开源开发者一章。）

![](https://www.linuxfoundation.org/wp-content/uploads/2017/08/Kubernetes-contributors-pie-chart.png)

上图为CNCF旗下的种子项目Kubernetes 参与的多样化的公司/组织分布饼图

当然，以上所谈并不是唯一的企业参与开源的方式，还有很多种方式可以参与，而且还要根据具体不同的项目而做出调整。开源项目及其相应的基金会所需要的一些资源，是企业可以提供的，如基础设施、基金、市场营销、法律服务等等。还有的一些开源项目让公司以提供资金和人员的方式来参与，作为回报，公司可以获得项目中一些顾问的角色，或者是提升企业的曝光率。

这里举一个例子，[Node.js 基金会](https://foundation.nodejs.org/) 的董事会成员就是由企业成员代表、技术指导委员会代表、以及个体成员选出的代表组成。其中包括哪些仅仅通过赞助金额的公司成员，他们赞助的金额在 5000美金到250000美金不等。虽然每个项目的赞助资格或会员资格的获取方式不同，但是为开源项目提供资金有助于开源项目支付其日常的开支，为项目的成功添砖加瓦。

## 作为公司员工参与开源项目该如何平衡社区与雇主

此话题算是本篇指南的主要题旨，当然这是开源的主要力量在，尽管对于每个项目具体的内容是有些差异的。这也意味着你每次参与一个开源项目，都需要花一些时间去了解该项目并且学习它工作的方式。

对于一个组织或公司参与开源项目的话，意味着就不可能有一个全能的条条框框为员工提供指示，而是要让员工自己去到具体的开源项目去参与并学习。不过这里有一些可以给出指导的几条建议。

* **加入社区：** 每个社区均有不同的参与模式和渠道。请仔细阅读社区的文档进行了解，而且要加入关键的社区渠道，比如邮件列表、论坛、IRC、Slack、缺陷跟踪、源代码仓库等。
* **先潜水：** 当你加入一个社区以后，需要“潜水”一阵子，去走心的学习，在你正式的开始贡献之前，阅读一些归档文件，以了解项目的文化。你需要在参与之前要去了解社区的规范和期望。越多花时间和精力去阅读和倾听，你的首次贡献被认可的机会就会越大。
* **理解社区治理：** 在贡献之前，要去阅读文档和网站的那些关于项目治理的章节和领导力章程，你需要了解谁能够做出决策以及如何做出决策，就不同类型的贡献而言。
* **千里之行，始于足下：** 以解决一个小的缺陷，或者是修复一个文档错误来开启你的开源贡献之旅是个不错的选择。因为这是学习流程较易上手的方式，而且这个更正错误的小的贡献对于怪四的需求不是那么的严重。在不太重要的较小贡献上犯错误，及时改正并积累经验，然后逐步发展到有能力做出组织需要的更为复杂的贡献。

经历了上述步骤之后，说明贵司已经可以为社区做一些小的贡献了，但是贵司的目标肯定不仅如此，那么接下来，就要“玩点”大的，要去在项目中产生更大的影响力。

* **在线下活动上打造更好的关系：** 无论是个人的关系，还是公司之间的联系，对于参与开源社区来讲都是很重要的。其中一个很好的结识其它社区成员的几乎就是参加线下活动，在开源社区平时大家都是靠电子邮件或及时聊天来保持联系，如果能够有机会见面，没有什么比这更加有效和令人激动的沟通方式了。通常这下线下活动能够吸引各色各样的社区成员，从项目的领导者到产品的热心用户均会悉数到场。当然，这里顺便要提及的是，这些线下活动有赞助商的慷慨解囊是无法进行的，正式因为有了他们，所以可以让开源社区的人们聚在一起，相互学习、探讨项目，进而打造出成功的项目。
* **要尽早、经常的参与社区：** 有很多公司会在开源项目的时机上犯同一个错误，那就是先是在公司内部进行了大量的开发工作，然后觉得“完美无缺”了，才将之开源到互联网上。这样的方式一般均会以失败而告终。事实上，开源项目是很复杂的，哪怕是看起来似乎比较明显的一个小的变更，但是它可能影响到项目的其它部分，所以任何的变更，都应该经过社区的其他成员的讨论或审核，以确保它是无害的，而且要确保所解决的问题是和项目的目标一致的。所以，在你花时间实现代码之前，就将之放在社区上进行讨论，这有助于聚焦问题本身，而不是你的单方面的实现。（这方面可以参考 Jon Corbet撰写的[如何参与到Linux内核社区](https://www.linux.com/publications/how-participate-linux-community)。）
* **贡献上游：** 本条指南的意思是，**请将任何贵司对开源项目的改动提交到原始的维护者哪里，以便于维护者在下次发布版本时将贵司的变更采纳。** 如果贵司是新加入开源的，那么就要花点时间去培训员工，和大家讲清楚上游贡献的重要性。最为常见的一个误区，就是想当然的认为自己的修复是那种“快而脏”的代码，只是适合于自己的环境，没有必要提交到上游去。这就是欠债的最大预兆。然而，速成的补丁需要在每次升级周期中被测试、更新、重新接受等，而这消耗的时间和精力是非常大的，所以这类行为在社区内部是被认为是非常自私自利的，或许有些组织能从这些速成的补丁中受益，但是从长远的角度来看，贵司的声誉还是会在开源社区中受损。

### 为上游贡献代码的最佳实践

#### 在贵司的内部

1. 以合适的原因去决定上游。
2. 始终坚持上游优先的代码设计和实现。
3. 采用“上游优先”策略。 即首先要去上游提交补丁，将贵司的产品作为下游。
4. 保持您的开发人员一直参与到开源项目中，哪怕是一些零星的参与。

#### 面向项目之外

1. 确保贵司的贡献对于他人是有用处的。
2. 遵守相应的代码风格。
3. 参与项目提交流程的制定和维护。
4. 针对贵司的贡献者，为他们提供文档和相应的解释。
5. 听取反馈，并采取相应的行动。
6. 保持耐心并反复修改代码直至被接受。

对于企业参与开源，其中最大的挑战莫过于让众人理解在开源项目中影响力是需要赢取的，而不是靠什么行政制度之类的。或许某人在公司内是个“人物”，但是开源社区是不看这些的，在没有赢得任何尊重之前，谁也不会在乎你在公司的头衔的。**影响力来自于参与！** 人们持续的为开源项目做贡献最终赢得了影响力颇大以及领导的位置，是因为他们用事实证明了自己的靠谱和责任心！

另外需要提醒的一点是，在参与开源社区的过程中，必须准备好随时都有冲突的可能性，在遇到之前你最好有所准备，免得到时候显得惊慌失措。尤其是当有些贡献者对于决策、方法论以及贡献的风格有不同的看法时会在审核流程中变得异常的激烈。这个时候一定要表现的冷静和专业，要确保争执聚焦在问题本身，而不要发生人生攻击之类的。要记住，你是参与到公开的开源项目，而且会永久的保留在互联网上，一场失控的争执，可能会让一些组织或个人困扰你很久。正式因为这些参与都是非常公开的，所以为新手们培训一些诸如如何和不同的人进行沟通、解决冲突的办法等等是一个很好的开始。

## 如何制定开源贡献策略

一个经过深思熟虑的开源贡献策略，不仅可以很好的帮助贵司的员工参与到开源项目中，而且还可以向贵司管理层汇报工作有着清晰的脉络。在开始时，尤其重要的一点是审视贵司的整体业务目标，从而能够让开源的相关努力能够很好的适应贵司战略性意义。（具体请参考创建开源业务战略的指南。）将开源贡献策略很明确的联系到整个公司的战略，不仅可以让高级的管理层了解工作的重要性，而且可以帮助员工对于自己的贡献的效用有一个明确的了解。

> “ 将开源作为企业战略重要的一环获得管理层的支持和认同是非常重要的，作为开源项目办公室的负责人的你要去真正的理解公司的目标，并将之融入到你的开源战略中！” [Nithya Ruff](https://twitter.com/nithyaruff) – –Comcast开源实践高级经理

贵司一旦制定了和公司主体的业务目标相一致的目标和策略，那么接下来就是进一步的具体实现了。以下所列出的内容或问题，可以很好的帮助开源项目办公室思考、捋顺，从而实现自己的设想：

* **为什么这些贡献很重要？** 这一步往往会被直接忽略，大家会直奔主题：赶紧的去实现计划啊！但是，且慢！最好是再多问几遍，你是否找到了参与开源项目对于贵司具有战略意义的重要论据？
* **贵司内部都用到了那些开源项目？** 花一些时间评估一下贵司（整体）现在已经在使用的开源项目，从而确定那些项目对于贵司的业务是具有战略意义的。所评估的内容需要聚焦的几点：关键业务基础设施（运营）、影响产品发布的开发和部署工具、以及那些面向客户的产品或服务很重要的软件。
* **那些项目是贡献的目标？** 多数公司都会使用大量的开源软件项目，所以确保计划能够聚焦到最终重要的项目上是非常重要的，（所谓的”好钢要用到刀刃”上。-译者注）假如说某开源项目对于贵司的业务非常重要，它的任何差错都可能引起严重的宕机或中断为客户服务的能力，那么这个项目就应该成为贵司参与贡献的候选目标。另外需要和大家讲清楚一点的就是，那么没有列出来的开源项目就不能贡献，它可能只是非贵司重点所关注，偶尔“客串”一下，有益无患。
* **贵司已经为开源项目做了什么？** 在很多情形下，贵司已经有员工早已为开源项目作了一下修复或变更的工作了。他们可能只是自己为某个版本打了几个补丁，也可能是将补丁提交到了上游以避免自己去维护。花一些时间和内部团队了解实际的情形，并对他们是否具备贡献开源的技能和兴趣进行一定的评估。
* **贵司是否已经具备相关的经验，如果没有的话要不要招聘专业人员？** 正如上面所讨论过的，能够找到一位具备贡献上游技能的工程师、或者是有能力让上游社区接受贡献的人，对于企业是非常重要的，如果贵司已经拥有了贡献某项目的相关开发者，那么就积极的支持他们就好了，如果没有的话，就该考虑去招聘那些能够为社区做贡献的工程师。这点和任何其它的计划一样，需要确保拥有充足的预算，是成功的充分条件！
* **贵司需要多少用于项目赞助资格/企业会员资格的资金？** 贵司所选择的项目的治理模式是什么类型的？因为只有考察了开源项目的治理模式，才需要考虑企业会员资格、为项目做赞助、以及赞助基金会等等，因为这些开源项目接受资金的捐赠，从而帮助项目取得成功。另外在一些情况下，参与这些可以帮助贵司以顾问的方式参与到项目，也可以帮助贵司提高对项目的影响力。另外，除了这些直接的资金支持之外，还可以考虑相关技术研讨会，因为这些技术会议，是宣传贵司的工作成果的最佳之选，而且技术会议也是“面基”——遇到想要的人才的最佳之地。
* **该如何提高开源的工作效率？** 为开源项目的贡献做营销或推广，做出具体的区分是蛮难的事情，这取决于贵司本身的立场。正因为如此，才愈发显得在公开的地方讨论贵司的贡献对于实现计划是多么的重要。赞助项目、在项目的技术会议做演讲这些都是推广工作的好途径，这对于让人们知道贵司正在做的事情或者是招聘到贡献者都是有益的。特别地，不要忽略参与贡献的有贵司员工的本地用户组。赞助这些本地的用户组，而且让贡献者们做分享可能是一个招聘到特定开源项目开发人员的好方法。
* **需要什么样的贡献者指南或流程？** 指南或流程要尽可能的少一些规章制度，因为这些内容的本质目标是帮助人们可以成功的贡献到开源中，它最好是为人们提供所需要的一些指南或清单项，确保不会发生许可、保密等违规行为，还成功的为开源项目做了贡献。当然，这些指南尤其对于新手有用，在Ta们正在提交之前，按照指南或流程来做事情，可以有效的避免不合适的行为。
* **应该提供何种类型的培训？** 针对开源贡献的最佳实践、开源的许可证、开源治理、以及一些参与开源社区的日常规范，这些培训都是必要的。培训诸如冲突解决、对付难缠的人员、以及一些必要的技能对于日后的社区维护是有益处的。当然，随着时间的推移，贵司还应该提供更多的内容，如为新的贡献者提供富有经验的贡献者做导师的计划等等。
* **如何确定计划是在成功的路上进行的？** 每个计划都应包含成功的标准，而且要有能够衡量目标实现的方式。这些内容应该直接来自于贵司的战略，当然要确保追踪这些活动是对于贵司是重要的，而不是那些看起来很花哨的内容。这里推荐一个工具 -- [GrimoireLab](http://grimoirelab.github.io/)，用于衡量和追踪开源项目的工具，而且它本身也是开源项目。（更多关于衡量的内容，请参考本指南系列之 —— [度量开源项目的成功要素](/posts/opensource_enterprise_guide/measuring_open_source_program)
* **贵司是否需要专门的开源项目办公室来有效的支持所有的开源工作？** 毫无疑问，拥有开源项目办公室或者是专门的人来负责实现以上这些计划，要比没有强很多。退一万步，即使贵司不会设立专门的开源项目办公室，也不会安排专门的人手，那么至少也要负责将上述的流程和培训落实了，以及提供许可证指南，回答管理层或贡献者的一些问题，甚至是和公司之外的进行沟通。（关于设立和创建开源项目办公室，请移步[创建开源项目办公室](/posts/opensource_enterprise_guide/creating-an-open-source-program)一文。）

## 开源贡献的11条黄金准则

如何在公司内为开源贡献打造健康的环境：

1. 为开源贡献创建政策和流程上的指南
2. 设置专门的团队来为所有的开源贡献进行监督和批准
3. 在特定的领域聚焦于贡献，有助于技术的更进
4. 为开源的贡献提供必要的 IT 基础设施和工具
5. 为员工提供最佳实践的培训
6. 要去跟踪贡献，衡量诸如改进、沟通、影响等等
7. 建立导师机制，以帮助那些受训经验较少的开发者
8. 提供贡献向导指南、动手实践、倡导的行为，以及禁止的行为等
9. 开源的法律支持可以让开发者们访问到
10. 从开源社区雇佣人才，更能体现价值
11. 要去遵守社区的流程和实践

## 写在最后

开源项目就在那里，它在很多的企业为其客户交付其产品和服务时扮演着重要的角色。如果贵司能在开源项目中拥有较大的影响力，那么对于贵司的成功就有很大的裨益，那么显而易见的就是去积极的参与到开源项目中去。请定制靠谱的贡献策略和实现的计划，进而成为优秀的开源中的一员铺平道路！加油吧！

## 贡献者

![](https://www.linuxfoundation.org/wp-content/uploads/2017/08/stormy_thumb.png) [Stormy Peters](https://twitter.com/storming) – Red Hat开源社区领导者高级经理

![](https://www.linuxfoundation.org/wp-content/uploads/2017/08/Nithya_thumb.png) [Nithya Ruff](https://twitter.com/nithyaruff) –Comcast开源实践高级经理

> 这些资源是与TODO（公开对话，开放式开发）小组 – Linux基金会的专业开源程序网络小组合作创建的。 特别感谢那些贡献自己的时间和知识来制作这些综合指南的开源项目经理。 参与的公司包括Autodesk，Comcast，Dropbox，Facebook，Google，Intel，Microsoft，Netflix，Oath（Yahoo + AOL），Red Hat，Salesforce和Samsung。 要了解更多信息，请访问 [todogroup.org](http://todogroup.org/)。我们邀请您在GitHub上下载、传播，如果可以请积极的参与这些指南。
