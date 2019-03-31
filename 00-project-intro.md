---
layout: default
title: 实验项目简介与要求
---

# 系统分析与设计实验项目简介与要求
{:.no_toc}

* 目录
{:toc}

## 1、项目实践的内容与目的

项目实践的内容：

* 从一个web或移动应用中选择一个基础业务过程（如订电影票）
* 在应用领域内给出创新内容或元素，提升产品价值

项目实践目的：

* 学习如何定义、描述软件的内容
* 学习面向对象分析与设计方法、设计模式在软件开发中的应用
* 学习使用工具，实现团队有效协作
* 了解软件开发的基本流程

## 2、历年项目实践概述

### 2019 挣闲钱

挣闲钱是大学生通过做任务挣钱的云平台，它属于以运营为中心的服务软件，也可以理解为面向大学生的专业“众包”系统。系统非常简单：有一个云服务中心，其业务在不断完善中；每个学生都装有“挣闲钱”客户端；一些机构，称为“奶牛”，他们提供任务给平台。基本业务是，奶牛发布任务要求与薪酬，系统推送到客户端，学生完成任务可获得系统内部的“闲钱币”，“闲钱币”可用于发布任务或提现。系统不支持零元交易。

挣闲钱系统包括是学生管理系统、任务管理系统、交易管理系统、账户管理系统等，特别合适采用面向服务的架构实现。系统的难点在于运营，即任务（业务）的发现与投放。以下一些场景供你思考：

* 基本假设：所有学生通过邮箱/手机登陆；学生注册的学号、姓名、年龄、性别、年级、专业等信息是真实的。学生平时使用昵称、头像在社区中活动，可以自由组成兴趣组。机构信息都是真实有效的。
* 可以考虑的任务场景：
    - 机构组织问卷调查。如学生会针对大二，女生就某个问题开展调查，共300份，符合条件学生完成调查就可得到一元闲钱。
    - 协会招新通知。如某协会正对计算机大一新生征集简历，填写提交简历可得到0.01元闲钱。
    - 取快递。如某学生出 0.5 元闲钱请同专业同年级取快递。

**项目基本要求**：系统必须支持问卷调查业务，至少一项其他业务。

### 2018 扫码点餐与结算系统

扫码点餐与结算系统是针对不同餐厅的个性化服务系统，这类系统通常采用端+云的解决方案。以扫码点餐系统为例，你不能采用为每个餐厅开发一套系统的传统方案，而是为每个餐厅提供移动app、微信小程序、网站等形式提供展示层服务，然后设计一个运营企业提供客户管理、支付管理、订餐管理等云服务，与你的客户共成长。

扫码点餐与结算系统涉及许多系统，如客户端、云服务端。除了每个餐厅都有一个个性化客户端外，它设计许多系统与服务：

* 消费者，它们使用某种客户端完成点餐与结算服务
* 餐厅服务者，它们使用服务系统完成现场服务、菜品准备等工作

**项目基本要求**：实现某餐厅扫码点餐系统的 端+云 原型。仅需要点餐到结算流程 + 一个创新业务

### 2017 互联网电影票售票系统

互联网电影票售票系统是比较常见的电子商务销售系统，常见有淘票票、格瓦拉等。它需要多个系统协作才能完成完成售票业务，涉及的利益相关人包括：

* 消费者，他们使用不同的电影票零售系统，如淘票票、格瓦拉等，它们提供电影票零售、与fans的互动社区、宣传推广等业务
* 院线，每个院线控制了若干电影院，如万达等院线则负责排片、电影票的供给

分销-院线-影院形成了一个完整的产业生态。类似的业务包括机票、酒店订房等互联网业务，它们有及其类似的业务和系统模型；

**项目基本要求**：实现一个具有售票功能的零售系统原型。仅需要实现售票业务 + 一个创新业务

**项目提高要求**：实现院线原型以及零售接口，实现院线与零售多对多的关系。例如：某电影在某影院上线，不同零售系统能竞争售票

