---
layout: post
title:  开放银行（一）
categories: 开放银行
---



> 开放银行(Open Banking) 是银行4.0阶段的起点,也是银行完整性的起点

* toc
{:toc}

##  银行发展至今经历的4个阶段

- **银行1.0** ， 网点服务阶段 （固定时间、固定地点）

- **银行2.0** ， 自助银行阶段  （ATM机 、Pos机 、电话银行）

- **银行3.0** ， 基于互联网的银行服务阶段 （网上银行、手机银行、互联网银行）
  - 互联网银行
  
    - 世界上第一家互联网银行——美国第一安全网络银行（Security First Network Bank，SFNB）
    - 中国：2015年6月 微众银行、网商银行等
    - 优势：一是KYC（了解你的客户），即在线完成开户，网点不是银行经营的必要，二是银行服务可以进一步覆盖过去没有覆盖到的人群，三是大数据的应用是贷款流程更加快速，并且坏账率明显降低。
  
  - 虚拟银行
  	- 中国香港：2019年3月，Livi VB Limited、SC Digital Solutions Limited、众安在线虚拟金融公司和WeLab Digital Limited
  
> 中国香港金融管理局对于虚拟银行的定位是：
>
> - 第一，提供新型的客户体验，找到新的突破点抢占传统银行的固有零售市场，例如利用大数据风险计量和快速审批的借贷
> - 第二，成为助力其他金融业务发展的工具，例如作为在线支付和在线理财背后的融资结算平台
> - 第三，促进普惠金融



- **银行4.0** ， 银行即服务阶段 （开放银行）
  - 个人数据和隐私保护意识；数字化革命
  - 谁能更快地深入消费者的各个场景，谁就能够成为消费者的首选

## 开放银行 （Open Banking ）

> 银行业当下面临的最大的挑战不是来自同业而是其他竞争者,尤其是金融科技公司的发展对银行构成巨大威胁。

**开放银行**,正是要求银行以开放的心态，在技术上通过API（Application Programming Interface,应用程序接口），构建一个共赢的生态圈，在这个生态圈内，银行不必拘泥于网点的服务方式，而是以一种更隐蔽的姿态，实现银行服务的输出共享。

- 银行即服务 Bank-as-a-Service,BaaS 或 银行即平台 Bank-as-a-Platform,简称BaaP

- 《银行4.0》：“未来银行的发展思维也可以融入‘第一性’原理（Elon Musk提出）。要开展真正的革命性工作，需解除思想上的桎梏，放弃’类别思维‘。“

- 银行服务的基本功能：（银行只需要有这些服务即可，并没有规定提供服务的地点、时间和方式。）

  1. 能够安全地存储货币 
  2. 能够安全地转移所有的货币
  3. 能够获得必要的信用额度

### 开放银行的定义
**欧洲银行管理局**(European Banking Authority，EBA)认为，开放银行是“连接两个世界”的一场运动，使客户在其它服务的场景下享受银行服务成为可能，通过彼此的基础设施将银行和非银机构的创新功能连接起来。

**波士顿咨询公司**(Boston Consulting Group，BCG)认为，开放银行是为顺应银行平台与第三方平台的一体化趋势，以客户需求为导向，以生态场景为触点，以API/SDK 等技术为手段，以服务碎片化、数据商业化为特征，通过与第三方数据、算法、业务、流程等的融合，实现业务驱动的应用架构转型，从前台到后台的整体体系升级，从而变成新时代银行。

**麦肯锡**(McKinsey & Company，MCK)认为，开放银行可简单定义为由互不相关的两方或多方利用 API 接口共享金融数据的一种合作模式。

**高德纳**(Gartner Group，Gartner)认为，开放银行是一种平台化商业模式，通过与商业生态系统共享数据、算法、交易、流程和其他业务功能，为商业生态系统的客户、员工、第三方开发者、金融科技公司、供应商和其他合作伙伴提供服务，使银行创造出新的价值，构建新的核心能力。

>综合以上各方对开放银行的理解，可以认为，开放银行是以客户为中心，以生态场景为触点，以 API/SDK 等技术为手段，以服务微型化、碎片化为特征，银行通过与第三方数据、业务等的共享融合来满足客户需求的平台商业模式。

### 开放银行的提出

开放银行由英文Open Banking 翻译而来，由英国提出，起源和推广是英国和欧盟关于银行业的数据共享和开放数据的探索，是一种利用开放API技术，让提供商访问客户财务信息的安全方法。一方面，可以让客户更详细的了解自己的账户；另一方面，客户可以通过第三方提供享受更好的金融服务。

- [**PSD2**](https://www.gemalto.com/financial/ebanking/psd2)《支付服务指令2》(Payment Services Directive 2)
  - 强客户认证（Strong Customer Authentication ,SCA），利用二个或多个元素进行身份验证：
    - 第一个元素是私密信息【自由客户知道的内容：密码/个人识别码/身份证号码】
    - 第二个元素是所有权【只有用户拥有的东西：移动设备/通证/智能卡】
    - 第三个元素是独特性【只有用户才拥有的东西：指纹/人脸/语言识别】

![psd2 compliance](../images/infog.png)

- 开放银行与PSD2的关系：开放银行是英国版的PSD2
  - PSD2仅要求银行开放数据，并没有规定API的接口标准和开放数据的内容，它是为了纯粹技术标准而建立的组织,主要工作是制定独立的银行间开放和共享标准。

此后，非欧盟国家的银行也开始纷纷自发行动，积极构建自己的开放银行。
  - 新加坡
  - 韩国
  - 澳大利亚

### 开放银行的驱动因素

> 银行拥有海量的、丰富的、高质量的数据资源以及可信的客户关系，虽然大都处于分散和割裂的状态，但这些资源背后蕴藏着巨大的行业价值。

在客户对金融服务要求越来越高、科技界的巨头跨国竞争越来越激烈、社会和监管对开放数据的呼声越来越强烈的大潮下，银行数据开放是不可避免的趋势。

数字化进程带来了三项重要改变：

- 第一，客户对于产品和服务的即时性和便捷性要求越来越高
- 第二，有关客户的行为信息和与用户的触达点都从线下转移到了线上
- 第三，用户转换服务提高上的门槛越来越低，用户忠诚度极大地取决与产品和服务是否满足其需求

银行作为市场主体，未来的方向就是无边界的银行服务，因此很多银行积极投身开放银行的实践。

### 开放银行开放什么

- 英国《调查令》授权的开放和通用银行标准，允许开放三部分数据和信息：
  - 第一部分是通过开放数据API发布参考信息
    - 所有分支机构的位置、所有分支机构开放时间、所有ATM地点信息
  - 第二部分是通过开放数据API发布特点产品信息
    - 产品价格、费用（利息）、特点和优点、条款和条件以及客户资格
  - 第三部分是通过可读或可写API发布个人活期账户和企业活期账户交易信息
    - 允许第三方提供商客户要求访问账户信息或从客户账户付款。
  - 面向开放银行目录（Open Banking Directory）上第三方提供商开放