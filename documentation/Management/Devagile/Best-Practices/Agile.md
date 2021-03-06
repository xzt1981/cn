# 敏捷实践
## 敏捷研发概念
敏捷研发是一种能应对快速变化需求的软件开发能力，涉及整个软件工程的理念与实践，它的核心是 迭代和增量式软件开发方法。开发者快速发布几个可运行但不完美的版本投入市场，在后续迭代中根据用户的反馈改进产品，新增一到多个用户可以感知的完整功能，从而逼近产品的最终形态。迭代就是整个理论的核心，敏捷研发大大完善了迭代开发的理论，使之能够被广大的软件开发团队认可，并开发了具体的实践方法如： Scrum 等。

敏捷研发比较特别的地方是它是 组织文化，流程以及工具的结合体，在敏捷研发介绍中要着重强调三者的同样重要而且缺一不可：“工具，流程，组织文化”。缺少工具支持的敏捷研发无法实现“高速”；缺少组织文化支持的敏捷研发会让团队成员之间无法团结一致完成共同的目标。

![敏捷](/image/DevAgile/image-agile/1.jpg)
## 运用DevAgile进行敏捷研发
DevAgile项目管理工具结合敏捷迭代的管理概念，帮助用户对项目进行迭代管理，打通需求、任务、缺陷等其他自定义工作项的沟通流转诉求，使项目管理过程进度安全可控。DevAgile项目管理默认由4个核心模块构成：需求管理、迭代管理、任务管理和缺陷管理。以下实践我们以Scrum模型来具体说明。
### 新建项目
敏捷开发第一步是确认敏捷项目团队的项目目标和人员构成，并选择对此次项目流程把控和项目内容最为熟练的人成为Scrum负责人，由他来创建项目。

项目创建路径：工作台主页--创建新项目

![项目](/image/DevAgile/image-agile/2.png)
### 定义需求（缺陷，任务）交付流程
创建项目后确定项目目标，时间，人员后需要讨论需求交付流程，进行工作项管理配置。

比较简单的流程如下：

![流程](/image/DevAgile/image-agile/流程.png)

需求状态划分的原则，从一个状态到另一个状态：
* 有交付产出物产生。
* 负责人员有变动。

例如：
* 从待评估到已评估，需要有PRD文档，或者该需求有详细的规则描述，能够达到研发同学用来做软件设计的程度。从待评估到已评估，研发团队,测试人员与产品经理要达成需求澄清的共识。
* 从开发中到待验证，关注的人员从研发人员转移到测试人员，验证通过后到待发布阶段，关注人员由测试人员转移到研发人员，研发人员提交上线单发布完成后改为已发布状态。

注意：上面的流程是由整个敏捷团队一起讨论决定的，比如，开发中后面是否要加联调中，待验证是否要改成提测（结合日常大家理解的命名规则），后面是否要加上交互验证（控制台产品）负责交互设计的同学有些是想做下交互设计的把关的等等。总之是整个敏捷团队讨论决定需求交付流程。

敏捷研发中追求的是快速交付有用的用户价值，及时获得用户反馈以便改进，需求的交付流程是体现的是用户价值的交付，所以项目关注的核心是需求的交付。缺陷和任务是对需求的细分和补充。
#### 云翼工程效率项目需求交付流程与定义
需求：可以交付的产品功能，是敏捷团队协作交付的用户价值，一个需求需要通过多次上线发布来实现可以拆分为子需求进行跟踪。需求内对个人工作内容的划分可以拆分为子任务。

按照上面的流程运行，各阶段定义如下：

![需求](/image/DevAgile/image-agile/需求阶段.png)

任务：具体分配给个人的工作内容

![任务](/image/DevAgile/image-agile/任务阶段.png)

### 邀请Scrum成员
Scrum三个角色：产品负责人、开发团队、Scrum Master（即项目负责人） 

Scrum团队是自组织、跨职能的完整团队。三种角色的组成可以使该团队拥有工作所需要的全部技能，不需依赖外部人员。且自组织的工作方式最大限度优化团队适应性、创造性和生产力。

项目成员邀请路径：项目主页--项目设置--成员管理--添加项目成员--ERP搜索成员/按部门搜索成员--批量勾选添加成员--为成员赋予角色

![成员](/image/DevAgile/image-agile/3.png)
### 需求管理
在Scrum中，产品负责人需要通过调研客户市场需求，按照商业/用户价值形成不同优先级的需求列表，列表条目的体现形式通常为用户故事，Scrum团队需要先开发对客户具有较高价值的需求。

因此产品负责人需要将项目的产品规划以需求形式记录更新，对于优先级较高且紧急的需求，应当提供相对完善的信息记录和需求文档，同时把相应的需求分配给负责人（通常需求负责人为产品负责人）。

需求管理路径：项目主页--需求管理--使用默认配置--添加需求--按照用户故事编写需求/上传附件--明确需求优先级--确定需求处理人--确定需求截止时间--拆分任务（迭代计划会议后）

