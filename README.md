

### 系统功能

|     | 功能    | 描述                              |
|-----|-------|---------------------------------|
|     | 用户管理  | 用户是系统操作者，该功能主要完成系统用户配置          |
| ⭐️  | 在线用户  | 当前系统中活跃用户状态监控，支持手动踢下线           |
|     | 角色管理  | 角色菜单权限分配、设置角色按机构进行数据范围权限划分      |
|     | 菜单管理  | 配置系统菜单、操作权限、按钮权限标识等，本地缓存提供性能    |
|     | 部门管理  | 配置系统组织机构（公司、部门、小组），树结构展现支持数据权限  |
|     | 岗位管理  | 配置系统用户所属担任职务                    |
| 🚀  | 租户管理  | 配置系统租户，支持 SaaS 场景下的多租户功能        |
| 🚀  | 租户套餐  | 配置租户套餐，自定每个租户的菜单、操作、按钮的权限       |
|     | 字典管理  | 对系统中经常使用的一些较为固定的数据进行维护          |
| 🚀  | 短信管理  | 短信渠道、短息模板、短信日志，对接阿里云、腾讯云等主流短信平台 |
| 🚀  | 邮件管理  | 邮箱账号、邮件模版、邮件发送日志，支持所有邮件平台       |
| 🚀  | 站内信   | 系统内的消息通知，提供站内信模版、站内信消息          |
| 🚀  | 操作日志  | 系统正常操作日志记录和查询，集成 Swagger 生成日志内容 |
| ⭐️  | 登录日志  | 系统登录日志记录查询，包含登录异常               |
| 🚀  | 错误码管理 | 系统所有错误码的管理，可在线修改错误提示，无需重启服务     |
|     | 通知公告  | 系统通知公告信息发布维护                    |
| 🚀  | 敏感词   | 配置系统敏感词，支持标签分组                  |
| 🚀  | 应用管理  | 管理 SSO 单点登录的应用，支持多种 OAuth2 授权方式 |
| 🚀  | 地区管理  | 展示省份、城市、区镇等城市信息，支持 IP 对应城市      |

![功能图](/.image/common/system-feature.png)

### 工作流程

|     | 功能    | 描述                                     |
|-----|-------|----------------------------------------|
| 🚀  | 流程模型  | 配置工作流的流程模型，支持文件导入与在线设计流程图，提供 7 种任务分配规则 |
| 🚀  | 流程表单  | 拖动表单元素生成相应的工作流表单，覆盖 Element UI 所有的表单组件 |
| 🚀  | 用户分组  | 自定义用户分组，可用于工作流的审批分组                    |
| 🚀  | 我的流程  | 查看我发起的工作流程，支持新建、取消流程等操作，高亮流程图、审批时间线    |
| 🚀  | 待办任务  | 查看自己【未】审批的工作任务，支持通过、不通过、转发、委派、退回等操作    |
| 🚀  | 已办任务  | 查看自己【已】审批的工作任务，未来会支持回退操作               |
| 🚀  | OA 请假 | 作为业务自定义接入工作流的使用示例，只需创建请求对应的工作流程，即可进行审批 |

![功能图](/.image/common/bpm-feature.png)

### 支付系统

|     | 功能   | 描述                        |
|-----|------|---------------------------|
| 🚀  | 应用信息 | 配置商户的应用信息，对接支付宝、微信等多个支付渠道 |
| 🚀  | 支付订单 | 查看用户发起的支付宝、微信等的【支付】订单     |
| 🚀  | 退款订单 | 查看用户发起的支付宝、微信等的【退款】订单     |
| 🚀  | 回调通知 | 查看支付回调业务的【支付】【退款】的通知结果    |
| 🚀  | 接入示例 | 提供接入支付系统的【支付】【退款】的功能实战    |

### 基础设施

