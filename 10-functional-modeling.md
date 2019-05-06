# 功能建模

## 1. 功能建模 - 系统顺序图与操作契约

**1.1 什么是功能建模？**

给出系统面向外部实体（用户及外部系统）要实现的 **业务操作** 功能的定义

**1.2 为什么要进行功能建模**

1. 识别所有系统要提供的业务操作，给出严格的定义
2. 通过识别这些操作，精确的估算工作量
3. 完善系统实现的细节（消息、参数）等，构建RPC风格设计，或进一步完善领域模型与资源API设计

建模方法与工具：

* 系统顺序图（System Sequence Diagram）
* 操作协议（Operation contracts）
* 基于功能点的项目工作量估计（Function Points）

**1.3 系统时序图案例**

微信OAuth2.0授权登录:

![微信OAuth2.0](https://res.wx.qq.com/op_res/ZLIc-BdWcu_ixroOT0sBEtk0UwpTewqS6ujxbC2QOpbKIVp_DzleM_C9I-9GPDDh)

微信小程序开放接口（login）工作原理：

![api-login.html](https://mp.weixin.qq.com/debug/wxadoc/dev/image/api-login.jpg?t=2018428)

**注意，我们不能获得用户微信号等敏感信息，只是微信 api 为你 appId 生成的 OpenID。 [详细说明](https://developers.weixin.qq.com/miniprogram/dev/api/open.html#wxgetuserinfoobject)

这个图描述了系统之间协作的过程

**1.4 功能点（FP）**

[Introduction to Function Points](http://www.ifpug.org/Conference%20Proceedings/IFPUG-2004/IFPUG2004-04-Aguiar-introduction-to-function-point-analysis.pdf) - IFPUG

**1.5 RPC风格 API 设计工具**

* Apache thrift
    - 官网：http://thrift.apache.org/
    - RPC 基础知识：[Apache Thrift - 可伸缩的跨语言服务开发框架](https://www.ibm.com/developerworks/cn/java/j-lo-apachethrift/)
    - 支持多种语言
* jsonRPC
    - 标准：https://www.jsonrpc.org/specification
    - 任何支持 [json](http://json.org/) 的语言都可以简单实现 jsonRPC
    - 一元（Unary）函数 RPC
* Google gRPC
    - 官网：https://grpc.io/
    - proto buffer 序列化与反序列化
    - HTTP2 加持。支持双向流和多种认证
    - 支持多种语言

## 2、需求分析全过程

![](images/analysis_all_in_one.png)

## 3、团队作业

* 1、About（项目规划）
* 2、Team profile（团队组建）
* 3、Investigation（项目前期调研）
* 4、Vision（项目愿景）
* 5、Product Backlog （产品特性）
* 6、Requirement specification（需求规格说明）
    - 6.1 Usecase Diagram（用例图）
    - 6.2 Use Cases（用例+活动图）
    - 6.3 Domian Model（领域模型）
    - 6.4 State Model（状态模型）
    - **6.5 System Sequence Diagram（功能模型）**
* 7、Design（设计）
    - 7.1 UI design
        - XX 用例 UI设计
    - 7.2 Database design
        - 7.2.1 用户及权限系统数据库设计
        - 7.2.2 XX子系统数据课设计 
        - 7.2.x 第三方数据评审结果
    - **7.3 API 设计**
* 8、生产规范与指南
    - 8.1 XX 代码规范
    - 8.2 REST API 设计规范
* X1 meet_recording
    - inception meeting (yy/mm/dd)
    - **Iteration X meeting (yy/mm/dd)**
* X2 Tech/Work Report
    - 学号-title

团队作业要求：
1. 6.5 系统顺序图
    - 每个成员至少编写一个应用场景的系统顺序图（左用户，中间是系统，右边是外部实体对象）
    - 至少一个操作需要写后置条件，用注释符号表示写在操作的后面
    - 请使用自己 git 账号体完成该任务（同时在文字中标明自己的学号）
2. 7.3 给出部分正式的 API 说明书
    - 建议参考 [微信开发平台](https://open.weixin.qq.com/cgi-bin/showdocument?action=dir_list&t=resource/res_list&verify=1&id=open1419317851&token=&lang=zh_CN) 或 [微信支付API](https://pay.weixin.qq.com/wiki/doc/api/app/app.php?chapter=9_1)
    - 部分应用场景的核心 API 必须给出代码实例
    - 部分复杂应用场景的核心 API，给出系统顺序图 












