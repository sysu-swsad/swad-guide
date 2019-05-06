---
layout: default
title: Inception 实践指南
---

# Inception 实践指南
{:.no_toc}

* 目录
{:toc}


## 1、团建工作

团建工作通常包括两个部分：团建组建与职责分配， 沟通渠道建设。

**团建组建与职责分配**

制品（artifact）是 **team profile**，它通常包括：

* 团队名称（中/英文简称）
* 团队目标： 项目愿景（一句话）
* 团队成员清单（学号，昵称，github账号连接，角色）。其中，角色是多选项，一般一个人选择 2-3 个角色为宜。角色分为三大类
    - 面向客户类
        - 具体角色：**项目经理**、 **客户经理**、 **产品经理**
        - 技能要求：与客户沟通的能力，获取需求能力，产品策划能力
        - 项目经理特别要求： 了解 Scrum 的基本运作过程，建议阅读：[硝烟中的Scrum和XP](http://www.infoq.com/cn/minibooks/scrum-xp-from-the-trenches)
    - 技术开发类
        - 具体角色： 架构师（技术经理）、开发工程师（也可以具体一些，如 java工程师 ，js工程师 ， UI/UX设计师等）
        - 技能要求： 专注某一类技术的实现的开发工程师，例如，项目计划引入智能语音交互技术，可以设定一个 AI工程师
        - UI/UX设计师特别要求： 具体艺术偏好，对用户体验有执念。建议阅读：[2018年的UI / UX设计趋势](http://www.uisdc.com/ui-ux-design-trend-2018)
        - 架构师特别要求： 技术比较全面，用一个词“全栈工程师”
    - 质量保证类
        - 具体角色： **QA 工程师**、 **DevOps 工程师**
        - QA 工程师要求： 理解项目各阶段测试需求，带领团队规划测试用例，确保测试需求（如代码覆盖）的指标得以实现
            - 具体技能：各种开发标准与规范的制定；单元测试、集成测试、功能测试、性能测试等方案的设计与相关工具的使用
        - DevOps 工程师要求：通过开发，支持开发环境、生产环境高效、自动化地运作
            - 具体技能：Github, Docker, Linux 命令行程序与 shell， python， 数据库等各类系统的部署
* 具体分工与个人宣言（每人一行）

案例：[示例](https://github.com/HYPJUDY/movie-ticket-and-service-website/blob/master/documents/2_team_profile.md)

**沟通渠道建设**

* 即时通讯群，如 QQ群
* 相关管理工具（KanBan），如 github project，TADP

## 2、产品调查报告

通过互联网收集现有竞争性产品信息，主要包括：

* 相关产品与发展综述
* 值得关注的竞争产品（3~5个），及其竞争优势
* 相关产品的市场（客户）定位
* 某个产品的典型业务实现的过程，核心界面
* 可能存在的新机遇（例如，AI技术发展，给改进这类产品来带了新机会，所以我们打算...）

案例：。。。

## 3、Inception 会议和会议纪要

**项目启动会议**

议题，例如：“XX云餐饮服务平台”，约一个小时

* 会议目标：定义产品范围、愿景和核心业务
* 任务1：介绍产品调查结果
* 任务2：产品讨论
    - 工具：“思维导图”，建议每个人都用它记录讨论要点
        - 组织、发现会议的逻辑
        - 控制会议的内容，在内容发散与聚焦之间找平衡
        - 重点标识符勾出你认为（贡献人含自己）最有价值的要点与冲突。（肯定别人提议，凝练议题要点，群面必杀之技）
    - 确定产品名称
    - 候选业务范围：
        - 基本业务，及其可能的创新点
        - 创新业务（至少一个）
        - 辅助业务
    - 创新点凝练
        - 围绕产品愿景的检查表（课程PPT），研讨产品的亮点与特色
        - 至少一个业务的亮点
        - 从业务流程再造、新业务、UX改进、新技术应用等角度思考技术亮点
    - 本步骤的目标，方便编写 vision 文档
* 任务3：定义产品
    - 按用户，利益、业务故事名称定义产品的服务范围（6~8个业务）
    - 本步骤的目标，方便编写第一版本 backlog 文档。 具体参考 _硝烟中的Scrum和XP_
* 任务4：分析涉及的相关技术与潜在风险
* 任务5：项目经理总结陈词（分派任务）

思维导图，[示例](https://github.com/HYPJUDY/movie-ticket-and-service-website/blob/master/documents/91_meet_recording.md)

## 4、项目的规划

建立一个 About.md 文档规划整个项目。

规划分为一个 Inception 和 若干迭代构成，每个迭代按 UP 工作流组织。建议一个迭代 3 周。每个迭代有目标和每周任务构成。

推荐文档内容结构：

* About Project
* Core Artifacts
* Iterations
    - Inception
    - Iteration n
        - goals
        - weeks n （github project kanban 的连接） 

注：项目规划每周更新一次

案例，[示例](https://github.com/AwesomeTickets/Dashboard)


## 5、项目文档提交！

### 5.1 Github 的组织
    
* 创建一个组织， 如 AwesomeTickets
* 每个成员加入项目组织
* 创建一个 documents 或 teamworks 或 dashboard 存储区域
* 创建一个 gh-pages 分支，选择合适的模板，作为团队作业发布区
* 创建第一个文件 index.md 作为作业的索引文件


### 5.2 团队作业清单

* 1、About（项目规划）
* 2、Team profile（团队组建）
* 3、Investigation（项目前期调研）
* 4、Vision（项目愿景）
* X1 meet_recording
    - inception meeting (yy/mm/dd)

注：sprint backlog 与 sprint plan 见项目规划要求  
注：meeting_recording 要求一周一次或一个迭代一次


  