## 3、项目要求与限制

1. 基本业务流程
    - 挣闲钱必须包括任务发放到任务完成的业务过程，基础业务是问卷调查。
    - 电影票系统必须包括从用户选择电影到完成订票业务的过程
    - 扫码点餐系统必须支持扫码、点餐到点餐完成的业务过程
2. 创新业务
    - 部分需求与设计
    - 部分实现
3. 实现技术，前端 + web 服务模式
    - 前端技术 （VUE， AngluarJS,  React 等 **JavaScript** 技术框架 ）
    - web 静态文件服务 （Nginx， 或 go 等）
    - 云端 服务实现 （Go, Java +  jesery, Python + Flask ... 等，任何语言！）  
    - 分布式部署 （docker）
4. 团队人数没有限制。
    - **建议** 5-8人为宜
5. 必须使用工具
    - UML 绘图， 如：UMLet（考试用）
    - 源代码管理，如：github
    - Markdown 文档发布工具， 如：git page
    - 带 Kanban 的团队协作工具，如 git project
6. deadline
    - 在 18 周 前提交所有内容
    - 不会延期，按代码仓库和项目文档直接给分
7. **项目评价要点**。请关注团队与个人贡献，以下要素会影响你成绩
    - 职责分工不明
    - 项目缺乏持续性。（持续时间四周以上及格，6周良好，8周优秀）
    - 个人贡献度低（用 PSP2.1 表、GITHUB 统计、Kanban 记录评估等，参见项目模板 x1-x5）
    - 团队最终贡献分配明显与 Git 记录的事实不符

## 5、往届优秀作品

**2019 作品选**

？？

**2018 作品选**

