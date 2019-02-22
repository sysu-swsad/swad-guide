---
layout: default
title: 组织第一次迭代
---

# 组织第一次迭代
{:.no_toc}

* 目录
{:toc}

## 1、问题

尽管 [硝烟中的Scrum和XP](http://www.infoq.com/cn/minibooks/scrum-xp-from-the-trenches) 给出了组织迭代（sprint）的一般方法。但是对于一个做创新项目的新人团队几乎完全不适用。团队几乎无法理解以下的准则，即不知道它对应的开发场景，更不知道如何应用？

> 敏捷的过程的实施要点：
>
> Lightweight: ‘Pay as you go.’ Use only the parts that are essential and effective for your project. When in doubt, leave it out.
> 轻量：做能做的事情。仅使用对项目是基础和有效地过程活动。如果你在犹豫，果断放弃它。  
>
> Non-predictive: Requirements and design build gradually as development proceeds rather than being completed before any work can begin.
> 不预测：需求和设计是伴随着开发构建，而不是在其他工作开展前必须完成。
>
> Adaptable: Planning and risk analysis/assessment are on-going and process can be adapted accordingly.
> 灵活：持续开展计划和风险评估，按需调整过程

这时团队状态大概是：

- 乐观者：依然沉醉的愿景的美好，不断设想要做哪些美好的事情
- 悲观者：不断思考哪些内容的实现缺乏把握，技能、技术。。。

总之，无法确定应该做什么，做多少合适（如果这些都知道，显然不是新手团队）。 因此，团队第一个迭代的目标就是用事实树立团队的信心，让乐观者放弃夸夸其谈去做具体工作，让悲观者明白团队的能力。具体问题包括：

* 这个迭代需要做的需求是什么？
* 需要哪些技术原型消除“技术风险”？
* 项目涉及哪些重要的知识与技能？
* 如何进一步细化需求？

## 2、用例故事

用讲故事的手段（自然语言故事），描述通过人机交互达成用户目标的过程。它特别关注用户看到或期望系统处理的数据。

### 2.1 用例建模的制品

* UML Usecase Diagram
* 用例描述
    - 用例文本
        - 简洁的用例文本(Brief)
        - 非正式的用例文本(Casual)
        - 详尽的用例文本(Detailed)
    - 故事板（Storyboard）
        - [User interface-flow diagram](http://agilemodeling.com/artifacts/uiFlowDiagram.htm)
        - [UI Prototypes](http://agilemodeling.com/artifacts/uiPrototype.htm)

### 2.2 使用故事板 与 UI原型

项目策划阶段的设想通常理想而粗糙，也不一定存在有价值的场景，只能作为需求的指引而不是需求。没有需求，技术团队的工作就失去了目标，而去做他们认为有意义的事情。这时，XP 的故事板方法与UI原型技术是最有生产力的！它给出了可信、具体的需求，为本轮迭代的设计、编码、需求与技术验证提供了依据。

* 选择合适 UI 原型工具
* 参照现有产品界面设计原型（不太符合团队设想也没关系，总比自己拍脑袋设计的 UI 强），以后再迭代再修改
* 接近真实的数据对故事板技术非常重要。 很多开发团队只管基本功能实现，使用 admin 或 想象的数据。一旦产品交付用户测试，就发现产品质量低下（要修改的细节太多），导致团队压力过大。

## 3、技术原型

* 搭建一个技术框架，哪怕只有登陆功能
* 在原型基础上实现部分需求功能
* 其他技术验证原型

## 4、技术与技能学习

## 5、项目文档提交！

1、 故事板技术

* 根据你的项目需要，选择一个业务绘制用户界面流草图
* 思考：故事板技术的优点与缺点
* 思考：如何才能使得UI原型的数据接近真实
* 使用 UI 原型工具，将 UI 原型导出为 html 静态，放置在 uideign 的一个子目录下
* 在团队作业 7.1 UI design 下建立一个子标题链接该 UI

**！！！数据、数据、真实数据！！！**

2、团队周任务管理

* 在大作业 git 文档仓库下建立一个XX周任务项目，采用 [To do、Inprogress、Done](https://github.com/sysu-sasd-project/dashboard/projects/1)模板
* 在周末观察该模板，思考：
    - 每个人工作量分配合理吗？
    - 如果出现大面积延期，总结原因，并给出解决方案？
    - 如果多数人都顺利完成了，总结为什么会这么顺利，如何挑战个人极限？ 

3、使用用例点估算工作量

参考：[使用用例点估算软件成本](https://www.ibm.com/developerworks/cn/rational/edge/09/mar09/collaris_dekker/index.html)