|     | 功能        | 描述                                           |
|-----|-----------|----------------------------------------------|
| 🚀  | 代码生成      | 前后端代码的生成（Java、Vue、SQL、单元测试），支持 CRUD 下载       |
| 🚀  | 系统接口      | 基于 Swagger 自动生成相关的 RESTful API 接口文档          |
| 🚀  | 数据库文档     | 基于 Screw 自动生成数据库文档，支持导出 Word、HTML、MD 格式      |
|     | 表单构建      | 拖动表单元素生成相应的 HTML 代码，支持导出 JSON、Vue 文件         |
| 🚀  | 配置管理      | 对系统动态配置常用参数，支持 SpringBoot 加载                 |
| ⭐️  | 定时任务      | 在线（添加、修改、删除)任务调度包含执行结果日志                     |
| 🚀  | 文件服务      | 支持将文件存储到 S3（MinIO、阿里云、腾讯云、七牛云）、本地、FTP、数据库等   | 
| 🚀  | WebSocket | 提供 WebSocket 接入示例，支持一对一、一对多发送方式              | 
| 🚀  | API 日志    | 包括 RESTful API 访问日志、异常日志两部分，方便排查 API 相关的问题   |
|     | MySQL 监控  | 监视当前系统数据库连接池状态，可进行分析SQL找出系统性能瓶颈              |
|     | Redis 监控  | 监控 Redis 数据库的使用情况，使用的 Redis Key 管理           |
| 🚀  | 消息队列      | 基于 Redis 实现消息队列，Stream 提供集群消费，Pub/Sub 提供广播消费 |
| 🚀  | Java 监控   | 基于 Spring Boot Admin 实现 Java 应用的监控           |
| 🚀  | 链路追踪      | 接入 SkyWalking 组件，实现链路追踪                      |
| 🚀  | 日志中心      | 接入 SkyWalking 组件，实现日志中心                      |
| 🚀  | 服务保障      | 基于 Redis 实现分布式锁、幂等、限流功能，满足高并发场景              |
| 🚀  | 日志服务      | 轻量级日志中心，查看远程服务器的日志                           |
| 🚀  | 单元测试      | 基于 JUnit + Mockito 实现单元测试，保证功能的正确性、代码的质量等    |

![功能图](/.image/common/infra-feature.png)

### 数据报表

|     | 功能    | 描述                 |
|-----|-------|--------------------|
| 🚀  | 报表设计器 | 支持数据报表、图形报表、打印设计等  |
| 🚀  | 大屏设计器 | 拖拽生成数据大屏，内置几十种图表组件 |

### 微信公众号

|     | 功能     | 描述                            |
|-----|--------|-------------------------------|
| 🚀  | 账号管理   | 配置接入的微信公众号，可支持多个公众号           |
| 🚀  | 数据统计   | 统计公众号的用户增减、累计用户、消息概况、接口分析等数据  |
| 🚀  | 粉丝管理   | 查看已关注、取关的粉丝列表，可对粉丝进行同步、打标签等操作 |
| 🚀  | 消息管理   | 查看粉丝发送的消息列表，可主动回复粉丝消息         |
| 🚀  | 自动回复   | 自动回复粉丝发送的消息，支持关注回复、消息回复、关键字回复 |
| 🚀  | 标签管理   | 对公众号的标签进行创建、查询、修改、删除等操作       |
| 🚀  | 菜单管理   | 自定义公众号的菜单，也可以从公众号同步菜单         |
| 🚀  | 素材管理   | 管理公众号的图片、语音、视频等素材，支持在线播放语音、视频 |
| 🚀  | 图文草稿箱  | 新增常用的图文素材到草稿箱，可发布到公众号         |
| 🚀  | 图文发表记录 | 查看已发布成功的图文素材，支持删除操作           |

### 商城系统

![功能图](/.image/common/mall-feature.png)

![功能图](/.image/common/mall-preview.png)

演示地址：<https://doc.iocoder.cn/mall-preview/>

### 会员中心

|     | 功能   | 描述                               |
|-----|------|----------------------------------|
| 🚀  | 会员管理 | 会员是 C 端的消费者，该功能用于会员的搜索与管理        |
| 🚀  | 会员标签 | 对会员的标签进行创建、查询、修改、删除等操作           |
| 🚀  | 会员等级 | 对会员的等级、成长值进行管理，可用于订单折扣等会员权益      |
| 🚀  | 会员分组 | 对会员进行分组，用于用户画像、内容推送等运营手段         |
| 🚀  | 积分签到 | 回馈给签到、消费等行为的积分，会员可订单抵现、积分兑换等途径消耗 |

### ERP 系统

![功能图](/.image/common/erp-feature.png)

演示地址：<https://doc.iocoder.cn/erp-preview/>

### CRM 系统

![功能图](/.image/common/crm-feature.png)

演示地址：<https://doc.iocoder.cn/crm-preview/>

## 🐨 技术栈

### 模块

