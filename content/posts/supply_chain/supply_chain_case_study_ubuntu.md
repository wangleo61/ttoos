---
categories:
- 开源
- 供应链
date: 2017-05-02T18:25:31+08:00
description: "Ubuntu有着无与伦比的全球开发者和用户社区，产品涉足云平台、服务器、桌面、移动端、项目托管、部署平台等，但是几年下来，开始渐渐的有些力不从心，上个月大变动。那么从社区运营、参与、开源软件上下游等视角来分析一下，它犯了那些不应该犯的错？"
keywords:
- Open Source
- Culture
- Supply Chain
tags:
- 开源相关
title: 这次我们谈谈开源项目得道者多助的Ubuntu犯下的人心不足蛇吞象的严重错误
url: ""
---

### 编译者按

John Mark 先生写了一系列关于开源软件供应链的文章，开源之道打算逐步译出，本文则是系列的中文首篇，其余按排期，稍安勿躁。且并没有按John的顺序，而是先选择了反面的案例，一来是Ubuntu母公司 —— Canonical近来高层变动、产品线浓缩、战略变更等，二来确实也是业内常见的毛病 —— 自大。所以就分享出来和大家一同探讨。

------

## 缘起

在过去的几篇文章里讨论了关于开源软件的供应链管理方面的内容，尤其是一些关于上游项目和下游产品的协作流程。但是均是较正面的例子分析，如企业级OpenStack、利用Docker和Kubernetes等上游项目做容器管理产品等。这次我想尝试一下反面的案例，或者是说如何避免一些常见的错误。是的，讲正面好说，讲反面意味着会惹人不高兴，尤其是在业内，之所以选择Canonical是因为它最近的高层变动、产品线废弃、以及裁掉了一些员工。当然Canonical这么多年还是做了很多优秀的事情的，不能一棒子打死。好，那么我们就先来讲讲那些做的很好的事情。

## Canonical 做对了那些