1. 【推】[2018 Tinny Hippo 小河马点餐系统](https://rookies-sysu.github.io/Dashboard/) 
    - 优秀的项目一定从 About 开始！简洁的 Demo，完美的看板安排！
2. 【推】[2018 Baoleme](https://baoleme.github.io/Dashboard/) 项目策划、需求分析、设计、测试、产品演示、每个迭代的会议、技术报告，每个工作都非常认真！餐饮客户端服务只能申请业主程序，这符合腾讯商业策略。
3. [2018研 为食喵](https://sysu-gogo.github.io/sysu-gogo-food-docs/) 
    - 罗裴然同学的总结较好展现了开发者转变观念带来的价值，其主要文档特别是API设计都是比较不错的。
4. [2018 Owl Movies](https://owl-movies-ticket-system.github.io/Dashboard/) 
    - 从 about 就看出是有组织的团队。当你在每个迭代打开仓库Insights->contributors，作为经理的就明白管理的真谛 -- 不是领导与指派，而是来自成员发自内心的自省。
5. [2018 中大零饭](https://dtosaad.github.io/documents/)
    - 居然看完了完整[视频演示](https://www.bilibili.com/video/av26106597)，包含基本功能和创新功能（协同点餐）
6. [2018 Eat点点](https://chickendinner8.github.io/) 
    - 小清新风格文档主页。 除了烤鸭之外的[鸭架汤](https://github.com/ChickenDinner8/SDP-document)也不错

**2017 作品选**

1. [MonkeyEye-FE](https://github.com/SYSUMonkeyEye/MonkeyEye-FE)
    - 做前端必看。有使用 Git 协同开发的说明，UVE 代码的组织，领域模型设计，界面与界面流的组织。 建议您阅读项目 Readme.md
2. [AwesomeTickets](https://github.com/AwesomeTickets)
    - 体现了多门课程知识在项目的应用。项目划分比较合理，设计过程清晰，文档完整。建议您阅读每个子项目 Readme.md
3. [Movie Ticket and Service Website](https://github.com/HYPJUDY/movie-ticket-and-service-website)
    - 这是一个标准的 Java Spring 多层架构 web 网站的实现方案。 
    - 项目文档清晰，有分析与设计课程所有作业的设计，它们在 documents 目录下。
4. [订你所想](https://github.com/SevenDwarfs)
    - 建议进入 dashboard 看他们的分工与技术博客

## 5、学生博客

### 5.1 Github 使用

**[Pro Git 入门必读](https://git-scm.com/book/zh/v2)**  

* 【推】 [2018 在Github上创建Organization](https://chun-ge.github.io/How-to-establish-an-organization-on-Github/)
    - 团队项目合作第一步，创建组织
* [2018 Git恢复之前版本的两种方法reset、revert（图文详解）](https://blog.csdn.net/yxlshk/article/details/79944535)
    - 必须的技巧

### 5.2 项目组织与管理工具与经验

**彼得·德鲁克，[《卓有成效的管理者》](https://book.douban.com/subject/1322025/)**  
**[硝烟中的Scrum和XP](https://www.infoq.cn/article/scrum-xp-from-the-trenches)**  


* 【推】 [2018 初为产品经理的心理障碍](https://blog.csdn.net/qq_33559972/article/details/79934411)
    - 强！把想法转化为产品设计的确有这个过程。技术和经验都重要
* [2018 团队协作工具之我见](https://summer06.github.io/2018/06/22/team_work_tool/)

### 5.3 原型设计与构建

* 【推】 [2017 Spring Boot Web Application](https://hypjudy.github.io/2017/05/30/spring-boot-web-application/)
    - 采用 Java  Spring MVC -  Thymeleaf 构建项目原型
* [2018 交互设计那些小纠结](https://blog.csdn.net/qq_33559972/article/details/80877316)
    - 写得好也重要

### 5.4 需求分析实战案例分享

* [2018 需求分析的思路转变](https://blog.csdn.net/qq_34112279/article/details/80954526)
    - 当你努力去做对别人（stakeholder）有价值的事情，就是好的开始

### 5.5 架构设计与模式

* 【推】 [2018 详解REST架构风格](https://segmentfault.com/a/1190000014768057)
    - 严谨的写作风格，干货的内容。获得 segmentfault 推荐的文章

### 5.6 表现层设计技术（VUE等 js 技术）

* [2018 Vue 跨域问题和前后端分离](https://www.jianshu.com/p/712a327e4d84)

### 5.7 服务层设计技术（Web，REST，gRPC 等技术）

[2018 Go语言：Web开发中的数据储存](https://blog.csdn.net/zzmian/article/details/78759804)
    - 介绍 go 语言处理 Cookie 与 session

### 5.8 DevOps 技术（CI/CD工具链，docker技术）

* 【推】 [2018 使用Travis CI和Codecov进行持续集成和代码覆盖率统计](https://pak-choi.github.io/%E7%B3%BB%E7%BB%9F%E5%88%86%E6%9E%90%E4%B8%8E%E8%AE%BE%E8%AE%A1/2018/04/15/SAAD-Report/)
    - 使用 Travis 测试必读， Paased 小图标代表高大上
* [2018 travis与docker hub集成](https://txzdream.github.io/2018/06/07/travis-docker-hub/)
    - go 使用 travis

* [2018 Docker 入门实战](https://ace-0.github.io/2018/04/13/docker-learning/)

* [2018 在 Ubuntu 16.04 LTS 上使用 docker-compose 实现 Nginx+Flask+MySQL+Redis 的 web 后台应用部署](https://www.zybuluo.com/longj/note/1173047)
    - 一键部署
* [2018 Docker 加速部署](https://www.zybuluo.com/longj/note/1189134)
* [2018 github+travis实现自动部署 && 前端跨域问题解决之Nginx配置篇](https://blog.csdn.net/liaozelin_/article/details/80906078)


### 5.9 接口设计方法与工具（Swagger 等）

### 5.x 其他

* [2018 Jmeter测试详记](https://humanlee1011.github.io/2018/07/07/Jmeter%E6%B5%8B%E8%AF%95%E8%AF%A6%E8%AE%B0/)