| 项目                    | 说明                 |
|-----------------------|--------------------|
| `yudao-dependencies`  | Maven 依赖版本管理       |
| `yudao-framework`     | Java 框架拓展          |
| `yudao-server`        | 管理后台 + 用户 APP 的服务端 |
| `yudao-module-system` | 系统功能的 Module 模块    |
| `yudao-module-member` | 会员中心的 Module 模块    |
| `yudao-module-infra`  | 基础设施的 Module 模块    |
| `yudao-module-bpm`    | 工作流程的 Module 模块    |
| `yudao-module-pay`    | 支付系统的 Module 模块    |
| `yudao-module-mall`   | 商城系统的 Module 模块    |
| `yudao-module-erp`    | ERP 系统的 Module 模块  |
| `yudao-module-crm`    | CRM 系统的 Module 模块  |
| `yudao-module-mp`     | 微信公众号的 Module 模块   |
| `yudao-module-report` | 大屏报表 Module 模块     |

### 框架

| 框架                                                                                          | 说明               | 版本             | 学习指南                                                           |
|---------------------------------------------------------------------------------------------|------------------|----------------|----------------------------------------------------------------|
| [Spring Boot](https://spring.io/projects/spring-boot)                                       | 应用开发框架           | 3.2.0          | [文档](https://github.com/YunaiV/SpringBoot-Labs)                |
| [MySQL](https://www.mysql.com/cn/)                                                          | 数据库服务器           | 5.7 / 8.0+     |                                                                |
| [Druid](https://github.com/alibaba/druid)                                                   | JDBC 连接池、监控组件    | 1.2.20         | [文档](http://www.iocoder.cn/Spring-Boot/datasource-pool/?yudao) |
| [MyBatis Plus](https://mp.baomidou.com/)                                                    | MyBatis 增强工具包    | 3.5.4.1        | [文档](http://www.iocoder.cn/Spring-Boot/MyBatis/?yudao)         |
| [Dynamic Datasource](https://dynamic-datasource.com/)                                       | 动态数据源            | 4.2.0          | [文档](http://www.iocoder.cn/Spring-Boot/datasource-pool/?yudao) |
| [Redis](https://redis.io/)                                                                  | key-value 数据库    | 5.0 / 6.0 /7.0 |                                                                |
| [Redisson](https://github.com/redisson/redisson)                                            | Redis 客户端        | 3.25.0         | [文档](http://www.iocoder.cn/Spring-Boot/Redis/?yudao)           |
| [Spring MVC](https://github.com/spring-projects/spring-framework/tree/master/spring-webmvc) | MVC 框架           | 6.1.1          | [文档](http://www.iocoder.cn/SpringMVC/MVC/?yudao)               |
| [Spring Security](https://github.com/spring-projects/spring-security)                       | Spring 安全框架      | 6.2.0          | [文档](http://www.iocoder.cn/Spring-Boot/Spring-Security/?yudao) |
| [Hibernate Validator](https://github.com/hibernate/hibernate-validator)                     | 参数校验组件           | 8.0.1          | [文档](http://www.iocoder.cn/Spring-Boot/Validation/?yudao)      |
| [Flowable](https://github.com/flowable/flowable-engine)                                     | 工作流引擎            | 7.0.0          | [文档](https://doc.iocoder.cn/bpm/)                              |
| [Quartz](https://github.com/quartz-scheduler)                                               | 任务调度组件           | 2.3.2          | [文档](http://www.iocoder.cn/Spring-Boot/Job/?yudao)             |
| [Springdoc](https://springdoc.org/)                                                         | Swagger 文档       | 2.2.0          | [文档](http://www.iocoder.cn/Spring-Boot/Swagger/?yudao)         |
| [SkyWalking](https://skywalking.apache.org/)                                                | 分布式应用追踪系统        | 9.0.0          | [文档](http://www.iocoder.cn/Spring-Boot/SkyWalking/?yudao)      |
| [Spring Boot Admin](https://github.com/codecentric/spring-boot-admin)                       | Spring Boot 监控平台 | 3.1.8          | [文档](http://www.iocoder.cn/Spring-Boot/Admin/?yudao)           |
| [Jackson](https://github.com/FasterXML/jackson)                                             | JSON 工具库         | 2.15.3         |                                                                |
| [MapStruct](https://mapstruct.org/)                                                         | Java Bean 转换     | 1.5.5.Final    | [文档](http://www.iocoder.cn/Spring-Boot/MapStruct/?yudao)       |
| [Lombok](https://projectlombok.org/)                                                        | 消除冗长的 Java 代码    | 1.18.30        | [文档](http://www.iocoder.cn/Spring-Boot/Lombok/?yudao)          |
| [JUnit](https://junit.org/junit5/)                                                          | Java 单元测试框架      | 5.10.1         | -                                                              |
| [Mockito](https://github.com/mockito/mockito)                                               | Java Mock 框架     | 5.7.0          | -                                                              |