![需求](/image/DevAgile/image-agile/4.png)
### 需求任务拆分
迭代规划会议之前，产品负责人将产品需求记录详尽，标明优先级（前一步骤），尽量细化需求，把需求拆成可被执行的任务，并对工作进行工时预估。为了给迭代计划会议提供材料，需要将拆分任务进行记录。

任务管理路径：项目主页--需求管理--创建子任务--指派人

### 迭代计划会议
在明确项目需求后，需要Scrum负责人组织迭代计划会议，Scrum负责人提前通过邮件等方式同步会议整体信息。对于后面的工作来说，迭代计划会议对于敏捷研发来说非常重要，是所有任务按期完成的基础。

通过任务工作量、工时预估，以及需求的优先级，可以确定本次迭代的工作量。如果工作量高于项目团队产能，则需要将一些需求放到下个迭代；如果低于项目团队产能，则可以将后续需求前置。
### 第一个迭代
迭代计划会议完成后，迭代目标确认，所有迭代需求项以及任务已经清晰定义，Scrum负责人要把会上一致通过的需求和任务规划进迭代中，并设定好截止时间、在迭代管理界面，负责人可以实时看到整个迭代的完成进度信息。

![迭代](/image/DevAgile/image-agile/5.png)

![迭代1](/image/DevAgile/image-agile/6.png)
然后可以开始第一个迭代周期，迭代开始后，各需求处理人要实时更新工作项的状态，迭代看板可以用于跟进进度，可以通过工作项所在状态的情况，及时发现需求的阻塞点。

![迭代2](/image/DevAgile/image-agile/7.png)
### 每日站会
作为敏捷开发项目，团队需要在迭代开始后，每天通过站会形式来讨论解决执行过程中的问题。站会要精简，控制在半小时以内，项目成员主要描述已完成事项、今日待办以及遇到的问题。有问题出现时，可记录在缺陷管理中，相关人员可协力解决。

在会议上，每一个开发团队 成员都需要说明:
* 昨天，我为帮助开发团队达成迭代目标做了什么?
* 今天，我为帮助开发团队达成迭代目标准备做什么?
* 是否有任何障碍在阻碍我或开发团队达成迭代目标?

### 缺陷记录
每日站会发现的缺陷，对紧急程度高的缺陷需要第一时间反馈到产品进行修复，结合人员产能，归在本次迭代中。优先级不高的会安排到接下来迭代修复。

缺陷管理路径：项目主页--缺陷管理–添加缺陷--分配处理人；项目主页--迭代管理--迭代详情--添加缺陷--分配处理人
### 迭代评审会议
迭代结束之前，需要相应的负责人对项目成果进行评估，用以检视所交付的产品增量并按需调整产品待办列表，保证确保事务完成情况和计算最初设想目标的达成率。

Scrum负责人验证迭代中的所有事项是否已是完成态，即迭代的进度是否为100%，如为100%，则标志着迭代产品任务已经完成。如非100%，则由产品负责人说明遗留的任务列表，并确认可能完成时间，如本期无法完成，需要调整本期交付的产品列表。

迭代评审结果，可能会根据实际工时等情况，将部分未完成的任务规划到新迭代中，在下一个迭代进行跟进。

迭代进度计算方式：当前迭代下需求/任务/缺陷已完成状态数占比全部工作项的比率

![评审](/image/DevAgile/image-agile/8.png)

![图表](/image/DevAgile/image-fuction/迭代图表.png)

### 完成第一个迭代
当迭代已经到预设的结束时间时，意味着本周期的迭代已经结束，即便是迭代中的事项暂未完成。为了保证项目的交付成果质量，未完成的迭代工作项需要规划到下一个迭代。
### 迭代回顾
最后整个团队还需要进行一次回顾会议，回顾这次迭代有哪些做的好，哪些做的不好，并列出下次的可执行任务，规划进下一个迭代，便于改进整个团队的研发效能。

在测试环节和正式上线之后，发现的问题，都可以在DevAgile缺陷管理模块中统一记录管理，并排出优先级作为下一个迭代中的工作来源之一。

DevAgile项目图表对也提供了对缺陷的统计功能，对缺陷状态占比进行统计，方便测试工程师了解项目的整体情况

![回顾](/image/DevAgile/image-agile/9.png)
### 开启新的迭代
敏捷研发重点在于高质量的用户团队反馈数据，有效缩小试错范围，合理安排工期，简化开发过程，并在项目范围内同步保证目标的一致性。

但对于不同的团队，工作现状及项目类型不同，仍需要项目负责人结合团队特点来实现敏捷迭代，提高产品交付效率。

除此之外，很多不确定性因素会导致计划失效，比如项目成员增减、技术应用效果、用户需求的改变、竞争者对我们的影响等都会让我们作出不同的反应。敏捷不是基于预定义的工作方式，而是基于经验性的方式，对以上这些变化，项目团队需要通过不断的反省调整来保持团队的敏捷性。