在2004年，也就是Ubuntu发行版的第一版发行的时候，立即在开源界引起轩然大波，毫不夸张的说，所产生的深远影响是今天的Linux任何发行版都做不到的。回忆下当年发生的事：红帽做出了决定性的转变，花很大努力去搞红帽自己的社区和产品，这让很多红帽发行版的用户感觉受到了冷遇。当时，大家普遍认为Fedora 将会成为红帽的弃儿，会因为资源匮乏而一蹶不振。其实，这一切的发生，都是由红帽自己所扮演的，最初他们对待Fedora确实不怎么用心，几乎将自己在社区的努力毁于一旦。（较为代表性和欢乐的说法，可以参考LWN的归档：[揭秘：Fedora如何和社区交互](https://lwn.net/Articles/83360/))

Ubuntu 从来就没有这些问题，从一开始，Mark Shuttleworth和他的团队对于提供一个易于使用、自由分发的Linux发行版是没有任何疑问的。在Ubuntu之前，有很多人尝试这么做过，但是Ubuntu做到了很多人没有做到的事情。那么究竟是哪里让Ubuntu在别人失败的地方成功了呢？

1. **选择了一个卓越的上游平台** 。Ubuntu 没有像很多发行版那样：要么是从头构建，要么是使用RedHat或Mandrake的衍生品（它们二者均经历尴尬的过渡阶段，一支成为Fedora，一支成为红帽系列），而是选择了坚实可靠、由社区独立维护的Linux发行版——Debian，那时openSuSE还尚未出现，其实基于SuSE去构建Linux，本身就是一个馊主意，因为SuSE和Novell有着千丝万缕的关系。而Slackware已经是在苟延残喘，毫无生气。当然Debian也有一些挑战，至少对于Debian的一些拥护者是自由文化的忠实捍卫者，这就会和像Ubuntu的目的——希望通过Debian做一些盈利的事情，是有一些冲突的。Debian的安装的易用性也是一个问题，而这恰好为Ubuntu提供了很好的机会。
2. **拥有高效的供应链，** 而这一点和上述有直接的关系。从他们所起步的基础设施平台的情况来看，构成Ubuntu的软件供应链是可靠的，开发人员和用户是完全能够在其上面做些事情的。
3. **Canonical在用户体验和社区投入很多。** 其实在Ubuntu出现之前，Linux的使用还是很深奥，且十分吃力的操作系统，Ubuntu的出现改变了这点，从一开始它就定位为“让人们更易使用的Linux”。如果你是计算机科学或电子电器专业的，想利用业余时间鼓捣点什么，那么Ubuntu是最佳选择。Ubuntu Linux发行版比原来任何一个发行版都简单、易用，从供应链的角度来看的话，Ubuntu实现这点是因为它积极的参与了[Gnome社区](https://gnome.org/)的用户体验项目，我知道这么说可能会让Gnome的一些朋友感到不快，但总的来说，Ubuntu曾经是被描绘为Gnome的阵营的，不可否认，Ubuntu对于Gnome的贡献是非常大的。
4. **从一开始就定位于全球化。** Ubuntu的[当地社区](http://loco.ubuntu.com/)(按Ubuntu的说法叫做：[LoCos](http://loco.ubuntu.com/))遍布全球各地，这些社区致力于Ubuntu的传播和并为本地的用户提供支持，这一切都有条不紊，Canonical提供各式各样的工具、广播信息、甚至在某些情况下，采用最原始的方式来进行。Ubuntu还拥有由Jono Bacon领导下的强大的社区团队，可以说Jono Bacon是Ubuntu社区成长的积极推动者和带头人（我个人曾经才OSCON上向大家介绍Jono是如何轻松驾驭Ubuntu社区的，至今印象深刻）。我们简直无法想象，如果这个庞大的全球社区陷入困境的话，对整个上游供应链的影响有多严重。这些全球用户和开发人员数量众多，而且是许多被Ubuntu采用的项目的上游社区的参与者。这是一个积极参与上游的最佳例证！它为开源生态中的每个人（包括Canonical自己）都带来了积极的成果。
5. **Ubuntu是最早采用“云原生”支持的发行版。** 这是Simon Wardley 让人们铭记的一点，Canonical 比其它任何的Linux发行版都更早的引入了“云原生”的负载，在2008-2009年，Ubuntu就成为了很多新兴的云平台和服务器技术的主要和默认的操作系统，一直延续到今天，即使是现在，如果一个新的项目要较早的采用新特性，第一时间会发布.DEB到Ubuntu，且会确保针对Ubuntu的用户的构建是成功的，且能够让开发者下载到源代码。这就给Ubuntu和Canonical带来了不可思议的优势。从供应链的角度来看，这是绝对是一手好牌！这意味着云本地工具的上游供应链是以Ubuntu为中心的，而Ubuntu通过包装是可以做很多事的。

## 又犯了哪些严重的错误

之所以写了Canonical上述的诸般取得的成绩，是不想一下子让读者感觉到Canonical一无是处，因为下面要谈及的内容，才是今天真正要说的，是关于犯错的事情。对于这个以令人难以置信的扩展到全球社区的Linux发行版而言，并没有从其供应链的成功学习到什么，相反却坠入了NIH综合症，相信你已经看到过很多关于针对Canonical批评的言论了，但是本文我仅谈他们关于供应链战略，以及是如何失败的。

1. [Launchpad](https://launchpad.net/)。 作为Canonical建立自己的供应链战略的标志性项目——Launchpad的创建开启了这一里程，这是一个基于Web的服务，用于让开发者来创建、共享、协作软件项目的平台。其还可以执行自动构建的服务，且可让开发者非常容易的发布和管理非官方构建的最新的软件："[个人包归档](https://launchpad.net/ubuntu/+ppas)" 或简称为PPA，无论从时间的把握还是愿景，Canonical的这个项目不可谓不伟大，尤其是随后Canonical声明Launchpad开源，更进一步增加了人气。但是这里隐藏了问题：如Launchpad这样复杂的维护代码库的服务平台确实是太难了。即使[倾公司全部之力](http://github.com/)去实现[这样的理念](http://sourceforge.net/)，都会遇到各式各样的挑战。有几种方法来处理这种复杂性：尽可能的去让上游来承载维护的成本，或者是基于Launchpad建立一个长期的收入模型从而维护其长期的发展，但是Canonical什么也没有做。事实上，Canonical的做法让情况变得更加的糟糕：他们既没有交付给上游，又没有建立收益模型来维持长期发展。换句话说，Launchpad越来越步履维艰，不仅是欠了很多的技术债务，而且仅仅由Launchpad团队来维系，而且还没有得到更多的资金用来进一步的发展。这就是Canonical从业务战略角度出发给人的第一错误印象。糟糕的用户体验，使得Ubuntu用户开始对Launchpad渐渐的失去了信心，将他们的软件开始迁移，而这进一步给了GitHub巨大的发展机会。(译者注：Launchpad创建于2004年，GitHub是2008年。所以作者会有如此一说。)
2. [juju](https://www.ubuntu.com/cloud/juju) 现在讲juju没有前途，可能还为时尚早，但是Canonical和Ubuntu到目前为止还没有显示出会将之打算利用起来，Puppet和Chef已经是成长起来了，而Ansible则是冉冉上升的一颗新星，而juju则是Canonical对于云时代的配置管理这块蛋糕的积极回应。如果Canonical在其用户的基础上在宽松一些的话，可能有非常大的机会。举例来说，Puppet和Chef，均是支持多个平台的，但是juju是捆绑在了ubuntu之下，假如说Ubuntu成为了构建云工具的事实上的标准的话，但企业仍然是由Windows、Unix以及RHEL占主导。开发者或许使用Ubuntu来构建很多工具，但是他们仍然需要将这些工具部署到实际但生产环境中，而juju是无法满足这点的。如果你是一位颇有进取心、年少有为的DevOps专家，那么juju的这种独断方式会断送了你的大好前途。因为它仅仅适用于Ubuntu，而且从来没有进入到Debian的上游社区的核心，juju的影响力非常的有限。Canonical无法与其他开发人员社区建立合作模式，而能够和其它的社区建立合作会大大的提升供应链的效率。还有juju并不能够为创收产品提供附件价值，因为它能够提供的服务能力非常的有限。因此，juju只是Canonical另外一个优秀的项目，却是糟糕的商业策略的典型案例罢了。
3. Unity。 如果说Launchpad和juju让人们意识到Canonical正在脱离正常到轨道的话，那么启动了Unity项目，则彻底的向人们证明了这点。在Ubuntu刚起步的时候，Canonical是[Gnome桌面社区](https://www.gnome.org/)的积极参与者。这是有道理的，因为Ubuntu一直都是基于Gnome的桌面环境。就某种程度上来说，Canonical决定放弃整个Gnome社区是希望能够以自己的方式走的更远、走的更快。与Launchpad和Juju一样，如果Canonical能够通过有效的商业模式，从而获得足够的收入，进而能持续发展，这是行的通的。个人来讲，我很喜欢Unity桌面环境。但是Unity的出现，而其它Linux桌面是推动Gnome3的，这导致了Ubuntu和整个其余的Linux产生了巨大的分歧。和Launchpad、Juju一样，Ubuntu再次将自己的打包者和开发者陷入了孤立，没有上游社区的支持来稳定供应链。这也就意味着，Canonical开发人员再次成为软件的唯一开发者和维护者，这进一步压缩了Canonical欲扩而不能的资源。
4. [Mir](https://launchpad.net/mir)，坦率一点说，我并不知道Mir的起源，但是这已经不重要了。我们只需要知道一点：开源的技术界参与的一个叫做Wayland的项目，这个项目的目标建立X.org窗口服务的继承者。而Canonical再一次和社区分道扬镳，自行构建Mir项目，最后的结局就是Mir和Unity殊途同归，最后的赢家是Wayland。再次验证了供应链法则：从其中学习、习惯其中、热爱其中，否则就是背离、失败。
5. Ubuntu mobile／Ubuntu phone。移动世界的操作系统和服务器、桌面完全不是一个世界，因为其所基于的硬件平台通常都是专用的、封闭的。整个生态系统都是由大型的运营商说了算的。尤其是Canonical所启动的并不是自己所擅长的专业领域，进入的门槛就高些，而且进入市场并没有一个强有力的合作伙伴。如iPhone背后由AT&T在撑腰，至于Ubuntu Phone ，外界看来是没有明确的合作伙伴的。Ubuntu 电话和移动的操作系统，所运行的均是DOA，这点相信Canonical比谁都清楚。
6. Ubuntu 平台自身， 谈到这点，各位看官可能有点诧异，是的，我在本文前面花了大量的笔墨去述说Ubuntu的成功，但是，我没有提到但是大家有所感觉：它没有一处特别出彩：它没有足够大的收入来支撑正在开发的那么多的项目。在Ubuntu应该成长起来的时候，产品方面也没有一个连贯的策略。它是一个云平台吗？移动平台？企业级服务？开发者工作站？而且基于它之上构建的补充项目从来就不够完善，没有做到为旨在创造世界上最优秀的云平台提供一套完美工具的集合，亦或者是最优秀的企业级服务，或者是任何其他的选择。Canonical 尝试让Ubuntu具备各种可能性，可用于各种目的，但是没有做到产品界的铁律，在适当的时候：“说不”！

## 总结

说实话，我罗列上面的Canonical的几步败笔，心情很是沉重。我个人对于Ubuntu所取得的社区成绩，仍然是仰望的态度，但是正是因为爱之切，所以希望它更好！在这个世界上没有几家公司能够获得如此的荣誉，培养了如此巨大的、全球性的用户和开发者社区，他们数以百万计，且几乎覆盖了所有的国家和地区，并且用户和开发者大多具有宗教版的热情。这是巨大的成就，是值得庆贺的事情，也是不可否认的事实。这才是众所周知的Ubuntu、Canonical，当然，还有他们的创始人——Mark Shuttleworth，这并非是短视的商业行为可以做到的。

我并不是说如果没有建立上游供应链，公司就不会成功 —— 有太多的例子可以说明这点。我的意思是想说明，如果手上仅有有限的资源，而且选择了构建多个产品，您将需要来自大量全球参与的间接作用。假如Canonical选择了聚焦于上述产品的某一款产品，你可以认为，供应链不是那么的重要。我要提醒的是，作为记录，以上所列出的任何挑战未必和开源这个事实有关。相反，为了维持其发展，他们需要更广泛的采用。为了维持这一模式，他们必须去创造一个成功的产品，从而获得较高的收入，然而这一天从未到来。

教训：**如果你想掌控自己的软件产品，你就得将自己的产品策略跟随开源。** 如果我在Canonical的话，我会推动一个更加积极的上游战略，以从更广泛的开源参与中获得更多的收益。

## 关于作者
![](https://opensource.com/sites/default/files/styles/profile_pictures/public/pictures/13083153_10153727865327746_5200498137445064668_n.jpg?itok=C6YJqe2I) John Mark Walker 是 Dell EMC 的产品管理总监，负责管理[ViPR 控制器](https://www.emc.com/products/storage/software-defined-storage/vipr-controller.htm)产品，以及[CoprHD](http://coprhd.github.io/)开源项目，他也是资深的开源社区活跃者，如ManageIQ、Gluster、Hyperic，乃至过去的SourceForge。

关于激进的言论，请关注他的Twitter：[@johnmark](http://twitter.com/johnmark)，他也有领英账号：[johnmarkwalker](https://opensource.com/users/www.linkedin.com/in/johnmarkwalker)，也不定期的会更新自己的博客：[johnmark.org](https://johnmark.org/blog/)。

John Mark 经常在各个开源技术会议上做演讲，并有优秀的论述开源的文章，如[根本就不存在开源社区](http://www.onlamp.com/pub/a/onlamp/2006/01/12/no_oss_community.html)、[永远不要搞创新](http://www.johnmark.org/blog/2013/11/it-was-never-about-innovation/)、[逝者如斯：写在VA Linux IPO 十年之际](http://www.cnet.com/news/10-years-gone-the-va-linux-systems-ipo/)。

英文原文：[Supply Chain Case Study: Canonical and Ubuntu](https://osenetwork.com/2017/04/27/supply-chain-case-study-canonical-and-ubuntu/) ，开源之道翻译出品。
