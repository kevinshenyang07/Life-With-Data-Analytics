# 2015年斯坦福创业课程－技术驱动的闪电式扩张(Blitzscaling) 11:Patrick Collison
>**版权声明**
>
>本文首发自微信公共帐号：donglaoshi-123；
>
>作者：沈洋
>
>无需授权即可转载，但请自觉保留以上版权声明。

**主讲人Patrick Collison**

<img src="https://pbs.twimg.com/profile_images/378800000609934413/83919213b96be1b267b6af3a63b7d4d7_400x400.jpeg" style="width: 100px;"/>

>Patrick Collison, [Stripe](https://stripe.com/)联合创始人，十五岁获得科学类奖项，从MIT辍学后创办Auctomatic，次年被加拿大公司Live Current Media收购，十九岁即成为百万富翁。两年后创立支付公司Stripe，获得Peter Thiel, Elon Musk以及红杉资本的投资。

**Stripe的简单介绍**

[估值50亿美元的在线支付创企Stripe，成为了互联网经济隐形的推动力](http://www.tuicool.com/articles/zeqyA3)

[估值暴涨的Stripe如何做网络支付？](http://tech.qq.com/original/biznext/b069.html)

**创立Stripe的过程？**

最开始的时候，我和我的弟弟John Collison会一起开发一些iPhone app来支付我们的学费，当初靠这个赚钱真的很容易。我们在开发的时候养成了顺手做一些小项目（side project）的习惯，然后当我们意识到在其他网站上付款如此让人头疼的时候，我们就想：“为什么不自己做一个支付平台呢？”最开始的时候我们觉得应该很快就能完成，然而五年多过去了我们仍然觉得它不够完善。

2010年的时候我们发布了第一版Stripe并邀请了一些朋友来体验用Stripe付款，开始的推广过程基本是靠口口相传。我很早就加入了LISP编程的社区，期间认识了Paul Graham（LISP大法好），此后我们加入YCombinator，发布了API供开发者使用。因为开始的种子用户很多都是自己创办公司的，所以我们对用户需求有着最直接的了解。

之后我们开始挖掘周围朋友们的资源，联系了一些小型支付公司，但是这一方式扩张太慢，直到我们招到了合适的市场拓展人才，我们才逐渐开始和传统企业以及银行合作。在我们招到第五个员工以后，我遇到了Billy Alvarado（Lala的联合创始人，现已被苹果收购）, 我们当时在想：“这个人不写代码，到我们公司来有什么用？”,但是Billy后来给我们带来了Wells Fargo的业务，成为了我们商务拓展中重要的一员。

<img src="https://cdn-images-1.medium.com/max/2000/1*yuJ_wY1Bo5MxL7ccu2L0vA.jpeg"/>

**Stripe现在的规模？**

我们目前每年的交易额在十亿美元级别，有超过十万家公司在使用我们的服务。我们从创办到现在有五年的时间了，目前有330名员工，是去年的两倍。目前我们仍然采用的是传统的组织和管理形式。我的观点如下：

1. Google/Facebook/Amazon采用的也是传统的方式（说明这并不会影响Stripe的扩张），用其他方式没有必要（会增加时间成本和机会成本）；

2. 没有经验可以借鉴，一旦出现问题难以解决。

当然有些地方还是需要改进的，比如面试。和Google的HR一样，我不认为GPA和进入公司之后的成绩有相关性，在白板上写算法题更是荒谬。我们让面试者带他们自己的电脑，使用他自己喜欢的语言。现在很多时候事物的变化比人的变化更快，人们往往习惯于原来的一套做事方法。


**如何找到优秀的人才？**

我们的产品是面向工程师的，所以工程师对我们有先天的好感。另一方面，对于如何判断一个人是否优秀从来都没有简单的解决办法。我们认为最重要的一点就是，你必须做好花很长时间才能招到优秀人才的准备。最开始的时候，我们花了半年时间才招到两名员工，之后的半年我们又陆陆续续招了三四个人。我们还让应聘者先尝试过来工作，很多都在几个礼拜以后就退出了。

我们撒网的方式是先找到那些优秀的人才，然后再想方设法使他们对Stripe感兴趣。我们在招聘方面极其坚持，我们会花三年以上的时间去和极其优秀的人才不断地沟通，这是其他公司都做不到的。这样的好处是，当我们招来第一个优秀的人才时，在招第二个第三个就会越来越容易。


**感觉你们的产品定位很准确，是这样吗？**

是又不完全是。在早期的时候，我们仅仅提供的是一个信用卡支付的接口，但是在建设好这一基础层后，我们必须针对不同的市场开发出不同的产品。以我们针对集市类型的公司（marketplaces）的产品Stripe connect为例，因为这些公司都有自己的交易系统，我们不得不向每个公司提供不同的接口来满足他们的需求。我们虽然和Paypal看上去很像，但是帮助Lyft（美国打车软件）促进双方的交易和转钱给你的朋友有着很大的区别。我们不仅需要处理交易，还需要考虑退款，小费，额外收费，货币汇兑等一系列问题。

**你们怎么决定下一步做哪些事情？**

这其实是一个很困难的问题。用户其实往往并不知道他们要什么，而且通过分析往往得不到正确的答案。不过我们很幸运，因为开发者们都比较坦率，愿意跟我们直接沟通。尽管如此，我们还是花了很长时间才能辨认出那些对我们的产品有着良好判断的人。

马克·扎克伯格说过：“从一年以内的角度看一件事情可能是可行的，但是从五年以内的角度看可能就行不通。”因此怎么制定优先级相当重要。我们的新产品的想法大约有70%从那些有良好判断的人那里得来，30%则来自那些人们还没想到却又十分重要的事。

**对于比特币怎么看？Stripe为什么会跟比特币联系在一起？**

首先看待事物不能仅仅看它的直接结果。比特币目前规模很小，但是它的一些理念非常吸引人,包括分布式系统，去中心化的基础架构，分类账簿系统（system of ledger）。中本聪的论文不仅仅是计算机科学的突破，同时也是政治哲学的一大进展，所以我们决定帮助比特币发展。

**谁负责Stripe的产品？**

我们并没有独立的技术部和产品部，而是分成一个个小组（原文product engineering teams），每个组都有一个经理，然后我管理这些经理。我个人也会参与到产品开发当中，所以有时候和产品的VP会有交叉管理的问题。

**Stripe有发布产品又取消的经历吗？**

我要再一次感谢我们的开发者客户们。我们在beta版本中就能得到比较详尽的评价，所以我们目前并没有取消某一个产品的情况。但是另一方面，Stripe在规模壮大以后创新的速度有所下降。我们在开发最初的产品的时候只有三个人，但是现在系统已经大到三个人维护不了，所以我们不得不招聘更多的人，给他们培训，让他们融入我们的工作流程。当然，如果你做的足够好，你也可能像facebook一样，在停滞了一段时间后再次快速扩张。

**和现在相比，Stripe有150人的时候和现在有什么区别？**

150人是一个坎。我们不得不采用正式而直截了当的沟通方式，尽管这种方式非常的不自然-比如我们开始说“这是我们第四季度的三个重点”。不过你换一个角度想，创业公司的环境本身就不自然-每过一年你的社交圈就要增加50%到100%，当我们坐在一起讨论的时候，一半的人去年都还没有加入Stripe。这样的好处是，新加入的人会带来新的想法，引发之前已经结束的讨论，坏处是，我们需要花很多时间给新人解释之前的讨论。

也许你会想要深入公司的每个角落，把你的想法传递给每一个人，使得整个公司达成一致，但是我觉得这样又过度了-人们会被吓跑。我觉得很重要的一点是，不要让公司变成你的一言堂，也不要让公司变成做你想做的所有事，而要让公司做正确的事。的确我在打造公司文化上有十分重要的责任，但是我希望公司每个人都能参与进来。

**从开发者转变为管理者感觉怎么样？**

我仍然十分怀念当初写代码的时候。我认为媒体和行业里的人把创始人和CEO的重要性过分夸大了，实际上Stripe是从一个小组转换变了一个大公司，转变的过程发生在所有人身上。

有一个对于CEO工作的概括我认为很恰当：战略、文化、招募高管、产品。这几个方面在开始做的好了，后面就会很容易，要是没做好，却很难修正。这个概括可能太简单了，但是对我来说挺管用的。


**下一期嘉宾**

Nirav Tolia

<img src="https://media.licdn.com/mpr/mpr/shrinknp_400_400/AAEAAQAAAAAAAADuAAAAJDAwYTFjYTVmLTQ2ZmEtNGY1ZS05MDdjLWIxNTk1NTM0MTVkZQ.jpg" style="width: 100px;"/>

>2000年即创立市场研究公司Epinion.com，之后成为天使投资人兼顾问，曾参与包括Zillow，SurveyMonkey等早期投资，2010年重出江湖创立社区社交网络公司Nextdoor.com。

Nirav Tolia的LinkedIn链接：[https://www.linkedin.com/in/niravtolia](https://www.linkedin.com/in/niravtolia)





**补充阅读材料**

[Stripe vs Paypal](https://memberful.com/blog/stripe-vs-paypal/)

[Quora:Why should I switch our websites to Stripe from Paypal?](https://www.quora.com/Why-should-I-switch-our-websites-to-Stripe-from-Paypal)

**本专栏为我的个人专栏，所有观点均为个人观点。如欲转载，请注明出处。如果文章有任何错误或是遗漏，欢迎指正。此外，本文部分图片与内容来自Grey Lock Partners与LinkedIn公开发表的博客与幻灯片，所有参考链接如下。**

[Patrick Collison维基百科](https://en.wikipedia.org/wiki/Patrick_Collison)

[国外学生做的课堂笔记@Note Essays](https://medium.com/notes-essays-cs183c-technology-enabled-blitzscalin/class-11-notes-essay-reid-hoffman-john-lilly-chris-yeh-and-allen-blue-s-cs183c-technology-ebf34cebae26)

